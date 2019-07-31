---
title: Atualizar windows10EndpointProtectionConfiguration
description: Atualizar as propriedades de um objeto windows10EndpointProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8f28c883a33271878cda8790e5358b8b22b50c5e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976884"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="d0005-103">Atualizar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0005-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="d0005-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d0005-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0005-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0005-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0005-106">Atualizar as propriedades de um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0005-106">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0005-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d0005-107">Prerequisites</span></span>
<span data-ttu-id="d0005-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0005-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0005-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d0005-110">Permission type</span></span>|<span data-ttu-id="d0005-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d0005-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0005-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d0005-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0005-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0005-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0005-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d0005-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0005-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0005-115">Not supported.</span></span>|
|<span data-ttu-id="d0005-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d0005-116">Application</span></span>|<span data-ttu-id="d0005-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d0005-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0005-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d0005-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d0005-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d0005-119">Request headers</span></span>
|<span data-ttu-id="d0005-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d0005-120">Header</span></span>|<span data-ttu-id="d0005-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d0005-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0005-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d0005-122">Authorization</span></span>|<span data-ttu-id="d0005-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0005-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0005-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d0005-124">Accept</span></span>|<span data-ttu-id="d0005-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0005-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0005-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d0005-126">Request body</span></span>
<span data-ttu-id="d0005-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0005-127">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="d0005-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0005-128">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="d0005-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0005-129">Property</span></span>|<span data-ttu-id="d0005-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0005-130">Type</span></span>|<span data-ttu-id="d0005-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0005-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0005-132">id</span><span class="sxs-lookup"><span data-stu-id="d0005-132">id</span></span>|<span data-ttu-id="d0005-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0005-133">String</span></span>|<span data-ttu-id="d0005-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d0005-134">Key of the entity.</span></span> <span data-ttu-id="d0005-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0005-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0005-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0005-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d0005-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0005-137">DateTimeOffset</span></span>|<span data-ttu-id="d0005-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d0005-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d0005-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0005-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0005-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d0005-140">roleScopeTagIds</span></span>|<span data-ttu-id="d0005-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0005-141">String collection</span></span>|<span data-ttu-id="d0005-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d0005-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d0005-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0005-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0005-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d0005-144">supportsScopeTags</span></span>|<span data-ttu-id="d0005-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-145">Boolean</span></span>|<span data-ttu-id="d0005-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d0005-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d0005-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d0005-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d0005-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d0005-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d0005-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d0005-149">This property is read-only.</span></span> <span data-ttu-id="d0005-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0005-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0005-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d0005-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d0005-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d0005-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d0005-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="d0005-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d0005-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0005-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0005-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d0005-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d0005-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d0005-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d0005-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="d0005-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d0005-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0005-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0005-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d0005-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d0005-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d0005-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d0005-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="d0005-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d0005-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0005-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0005-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0005-163">createdDateTime</span></span>|<span data-ttu-id="d0005-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0005-164">DateTimeOffset</span></span>|<span data-ttu-id="d0005-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d0005-165">DateTime the object was created.</span></span> <span data-ttu-id="d0005-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0005-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0005-167">descrição</span><span class="sxs-lookup"><span data-stu-id="d0005-167">description</span></span>|<span data-ttu-id="d0005-168">String</span><span class="sxs-lookup"><span data-stu-id="d0005-168">String</span></span>|<span data-ttu-id="d0005-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0005-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d0005-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0005-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0005-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d0005-171">displayName</span></span>|<span data-ttu-id="d0005-172">String</span><span class="sxs-lookup"><span data-stu-id="d0005-172">String</span></span>|<span data-ttu-id="d0005-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0005-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d0005-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0005-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0005-175">versão</span><span class="sxs-lookup"><span data-stu-id="d0005-175">version</span></span>|<span data-ttu-id="d0005-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d0005-176">Int32</span></span>|<span data-ttu-id="d0005-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0005-177">Version of the device configuration.</span></span> <span data-ttu-id="d0005-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0005-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0005-179">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="d0005-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="d0005-180">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="d0005-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="d0005-181">Essa política destina-se a fornecer segurança adicional contra dispositivos compatíveis com DMA externo.</span><span class="sxs-lookup"><span data-stu-id="d0005-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="d0005-182">Permite mais controle sobre a enumeração de dispositivos compatíveis com DMA externo incompatíveis com o remapeamento de DMA/isolamento de memória do dispositivo e área restrita.</span><span class="sxs-lookup"><span data-stu-id="d0005-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="d0005-183">Essa política só entra em vigor quando a proteção DMA de kernel é suportada e habilitada pelo firmware do sistema.</span><span class="sxs-lookup"><span data-stu-id="d0005-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="d0005-184">A proteção DMA de kernel é um recurso de plataforma que não pode ser controlado via política ou pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="d0005-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="d0005-185">É preciso ter suporte do sistema no momento da fabricação.</span><span class="sxs-lookup"><span data-stu-id="d0005-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="d0005-186">Para verificar se o sistema suporta a proteção DMA de kernel, verifique o campo proteção DMA de kernel na página Resumo de MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="d0005-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="d0005-187">Os valores possíveis são: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="d0005-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="d0005-188">firewallRules</span><span class="sxs-lookup"><span data-stu-id="d0005-188">firewallRules</span></span>|<span data-ttu-id="d0005-189">coleção [windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="d0005-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="d0005-190">Define as configurações da regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="d0005-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="d0005-191">Essa coleção pode conter um máximo de 150 elementos.</span><span class="sxs-lookup"><span data-stu-id="d0005-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="d0005-192">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="d0005-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="d0005-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-194">Esse direito de usuário é usado pelo Gerenciador de credenciais durante o backup/restauração.</span><span class="sxs-lookup"><span data-stu-id="d0005-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="d0005-195">As credenciais salvas dos usuários podem ser comprometidas se esse privilégio for dado a outras entidades.</span><span class="sxs-lookup"><span data-stu-id="d0005-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="d0005-196">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="d0005-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0005-197">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="d0005-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="d0005-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-199">Esse direito de usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="d0005-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="d0005-200">O estado permitido é suportado.</span><span class="sxs-lookup"><span data-stu-id="d0005-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="d0005-201">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="d0005-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="d0005-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-203">Esse direito de usuário determina quais usuários e grupos são bloqueados para se conectarem ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="d0005-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="d0005-204">Há suporte para o bloco de estado.</span><span class="sxs-lookup"><span data-stu-id="d0005-204">State Block is supported.</span></span>|
|<span data-ttu-id="d0005-205">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d0005-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="d0005-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-207">Esse direito de usuário permite que um processo represente qualquer usuário sem autenticação.</span><span class="sxs-lookup"><span data-stu-id="d0005-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="d0005-208">Portanto, o processo pode ter acesso aos mesmos recursos locais que esse usuário.</span><span class="sxs-lookup"><span data-stu-id="d0005-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="d0005-209">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="d0005-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0005-210">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="d0005-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="d0005-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-212">Esse direito de usuário determina quais usuários podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="d0005-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="d0005-213">Estados não configurados, permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="d0005-213">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="d0005-214">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="d0005-214">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="d0005-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-216">Esse direito de usuário determina quais usuários não podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="d0005-216">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="d0005-217">Estados não configurados, bloqueados são suportados</span><span class="sxs-lookup"><span data-stu-id="d0005-217">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="d0005-218">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="d0005-218">userRightsBackupData</span></span>|[<span data-ttu-id="d0005-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-220">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao fazer backup de arquivos e diretórios.</span><span class="sxs-lookup"><span data-stu-id="d0005-220">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="d0005-221">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="d0005-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0005-222">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="d0005-222">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="d0005-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-224">Este direito de usuário determina quais usuários e grupos podem alterar a hora e a data no relógio interno do computador.</span><span class="sxs-lookup"><span data-stu-id="d0005-224">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="d0005-225">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="d0005-225">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0005-226">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="d0005-226">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="d0005-227">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-227">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-228">Configuração de segurança que determina se os usuários podem criar objetos globais que estão disponíveis para todas as sessões.</span><span class="sxs-lookup"><span data-stu-id="d0005-228">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="d0005-229">Os usuários que podem criar objetos globais podem afetar processos executados em sessões de outros usuários, o que pode levar a falhas de aplicativos ou corrupção de dados.</span><span class="sxs-lookup"><span data-stu-id="d0005-229">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="d0005-230">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="d0005-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0005-231">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="d0005-231">userRightsCreatePageFile</span></span>|[<span data-ttu-id="d0005-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-233">Esse direito de usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de paginação.</span><span class="sxs-lookup"><span data-stu-id="d0005-233">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="d0005-234">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="d0005-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0005-235">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="d0005-235">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="d0005-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-237">Este direito de usuário determina quais contas podem ser usadas por processos para criar um objeto de diretório usando o Gerenciador de objetos.</span><span class="sxs-lookup"><span data-stu-id="d0005-237">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="d0005-238">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="d0005-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0005-239">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="d0005-239">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="d0005-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-241">Esse direito de usuário determina se o usuário pode criar um link simbólico do computador no qual está conectado.</span><span class="sxs-lookup"><span data-stu-id="d0005-241">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="d0005-242">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="d0005-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0005-243">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="d0005-243">userRightsCreateToken</span></span>|[<span data-ttu-id="d0005-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-245">Esse direito de usuário determina quais usuários/grupos podem ser usados por processos para criar um token que pode ser usado para obter acesso a qualquer recurso local quando o processo usa uma API interna para criar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="d0005-245">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="d0005-246">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="d0005-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0005-247">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="d0005-247">userRightsDebugPrograms</span></span>|[<span data-ttu-id="d0005-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-249">Esse direito de usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel.</span><span class="sxs-lookup"><span data-stu-id="d0005-249">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="d0005-250">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="d0005-250">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="d0005-251">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="d0005-251">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="d0005-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-253">Este direito de usuário determina quais usuários e grupos estão proibidos de fazer logon como um cliente de serviços de área de trabalho remota.</span><span class="sxs-lookup"><span data-stu-id="d0005-253">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="d0005-254">Há suporte apenas para os Estados não configurados e bloqueados</span><span class="sxs-lookup"><span data-stu-id="d0005-254">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="d0005-255">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="d0005-255">userRightsDelegation</span></span>|[<span data-ttu-id="d0005-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-257">Este direito de usuário determina quais usuários podem definir a configuração confiável para delegação em um objeto de usuário ou computador.</span><span class="sxs-lookup"><span data-stu-id="d0005-257">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="d0005-258">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-258">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-259">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="d0005-259">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="d0005-260">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-260">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-261">Este direito de usuário determina quais contas podem ser usadas por um processo para adicionar entradas ao log de segurança.</span><span class="sxs-lookup"><span data-stu-id="d0005-261">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="d0005-262">O log de segurança é usado para rastrear o acesso de sistema não autorizado.</span><span class="sxs-lookup"><span data-stu-id="d0005-262">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="d0005-263">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-263">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-264">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="d0005-264">userRightsImpersonateClient</span></span>|[<span data-ttu-id="d0005-265">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-265">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-266">A atribuição desse direito de usuário a um usuário permite que programas executados em nome desse usuário representem um cliente.</span><span class="sxs-lookup"><span data-stu-id="d0005-266">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="d0005-267">A exigência desse direito de usuário para esse tipo de representação impede que um usuário não autorizado convença um cliente a se conectar a um serviço que ele criou e, em seguida, representando esse cliente, o que pode elevar as permissões do usuário não autorizado para níveis administrativos ou de sistema.</span><span class="sxs-lookup"><span data-stu-id="d0005-267">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="d0005-268">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-269">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="d0005-269">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="d0005-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-271">Este direito de usuário determina quais contas podem usar um processo com acesso de propriedade de gravação a outro processo para aumentar a prioridade de execução atribuída ao outro processo.</span><span class="sxs-lookup"><span data-stu-id="d0005-271">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="d0005-272">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-273">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="d0005-273">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="d0005-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-275">Esse direito de usuário determina quais usuários podem carregar e descarregar dinamicamente drivers de dispositivo ou outro código no modo kernel.</span><span class="sxs-lookup"><span data-stu-id="d0005-275">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="d0005-276">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-277">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="d0005-277">userRightsLockMemory</span></span>|[<span data-ttu-id="d0005-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-279">Esse direito de usuário determina quais contas podem usar um processo para manter os dados na memória física, o que impede que o sistema pagine os dados para a memória virtual em disco.</span><span class="sxs-lookup"><span data-stu-id="d0005-279">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="d0005-280">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-281">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="d0005-281">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="d0005-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-283">Esse direito de usuário determina quais usuários podem especificar opções de auditoria de acesso a objetos para recursos individuais, como arquivos, objetos do Active Directory e chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="d0005-283">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="d0005-284">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-285">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="d0005-285">userRightsManageVolumes</span></span>|[<span data-ttu-id="d0005-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-287">Esse direito de usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como a desfragmentação remota.</span><span class="sxs-lookup"><span data-stu-id="d0005-287">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="d0005-288">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-289">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="d0005-289">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="d0005-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-291">Esse direito de usuário determina quem pode modificar os valores de ambiente de firmware.</span><span class="sxs-lookup"><span data-stu-id="d0005-291">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="d0005-292">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-293">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="d0005-293">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="d0005-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-295">Este direito de usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves de registro ou processos pertencentes a outros usuários.</span><span class="sxs-lookup"><span data-stu-id="d0005-295">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="d0005-296">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-297">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="d0005-297">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="d0005-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-299">Esse direito de usuário determina quais usuários podem usar ferramentas de monitoramento de desempenho para monitorar o desempenho de processos do sistema.</span><span class="sxs-lookup"><span data-stu-id="d0005-299">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="d0005-300">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-300">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-301">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="d0005-301">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="d0005-302">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-302">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-303">Esse direito de usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede.</span><span class="sxs-lookup"><span data-stu-id="d0005-303">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="d0005-304">O mau uso desse direito de usuário pode resultar em uma negação de serviço.</span><span class="sxs-lookup"><span data-stu-id="d0005-304">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="d0005-305">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-306">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="d0005-306">userRightsRestoreData</span></span>|[<span data-ttu-id="d0005-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-308">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao restaurar backups de arquivos e diretórios e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto.</span><span class="sxs-lookup"><span data-stu-id="d0005-308">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="d0005-309">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-310">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="d0005-310">userRightsTakeOwnership</span></span>|[<span data-ttu-id="d0005-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-312">Esse direito de usuário determina quais usuários podem assumir a propriedade de qualquer objeto protegível no sistema, incluindo objetos do Active Directory, arquivos e pastas, impressoras, chaves do registro, processos e threads.</span><span class="sxs-lookup"><span data-stu-id="d0005-312">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="d0005-313">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-313">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="d0005-314">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="d0005-314">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="d0005-315">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="d0005-315">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="d0005-316">Essa configuração de segurança determina quais contas de serviço são impedidas de registrar um processo como um serviço.</span><span class="sxs-lookup"><span data-stu-id="d0005-316">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="d0005-317">Observação: esta configuração de segurança não se aplica às contas de sistema, serviço local ou serviço de rede.</span><span class="sxs-lookup"><span data-stu-id="d0005-317">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="d0005-318">Só há suporte para o estado bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d0005-318">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="d0005-319">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="d0005-319">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="d0005-320">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-320">Boolean</span></span>|<span data-ttu-id="d0005-321">Essa configuração determina se o salvamento de jogos do Xbox está habilitado (1) ou desabilitado (0).</span><span class="sxs-lookup"><span data-stu-id="d0005-321">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="d0005-322">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="d0005-322">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="d0005-323">instarttype</span><span class="sxs-lookup"><span data-stu-id="d0005-323">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d0005-324">Esta configuração determina se o tipo de início do serviço de gerenciamento de acessórios é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="d0005-324">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d0005-325">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="d0005-325">Default: Manual.</span></span> <span data-ttu-id="d0005-326">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0005-326">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d0005-327">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="d0005-327">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="d0005-328">instarttype</span><span class="sxs-lookup"><span data-stu-id="d0005-328">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d0005-329">Essa configuração determina se o tipo de início do serviço do Live Authentication Manager é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="d0005-329">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d0005-330">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="d0005-330">Default: Manual.</span></span> <span data-ttu-id="d0005-331">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0005-331">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d0005-332">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="d0005-332">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="d0005-333">instarttype</span><span class="sxs-lookup"><span data-stu-id="d0005-333">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d0005-334">Essa configuração determina se o tipo de início do serviço de salvamento do Live Game é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="d0005-334">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d0005-335">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="d0005-335">Default: Manual.</span></span> <span data-ttu-id="d0005-336">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0005-336">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d0005-337">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="d0005-337">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="d0005-338">instarttype</span><span class="sxs-lookup"><span data-stu-id="d0005-338">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="d0005-339">Esta configuração determina se o tipo de início do serviço de rede é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="d0005-339">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="d0005-340">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="d0005-340">Default: Manual.</span></span> <span data-ttu-id="d0005-341">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0005-341">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="d0005-342">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="d0005-342">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="d0005-343">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-343">Boolean</span></span>|<span data-ttu-id="d0005-344">Impedir que os usuários adicionem novas contas da Microsoft a este computador.</span><span class="sxs-lookup"><span data-stu-id="d0005-344">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="d0005-345">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="d0005-345">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="d0005-346">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-346">Boolean</span></span>|<span data-ttu-id="d0005-347">Habilitar contas locais que não estão protegidas por senha para fazer logon de locais diferentes do dispositivo físico. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="d0005-347">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="d0005-348">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="d0005-348">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="d0005-349">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-349">Boolean</span></span>|<span data-ttu-id="d0005-350">Determina se a conta de administrador local está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="d0005-350">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="d0005-351">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="d0005-351">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="d0005-352">String</span><span class="sxs-lookup"><span data-stu-id="d0005-352">String</span></span>|<span data-ttu-id="d0005-353">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "administrador".</span><span class="sxs-lookup"><span data-stu-id="d0005-353">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="d0005-354">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="d0005-354">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="d0005-355">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-355">Boolean</span></span>|<span data-ttu-id="d0005-356">Determina se a conta de convidado está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="d0005-356">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="d0005-357">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="d0005-357">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="d0005-358">String</span><span class="sxs-lookup"><span data-stu-id="d0005-358">String</span></span>|<span data-ttu-id="d0005-359">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "convidado".</span><span class="sxs-lookup"><span data-stu-id="d0005-359">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="d0005-360">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="d0005-360">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="d0005-361">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-361">Boolean</span></span>|<span data-ttu-id="d0005-362">Impedir que um computador portátil seja desencaixado sem ter que fazer logon.</span><span class="sxs-lookup"><span data-stu-id="d0005-362">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="d0005-363">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="d0005-363">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="d0005-364">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-364">Boolean</span></span>|<span data-ttu-id="d0005-365">Restringir a instalação dos drivers de impressora como parte da conexão a uma impressora compartilhada somente para administradores.</span><span class="sxs-lookup"><span data-stu-id="d0005-365">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="d0005-366">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="d0005-366">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="d0005-367">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-367">Boolean</span></span>|<span data-ttu-id="d0005-368">Habilitar essa configuração permite que somente o usuário conectado interativamente acesse a mídia de CD-ROM.</span><span class="sxs-lookup"><span data-stu-id="d0005-368">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="d0005-369">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="d0005-369">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="d0005-370">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="d0005-370">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="d0005-371">Defina quem tem permissão para formatar e ejetar a mídia NTFS removível.</span><span class="sxs-lookup"><span data-stu-id="d0005-371">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="d0005-372">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="d0005-372">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="d0005-373">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="d0005-373">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="d0005-374">Int32</span><span class="sxs-lookup"><span data-stu-id="d0005-374">Int32</span></span>|<span data-ttu-id="d0005-375">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="d0005-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="d0005-376">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="d0005-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="d0005-377">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="d0005-377">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="d0005-378">Int32</span><span class="sxs-lookup"><span data-stu-id="d0005-378">Int32</span></span>|<span data-ttu-id="d0005-379">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="d0005-379">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="d0005-380">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="d0005-380">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="d0005-381">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="d0005-381">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="d0005-382">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-382">Boolean</span></span>|<span data-ttu-id="d0005-383">Exigir CTRL + ALT + DEL para ser pressionada para que um usuário possa fazer logon.</span><span class="sxs-lookup"><span data-stu-id="d0005-383">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="d0005-384">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="d0005-384">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="d0005-385">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-385">Boolean</span></span>|<span data-ttu-id="d0005-386">Não exibe o nome de usuário da última pessoa que entrou neste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0005-386">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="d0005-387">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="d0005-387">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="d0005-388">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-388">Boolean</span></span>|<span data-ttu-id="d0005-389">Não exibe o nome de usuário da pessoa que está entrando neste dispositivo depois que as credenciais são inseridas e antes da área de trabalho do dispositivo ser exibida.</span><span class="sxs-lookup"><span data-stu-id="d0005-389">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="d0005-390">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="d0005-390">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="d0005-391">String</span><span class="sxs-lookup"><span data-stu-id="d0005-391">String</span></span>|<span data-ttu-id="d0005-392">Defina o título da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="d0005-392">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="d0005-393">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="d0005-393">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="d0005-394">String</span><span class="sxs-lookup"><span data-stu-id="d0005-394">String</span></span>|<span data-ttu-id="d0005-395">Definir o texto da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="d0005-395">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="d0005-396">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="d0005-396">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="d0005-397">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-397">Boolean</span></span>|<span data-ttu-id="d0005-398">Bloquear solicitações de autenticação PKU2U para este dispositivo para usar identidades online.</span><span class="sxs-lookup"><span data-stu-id="d0005-398">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="d0005-399">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="d0005-399">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="d0005-400">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-400">Boolean</span></span>|<span data-ttu-id="d0005-401">Boolean do auxiliar da interface do usuário para entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="d0005-401">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="d0005-402">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="d0005-402">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="d0005-403">String</span><span class="sxs-lookup"><span data-stu-id="d0005-403">String</span></span>|<span data-ttu-id="d0005-404">Edite a cadeia de caracteres de definição de descritor de segurança padrão para permitir ou impedir que usuários e grupos façam chamadas remotas para o SAM.</span><span class="sxs-lookup"><span data-stu-id="d0005-404">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="d0005-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="d0005-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="d0005-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="d0005-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="d0005-407">Essa configuração de segurança permite que um cliente exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="d0005-407">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="d0005-408">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="d0005-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="d0005-409">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="d0005-409">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="d0005-410">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="d0005-410">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="d0005-411">Essa configuração de segurança permite que um servidor exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="d0005-411">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="d0005-412">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="d0005-412">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="d0005-413">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="d0005-413">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="d0005-414">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="d0005-414">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="d0005-415">Essa configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede.</span><span class="sxs-lookup"><span data-stu-id="d0005-415">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="d0005-416">Os possíveis valores são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="d0005-416">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="d0005-417">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="d0005-417">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="d0005-418">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-418">Boolean</span></span>|<span data-ttu-id="d0005-419">Se for habilitada, o cliente SMB permitirá logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="d0005-419">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="d0005-420">Se não configurada, o cliente SMB rejeitará logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="d0005-420">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="d0005-421">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="d0005-421">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="d0005-422">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-422">Boolean</span></span>|<span data-ttu-id="d0005-423">Configuração de segurança que determina se o arquivo de paginação de memória virtual será limpo quando o sistema for desligado.</span><span class="sxs-lookup"><span data-stu-id="d0005-423">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="d0005-424">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="d0005-424">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="d0005-425">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-425">Boolean</span></span>|<span data-ttu-id="d0005-426">Configuração de segurança que determina se um computador pode ser desligado sem a necessidade de fazer logon no Windows.</span><span class="sxs-lookup"><span data-stu-id="d0005-426">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="d0005-427">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="d0005-427">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="d0005-428">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-428">Boolean</span></span>|<span data-ttu-id="d0005-429">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="d0005-429">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="d0005-430">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="d0005-430">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="d0005-431">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-431">Boolean</span></span>|<span data-ttu-id="d0005-432">Virtualizar falhas de gravação de arquivo e registro para locais por usuário</span><span class="sxs-lookup"><span data-stu-id="d0005-432">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="d0005-433">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="d0005-433">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="d0005-434">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-434">Boolean</span></span>|<span data-ttu-id="d0005-435">Impor a validação de caminho de certificação PKI para um determinado arquivo executável antes que seja permitido executar.</span><span class="sxs-lookup"><span data-stu-id="d0005-435">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="d0005-436">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="d0005-436">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="d0005-437">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="d0005-437">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="d0005-438">Definir o comportamento do prompt de elevação para administradores no modo de aprovação de administrador.</span><span class="sxs-lookup"><span data-stu-id="d0005-438">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="d0005-439">Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="d0005-439">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="d0005-440">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="d0005-440">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="d0005-441">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="d0005-441">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="d0005-442">Definir o comportamento do prompt de elevação para usuários padrão.</span><span class="sxs-lookup"><span data-stu-id="d0005-442">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="d0005-443">Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="d0005-443">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="d0005-444">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="d0005-444">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="d0005-445">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-445">Boolean</span></span>|<span data-ttu-id="d0005-446">Habilite todas as solicitações de elevação para ir para a área de trabalho do usuário interativo, e não para a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="d0005-446">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="d0005-447">As configurações de política de comportamento de prompt para administradores e usuários padrão são usadas.</span><span class="sxs-lookup"><span data-stu-id="d0005-447">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="d0005-448">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="d0005-448">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="d0005-449">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-449">Boolean</span></span>|<span data-ttu-id="d0005-450">Instalações de aplicativos que exigem privilégios elevados solicitarão credenciais de administrador. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="d0005-450">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="d0005-451">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="d0005-451">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="d0005-452">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-452">Boolean</span></span>|<span data-ttu-id="d0005-453">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="d0005-453">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="d0005-454">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="d0005-454">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="d0005-455">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-455">Boolean</span></span>|<span data-ttu-id="d0005-456">Define se a conta de administrador interna usa o modo de aprovação de administrador ou executa todos os aplicativos com privilégios de administrador completo. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="d0005-456">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="d0005-457">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="d0005-457">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="d0005-458">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-458">Boolean</span></span>|<span data-ttu-id="d0005-459">Definir se o modo de aprovação de administrador e todas as configurações de política de UAC estão habilitados, o padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="d0005-459">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="d0005-460">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="d0005-460">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="d0005-461">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="d0005-461">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="d0005-462">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d0005-462">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="d0005-463">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-463">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="d0005-464">Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="d0005-464">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="d0005-465">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="d0005-465">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="d0005-466">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="d0005-466">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="d0005-467">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d0005-467">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="d0005-468">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="d0005-468">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="d0005-469">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="d0005-469">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="d0005-470">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="d0005-470">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="d0005-471">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-471">Boolean</span></span>|<span data-ttu-id="d0005-472">Configuração de segurança que determina se o cliente SMB tentará negociar assinatura de pacote SMB.</span><span class="sxs-lookup"><span data-stu-id="d0005-472">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="d0005-473">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="d0005-473">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="d0005-474">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-474">Boolean</span></span>|<span data-ttu-id="d0005-475">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do cliente SMB.</span><span class="sxs-lookup"><span data-stu-id="d0005-475">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="d0005-476">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="d0005-476">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="d0005-477">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-477">Boolean</span></span>|<span data-ttu-id="d0005-478">Se essa configuração de segurança estiver habilitada, o redirecionador de bloco de mensagens de servidor (SMB) terá permissão para enviar senhas de texto não criptografado para servidores SMB não Microsoft que não ofereçam suporte à criptografia de senha durante a autenticação.</span><span class="sxs-lookup"><span data-stu-id="d0005-478">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="d0005-479">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="d0005-479">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="d0005-480">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-480">Boolean</span></span>|<span data-ttu-id="d0005-481">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do servidor SMB.</span><span class="sxs-lookup"><span data-stu-id="d0005-481">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="d0005-482">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="d0005-482">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="d0005-483">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-483">Boolean</span></span>|<span data-ttu-id="d0005-484">Configuração de segurança que determina se o servidor SMB negociará assinatura de pacote SMB com clientes que solicitarem.</span><span class="sxs-lookup"><span data-stu-id="d0005-484">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="d0005-485">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="d0005-485">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="d0005-486">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-486">Boolean</span></span>|<span data-ttu-id="d0005-487">Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e pipes para as configurações de pipes nomeados que podem ser acessados anonimamente e compartilhamentos que podem ser acessados anonimamente</span><span class="sxs-lookup"><span data-stu-id="d0005-487">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="d0005-488">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="d0005-488">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="d0005-489">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-489">Boolean</span></span>|<span data-ttu-id="d0005-490">Essa configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas com o computador.</span><span class="sxs-lookup"><span data-stu-id="d0005-490">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="d0005-491">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="d0005-491">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="d0005-492">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-492">Boolean</span></span>|<span data-ttu-id="d0005-493">Configuração de segurança que determina se os usuários anônimos devem executar determinadas atividades, como enumeração de nomes de contas de domínio e compartilhamentos de rede.</span><span class="sxs-lookup"><span data-stu-id="d0005-493">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="d0005-494">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="d0005-494">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="d0005-495">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-495">Boolean</span></span>|<span data-ttu-id="d0005-496">Essa configuração de segurança determina se, na próxima alteração de senha, o valor de hash do LM (LAN Manager) para a nova senha é armazenado.</span><span class="sxs-lookup"><span data-stu-id="d0005-496">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="d0005-497">Ele não é armazenado por padrão.</span><span class="sxs-lookup"><span data-stu-id="d0005-497">It’s not stored by default.</span></span>|
|<span data-ttu-id="d0005-498">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="d0005-498">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="d0005-499">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="d0005-499">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="d0005-500">Essa configuração de segurança determina o que acontece quando o cartão inteligente de um usuário conectado é removido do leitor de cartão inteligente.</span><span class="sxs-lookup"><span data-stu-id="d0005-500">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="d0005-501">Os valores possíveis são: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="d0005-501">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="d0005-502">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="d0005-502">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="d0005-503">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-503">Boolean</span></span>|<span data-ttu-id="d0005-504">Usado para desabilitar a exibição da área de proteção de aplicativo e navegador.</span><span class="sxs-lookup"><span data-stu-id="d0005-504">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="d0005-505">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="d0005-505">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="d0005-506">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-506">Boolean</span></span>|<span data-ttu-id="d0005-507">Usado para desabilitar a exibição da área de opções da família.</span><span class="sxs-lookup"><span data-stu-id="d0005-507">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="d0005-508">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="d0005-508">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="d0005-509">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-509">Boolean</span></span>|<span data-ttu-id="d0005-510">Usado para desabilitar a exibição da área de desempenho e integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0005-510">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="d0005-511">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="d0005-511">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="d0005-512">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-512">Boolean</span></span>|<span data-ttu-id="d0005-513">Usado para desabilitar a exibição da área de firewall e proteção de rede.</span><span class="sxs-lookup"><span data-stu-id="d0005-513">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="d0005-514">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="d0005-514">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="d0005-515">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-515">Boolean</span></span>|<span data-ttu-id="d0005-516">Usado para desabilitar a exibição da área de proteção contra vírus e ameaças.</span><span class="sxs-lookup"><span data-stu-id="d0005-516">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="d0005-517">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="d0005-517">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="d0005-518">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-518">Boolean</span></span>|<span data-ttu-id="d0005-519">Usado para desabilitar a exibição da área de proteção da conta.</span><span class="sxs-lookup"><span data-stu-id="d0005-519">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="d0005-520">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="d0005-520">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="d0005-521">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-521">Boolean</span></span>|<span data-ttu-id="d0005-522">Usado para desabilitar a exibição do botão limpar TPM.</span><span class="sxs-lookup"><span data-stu-id="d0005-522">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="d0005-523">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="d0005-523">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="d0005-524">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-524">Boolean</span></span>|<span data-ttu-id="d0005-525">Usado para desabilitar a exibição da área de proteção de hardware.</span><span class="sxs-lookup"><span data-stu-id="d0005-525">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="d0005-526">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="d0005-526">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="d0005-527">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-527">Boolean</span></span>|<span data-ttu-id="d0005-528">Usado para desabilitar a exibição do controle da área de notificação.</span><span class="sxs-lookup"><span data-stu-id="d0005-528">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="d0005-529">O usuário precisa sair e entrar ou reiniciar o computador para que essa configuração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="d0005-529">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="d0005-530">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="d0005-530">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="d0005-531">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-531">Boolean</span></span>|<span data-ttu-id="d0005-532">Usado para desabilitar a exibição da área de proteção contra ransomware.</span><span class="sxs-lookup"><span data-stu-id="d0005-532">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="d0005-533">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="d0005-533">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="d0005-534">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-534">Boolean</span></span>|<span data-ttu-id="d0005-535">Usado para desabilitar a exibição da área de inicialização segura sob segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0005-535">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="d0005-536">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="d0005-536">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="d0005-537">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-537">Boolean</span></span>|<span data-ttu-id="d0005-538">Usado para desabilitar a exibição do processo de segurança Solucionando problemas de segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d0005-538">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="d0005-539">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="d0005-539">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="d0005-540">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-540">Boolean</span></span>|<span data-ttu-id="d0005-541">Usado para desabilitar a exibição de atualizar o firmware do TPM quando um firmware vulnerável é detectado.</span><span class="sxs-lookup"><span data-stu-id="d0005-541">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="d0005-542">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="d0005-542">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="d0005-543">String</span><span class="sxs-lookup"><span data-stu-id="d0005-543">String</span></span>|<span data-ttu-id="d0005-544">O nome da empresa que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="d0005-544">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="d0005-545">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="d0005-545">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="d0005-546">String</span><span class="sxs-lookup"><span data-stu-id="d0005-546">String</span></span>|<span data-ttu-id="d0005-547">O endereço de email que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="d0005-547">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="d0005-548">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="d0005-548">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="d0005-549">String</span><span class="sxs-lookup"><span data-stu-id="d0005-549">String</span></span>|<span data-ttu-id="d0005-550">O número de telefone ou Skype ID que é exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="d0005-550">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="d0005-551">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="d0005-551">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="d0005-552">String</span><span class="sxs-lookup"><span data-stu-id="d0005-552">String</span></span>|<span data-ttu-id="d0005-553">A URL do portal da ajuda que é exibida para os usuários.</span><span class="sxs-lookup"><span data-stu-id="d0005-553">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="d0005-554">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="d0005-554">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="d0005-555">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="d0005-555">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="d0005-556">Notificações para mostrar das áreas de aplicativo exibidas.</span><span class="sxs-lookup"><span data-stu-id="d0005-556">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="d0005-557">Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="d0005-557">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="d0005-558">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="d0005-558">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="d0005-559">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="d0005-559">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="d0005-560">Configurar onde exibir informações de contato de ti para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="d0005-560">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="d0005-561">Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="d0005-561">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="d0005-562">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="d0005-562">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="d0005-563">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="d0005-563">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="d0005-564">Defina as configurações do Windows Defender TamperProtection.</span><span class="sxs-lookup"><span data-stu-id="d0005-564">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="d0005-565">Os valores possíveis são: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="d0005-565">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="d0005-566">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="d0005-566">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="d0005-567">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-567">Boolean</span></span>|<span data-ttu-id="d0005-568">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="d0005-568">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="d0005-569">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="d0005-569">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="d0005-570">Int32</span><span class="sxs-lookup"><span data-stu-id="d0005-570">Int32</span></span>|<span data-ttu-id="d0005-571">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="d0005-571">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="d0005-572">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="d0005-572">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="d0005-573">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="d0005-573">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="d0005-574">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="d0005-574">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="d0005-575">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="d0005-575">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="d0005-576">Selecione a codificação de chave pré-compartilhada a ser usada.</span><span class="sxs-lookup"><span data-stu-id="d0005-576">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="d0005-577">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="d0005-577">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="d0005-578">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="d0005-578">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="d0005-579">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-579">Boolean</span></span>|<span data-ttu-id="d0005-580">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="d0005-580">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="d0005-581">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="d0005-581">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="d0005-582">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-582">Boolean</span></span>|<span data-ttu-id="d0005-583">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="d0005-583">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="d0005-584">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="d0005-584">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="d0005-585">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-585">Boolean</span></span>|<span data-ttu-id="d0005-586">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="d0005-586">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="d0005-587">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="d0005-587">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="d0005-588">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-588">Boolean</span></span>|<span data-ttu-id="d0005-589">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="d0005-589">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="d0005-590">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="d0005-590">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="d0005-591">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="d0005-591">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="d0005-592">Especifique como a lista de certificados revogados será imposta.</span><span class="sxs-lookup"><span data-stu-id="d0005-592">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="d0005-593">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="d0005-593">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="d0005-594">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="d0005-594">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="d0005-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0005-595">Boolean</span></span>|<span data-ttu-id="d0005-596">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="d0005-596">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="d0005-597">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="d0005-597">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="d0005-598">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="d0005-598">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="d0005-599">Configura como o enfileiramento de pacotes deve ser aplicado no cenário de gateway de túnel.</span><span class="sxs-lookup"><span data-stu-id="d0005-599">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="d0005-600">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="d0005-600">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="d0005-601">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="d0005-601">firewallProfileDomain</span></span>|[<span data-ttu-id="d0005-602">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d0005-602">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="d0005-603">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="d0005-603">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="d0005-604">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="d0005-604">firewallProfilePublic</span></span>|[<span data-ttu-id="d0005-605">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d0005-605">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="d0005-606">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="d0005-606">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="d0005-607">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="d0005-607">firewallProfilePrivate</span></span>|[<span data-ttu-id="d0005-608">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="d0005-608">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="d0005-609">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="d0005-609">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="d0005-610">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="d0005-610">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="d0005-611">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-611">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-612">O valor que indica o comportamento do Adobe Reader de criar processos filhos.</span><span class="sxs-lookup"><span data-stu-id="d0005-612">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="d0005-613">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-613">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-614">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="d0005-614">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="d0005-615">String collection</span><span class="sxs-lookup"><span data-stu-id="d0005-615">String collection</span></span>|<span data-ttu-id="d0005-616">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="d0005-616">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="d0005-617">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-617">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="d0005-618">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d0005-618">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0005-619">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="d0005-619">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="d0005-620">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-620">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-621">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="d0005-621">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="d0005-622">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-623">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="d0005-623">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="d0005-624">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-625">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="d0005-625">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="d0005-626">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-626">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-627">O valor que indica o comportamento dos aplicativos de comunicação do Office, incluindo o Microsoft Outlook, da criação de processos filhos.</span><span class="sxs-lookup"><span data-stu-id="d0005-627">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="d0005-628">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-628">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-629">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="d0005-629">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="d0005-630">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d0005-630">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0005-631">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="d0005-631">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="d0005-632">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-632">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-633">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="d0005-633">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="d0005-634">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-634">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-635">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="d0005-635">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="d0005-636">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-636">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-637">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="d0005-637">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="d0005-638">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d0005-638">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0005-639">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="d0005-639">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="d0005-640">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-640">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-641">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="d0005-641">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="d0005-642">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-642">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-643">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="d0005-643">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="d0005-644">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-644">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-645">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="d0005-645">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="d0005-646">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d0005-646">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0005-647">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="d0005-647">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="d0005-648">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-648">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-649">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="d0005-649">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="d0005-650">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-651">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="d0005-651">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="d0005-652">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-653">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="d0005-653">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="d0005-654">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d0005-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0005-655">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="d0005-655">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="d0005-656">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-657">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="d0005-657">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="d0005-658">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-659">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="d0005-659">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="d0005-660">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-661">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="d0005-661">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="d0005-662">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d0005-662">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0005-663">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="d0005-663">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="d0005-664">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-664">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-665">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="d0005-665">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="d0005-666">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-667">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="d0005-667">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="d0005-668">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-669">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="d0005-669">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="d0005-670">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-671">Valor que indica se a credencial que está sendo roubada do subsistema de autoridade de segurança local do Windows é permitida.</span><span class="sxs-lookup"><span data-stu-id="d0005-671">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="d0005-672">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-673">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="d0005-673">defenderProcessCreationType</span></span>|[<span data-ttu-id="d0005-674">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d0005-674">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0005-675">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="d0005-675">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="d0005-676">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-676">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-677">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="d0005-677">defenderProcessCreation</span></span>|[<span data-ttu-id="d0005-678">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-679">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="d0005-679">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="d0005-680">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-681">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="d0005-681">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="d0005-682">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d0005-682">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0005-683">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="d0005-683">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="d0005-684">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-684">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-685">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="d0005-685">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="d0005-686">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-687">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="d0005-687">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="d0005-688">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-689">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="d0005-689">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="d0005-690">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d0005-690">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0005-691">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="d0005-691">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="d0005-692">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-692">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-693">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="d0005-693">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="d0005-694">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-694">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-695">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="d0005-695">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="d0005-696">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-696">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-697">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="d0005-697">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="d0005-698">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="d0005-698">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="d0005-699">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="d0005-699">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="d0005-700">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-700">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-701">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="d0005-701">defenderEmailContentExecution</span></span>|[<span data-ttu-id="d0005-702">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-702">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-703">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="d0005-703">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="d0005-704">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-704">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-705">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-705">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="d0005-706">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-706">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-707">O valor que indica o uso da proteção avançada contra o Ransomeware.</span><span class="sxs-lookup"><span data-stu-id="d0005-707">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="d0005-708">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-708">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-709">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="d0005-709">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="d0005-710">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-710">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="d0005-711">Valor que indica o comportamento das pastas protegidas.</span><span class="sxs-lookup"><span data-stu-id="d0005-711">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="d0005-712">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="d0005-712">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="d0005-713">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="d0005-713">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="d0005-714">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0005-714">String collection</span></span>|<span data-ttu-id="d0005-715">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="d0005-715">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="d0005-716">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="d0005-716">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="d0005-717">String collection</span><span class="sxs-lookup"><span data-stu-id="d0005-717">String collection</span></span>|<span data-ttu-id="d0005-718">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="d0005-718">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="d0005-719">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-719">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="d0005-720">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="d0005-720">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="d0005-721">Valor que indica o comportamento de NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="d0005-721">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="d0005-722">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="d0005-722">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="d0005-723">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="d0005-723">defenderExploitProtectionXml</span></span>|<span data-ttu-id="d0005-724">Binária</span><span class="sxs-lookup"><span data-stu-id="d0005-724">Binary</span></span>|<span data-ttu-id="d0005-725">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="d0005-725">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="d0005-726">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="d0005-726">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="d0005-727">String</span><span class="sxs-lookup"><span data-stu-id="d0005-727">String</span></span>|<span data-ttu-id="d0005-728">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="d0005-728">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="d0005-729">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="d0005-729">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="d0005-730">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-730">Boolean</span></span>|<span data-ttu-id="d0005-731">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="d0005-731">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="d0005-732">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="d0005-732">appLockerApplicationControl</span></span>|[<span data-ttu-id="d0005-733">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="d0005-733">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="d0005-734">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="d0005-734">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="d0005-735">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="d0005-735">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="d0005-736">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="d0005-736">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="d0005-737">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="d0005-737">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="d0005-738">Ative o Credential Guard quando o nível de segurança da plataforma com segurança baseada em inicialização e virtualização segura estiverem habilitados.</span><span class="sxs-lookup"><span data-stu-id="d0005-738">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="d0005-739">Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="d0005-739">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="d0005-740">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="d0005-740">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="d0005-741">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-741">Boolean</span></span>|<span data-ttu-id="d0005-742">Ativa a segurança baseada em virtualização (VBS).</span><span class="sxs-lookup"><span data-stu-id="d0005-742">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="d0005-743">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="d0005-743">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="d0005-744">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-744">Boolean</span></span>|<span data-ttu-id="d0005-745">Essa propriedade será substituída em maio de 2019 e será substituída pela propriedade DeviceGuardSecureBootWithDMA.</span><span class="sxs-lookup"><span data-stu-id="d0005-745">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="d0005-746">Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="d0005-746">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="d0005-747">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="d0005-747">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="d0005-748">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="d0005-748">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="d0005-749">Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="d0005-749">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="d0005-750">Os valores possíveis são: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="d0005-750">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="d0005-751">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="d0005-751">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="d0005-752">habilitação</span><span class="sxs-lookup"><span data-stu-id="d0005-752">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="d0005-753">Permite que o administrador de ti configure o lançamento do System Guard.</span><span class="sxs-lookup"><span data-stu-id="d0005-753">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="d0005-754">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="d0005-754">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="d0005-755">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="d0005-755">smartScreenEnableInShell</span></span>|<span data-ttu-id="d0005-756">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-756">Boolean</span></span>|<span data-ttu-id="d0005-757">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="d0005-757">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="d0005-758">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="d0005-758">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="d0005-759">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-759">Boolean</span></span>|<span data-ttu-id="d0005-760">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="d0005-760">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="d0005-761">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="d0005-761">applicationGuardEnabled</span></span>|<span data-ttu-id="d0005-762">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-762">Boolean</span></span>|<span data-ttu-id="d0005-763">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="d0005-763">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="d0005-764">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="d0005-764">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="d0005-765">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="d0005-765">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="d0005-766">Habilitar o Windows Defender Application Guard para novas versões do Windows.</span><span class="sxs-lookup"><span data-stu-id="d0005-766">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="d0005-767">Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="d0005-767">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="d0005-768">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="d0005-768">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="d0005-769">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="d0005-769">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="d0005-770">Bloquear a área de transferência para transferir o arquivo de imagem, o arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="d0005-770">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="d0005-771">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="d0005-771">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="d0005-772">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="d0005-772">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="d0005-773">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-773">Boolean</span></span>|<span data-ttu-id="d0005-774">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="d0005-774">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="d0005-775">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="d0005-775">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="d0005-776">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-776">Boolean</span></span>|<span data-ttu-id="d0005-777">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="d0005-777">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="d0005-778">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="d0005-778">applicationGuardForceAuditing</span></span>|<span data-ttu-id="d0005-779">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-779">Boolean</span></span>|<span data-ttu-id="d0005-780">A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)</span><span class="sxs-lookup"><span data-stu-id="d0005-780">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="d0005-781">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="d0005-781">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="d0005-782">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="d0005-782">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="d0005-783">Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="d0005-783">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="d0005-784">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="d0005-784">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="d0005-785">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="d0005-785">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="d0005-786">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-786">Boolean</span></span>|<span data-ttu-id="d0005-787">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="d0005-787">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="d0005-788">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="d0005-788">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="d0005-789">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-789">Boolean</span></span>|<span data-ttu-id="d0005-790">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="d0005-790">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="d0005-791">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="d0005-791">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="d0005-792">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-792">Boolean</span></span>|<span data-ttu-id="d0005-793">Permitir a impressão em impressoras locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="d0005-793">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="d0005-794">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="d0005-794">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="d0005-795">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-795">Boolean</span></span>|<span data-ttu-id="d0005-796">Permitir a impressão em impressoras da rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="d0005-796">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="d0005-797">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="d0005-797">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="d0005-798">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-798">Boolean</span></span>|<span data-ttu-id="d0005-799">Permitir que o Application Guard use virtual GPU</span><span class="sxs-lookup"><span data-stu-id="d0005-799">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="d0005-800">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="d0005-800">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="d0005-801">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-801">Boolean</span></span>|<span data-ttu-id="d0005-802">Permitir que os usuários baixem arquivos da borda no contêiner do Application Guard e salve-os no sistema de arquivos host</span><span class="sxs-lookup"><span data-stu-id="d0005-802">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="d0005-803">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="d0005-803">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="d0005-804">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-804">Boolean</span></span>|<span data-ttu-id="d0005-805">Permite que o administrador permita que os usuários padrão habilitem o encrpytion durante o ingresso no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d0005-805">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="d0005-806">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="d0005-806">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="d0005-807">Booliano</span><span class="sxs-lookup"><span data-stu-id="d0005-807">Boolean</span></span>|<span data-ttu-id="d0005-808">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="d0005-808">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="d0005-809">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="d0005-809">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="d0005-810">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0005-810">Boolean</span></span>|<span data-ttu-id="d0005-811">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d0005-811">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="d0005-812">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="d0005-812">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="d0005-813">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="d0005-813">bitLockerEncryptDevice</span></span>|<span data-ttu-id="d0005-814">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0005-814">Boolean</span></span>|<span data-ttu-id="d0005-815">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d0005-815">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="d0005-816">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d0005-816">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="d0005-817">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d0005-817">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="d0005-818">Política de unidade de sistema BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d0005-818">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="d0005-819">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d0005-819">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="d0005-820">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d0005-820">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="d0005-821">Política de unidade fixa do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d0005-821">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="d0005-822">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d0005-822">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="d0005-823">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="d0005-823">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="d0005-824">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d0005-824">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="d0005-825">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0005-825">Response</span></span>
<span data-ttu-id="d0005-826">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d0005-826">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0005-827">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d0005-827">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0005-828">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d0005-828">Request</span></span>
<span data-ttu-id="d0005-829">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d0005-829">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 28958

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
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
  "dmaGuardDeviceEnumerationPolicy": "blockAll",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "Display Name value",
      "description": "Description value",
      "packageFamilyName": "Package Family Name value",
      "filePath": "File Path value",
      "serviceName": "Service Name value",
      "protocol": 8,
      "localPortRanges": [
        "Local Port Ranges value"
      ],
      "remotePortRanges": [
        "Remote Port Ranges value"
      ],
      "localAddressRanges": [
        "Local Address Ranges value"
      ],
      "remoteAddressRanges": [
        "Remote Address Ranges value"
      ],
      "profileTypes": "domain",
      "action": "blocked",
      "trafficDirection": "out",
      "interfaceTypes": "remoteAccess",
      "edgeTraversal": "blocked",
      "localUserAuthorizations": "Local User Authorizations value"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDenyLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
  "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
  "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
  "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
  "localSecurityOptionsMachineInactivityLimit": 10,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
  "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
  "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
  "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
  "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
  "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
  "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
  "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
  "windowsDefenderTamperProtection": "enable",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "enable",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
  "defenderOfficeAppsLaunchChildProcessType": "block",
  "defenderOfficeAppsLaunchChildProcess": "enable",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
  "defenderOfficeMacroCodeAllowWin32Imports": "enable",
  "defenderScriptObfuscatedMacroCodeType": "block",
  "defenderScriptObfuscatedMacroCode": "enable",
  "defenderScriptDownloadedPayloadExecutionType": "block",
  "defenderScriptDownloadedPayloadExecution": "enable",
  "defenderPreventCredentialStealingType": "enable",
  "defenderProcessCreationType": "block",
  "defenderProcessCreation": "enable",
  "defenderUntrustedUSBProcessType": "block",
  "defenderUntrustedUSBProcess": "enable",
  "defenderUntrustedExecutableType": "block",
  "defenderUntrustedExecutable": "enable",
  "defenderEmailContentExecutionType": "block",
  "defenderEmailContentExecution": "enable",
  "defenderAdvancedRansomewareProtectionType": "enable",
  "defenderGuardMyFoldersType": "enable",
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderNetworkProtectionType": "enable",
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "withoutDMA",
  "deviceGuardLaunchSystemGuard": "enabled",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "enabledForEdge",
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "required",
    "startupAuthenticationTpmPinUsage": "required",
    "startupAuthenticationTpmKeyUsage": "required",
    "startupAuthenticationTpmPinAndKeyUsage": "required",
    "minimumPinLength": 0,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "Preboot Recovery Message value",
    "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```

### <a name="response"></a><span data-ttu-id="d0005-830">Resposta</span><span class="sxs-lookup"><span data-stu-id="d0005-830">Response</span></span>
<span data-ttu-id="d0005-p206">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d0005-p206">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 29130

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
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
  "dmaGuardDeviceEnumerationPolicy": "blockAll",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "Display Name value",
      "description": "Description value",
      "packageFamilyName": "Package Family Name value",
      "filePath": "File Path value",
      "serviceName": "Service Name value",
      "protocol": 8,
      "localPortRanges": [
        "Local Port Ranges value"
      ],
      "remotePortRanges": [
        "Remote Port Ranges value"
      ],
      "localAddressRanges": [
        "Local Address Ranges value"
      ],
      "remoteAddressRanges": [
        "Remote Address Ranges value"
      ],
      "profileTypes": "domain",
      "action": "blocked",
      "trafficDirection": "out",
      "interfaceTypes": "remoteAccess",
      "edgeTraversal": "blocked",
      "localUserAuthorizations": "Local User Authorizations value"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDenyLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "userRightsRegisterProcessAsService": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "blocked",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "Name value",
        "description": "Description value",
        "securityIdentifier": "Security Identifier value"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "automatic",
  "xboxServicesLiveAuthManagerServiceStartupMode": "automatic",
  "xboxServicesLiveGameSaveServiceStartupMode": "automatic",
  "xboxServicesLiveNetworkingServiceStartupMode": "automatic",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "Local Security Options Guest Account Name value",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "administrators",
  "localSecurityOptionsMachineInactivityLimit": 10,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 3,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "Local Security Options Log On Message Title value",
  "localSecurityOptionsLogOnMessageText": "Local Security Options Log On Message Text value",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "Local Security Options Allow Remote Calls To Security Accounts Manager value",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "requireNtmlV2SessionSecurity",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "requireNtmlV2SessionSecurity",
  "lanManagerAuthenticationLevel": "lmNtlmAndNtlmV2",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "elevateWithoutPrompting",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "automaticallyDenyElevationRequests",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "userDisplayNameDomainUser",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "administrators",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "noAction",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "Defender Security Center Organization Display Name value",
  "defenderSecurityCenterHelpEmail": "Defender Security Center Help Email value",
  "defenderSecurityCenterHelpPhone": "Defender Security Center Help Phone value",
  "defenderSecurityCenterHelpURL": "Defender Security Center Help URL value",
  "defenderSecurityCenterNotificationsFromApp": "blockNoncriticalNotifications",
  "defenderSecurityCenterITContactDisplay": "displayInAppAndInNotifications",
  "windowsDefenderTamperProtection": "enable",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "enable",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "enable",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "block",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "enable",
  "defenderOfficeAppsLaunchChildProcessType": "block",
  "defenderOfficeAppsLaunchChildProcess": "enable",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "block",
  "defenderOfficeMacroCodeAllowWin32Imports": "enable",
  "defenderScriptObfuscatedMacroCodeType": "block",
  "defenderScriptObfuscatedMacroCode": "enable",
  "defenderScriptDownloadedPayloadExecutionType": "block",
  "defenderScriptDownloadedPayloadExecution": "enable",
  "defenderPreventCredentialStealingType": "enable",
  "defenderProcessCreationType": "block",
  "defenderProcessCreation": "enable",
  "defenderUntrustedUSBProcessType": "block",
  "defenderUntrustedUSBProcess": "enable",
  "defenderUntrustedExecutableType": "block",
  "defenderUntrustedExecutable": "enable",
  "defenderEmailContentExecutionType": "block",
  "defenderEmailContentExecution": "enable",
  "defenderAdvancedRansomewareProtectionType": "enable",
  "defenderGuardMyFoldersType": "enable",
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderNetworkProtectionType": "enable",
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "enableWithUEFILock",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "withoutDMA",
  "deviceGuardLaunchSystemGuard": "enabled",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "enabledForEdge",
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "required",
    "startupAuthenticationTpmPinUsage": "required",
    "startupAuthenticationTpmKeyUsage": "required",
    "startupAuthenticationTpmPinAndKeyUsage": "required",
    "minimumPinLength": 0,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "Preboot Recovery Message value",
    "prebootRecoveryUrl": "https://example.com/prebootRecoveryUrl/"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "required",
      "recoveryKeyUsage": "required",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "passwordOnly",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```





