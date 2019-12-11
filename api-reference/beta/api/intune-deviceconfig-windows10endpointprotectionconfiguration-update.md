---
title: Atualizar windows10EndpointProtectionConfiguration
description: Atualizar as propriedades de um objeto windows10EndpointProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c0e0d1f9cae4c31586fdff7a3749da886dde16a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947481"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="500ec-103">Atualizar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="500ec-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="500ec-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="500ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="500ec-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="500ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="500ec-106">Atualizar as propriedades de um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="500ec-106">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="500ec-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="500ec-107">Prerequisites</span></span>
<span data-ttu-id="500ec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="500ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="500ec-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="500ec-110">Permission type</span></span>|<span data-ttu-id="500ec-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="500ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="500ec-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="500ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="500ec-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="500ec-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="500ec-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="500ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="500ec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="500ec-115">Not supported.</span></span>|
|<span data-ttu-id="500ec-116">Application</span><span class="sxs-lookup"><span data-stu-id="500ec-116">Application</span></span>|<span data-ttu-id="500ec-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="500ec-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="500ec-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="500ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="500ec-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="500ec-119">Request headers</span></span>
|<span data-ttu-id="500ec-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="500ec-120">Header</span></span>|<span data-ttu-id="500ec-121">Valor</span><span class="sxs-lookup"><span data-stu-id="500ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="500ec-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="500ec-122">Authorization</span></span>|<span data-ttu-id="500ec-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="500ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="500ec-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="500ec-124">Accept</span></span>|<span data-ttu-id="500ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="500ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="500ec-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="500ec-126">Request body</span></span>
<span data-ttu-id="500ec-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="500ec-127">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="500ec-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="500ec-128">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="500ec-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="500ec-129">Property</span></span>|<span data-ttu-id="500ec-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="500ec-130">Type</span></span>|<span data-ttu-id="500ec-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="500ec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="500ec-132">id</span><span class="sxs-lookup"><span data-stu-id="500ec-132">id</span></span>|<span data-ttu-id="500ec-133">String</span><span class="sxs-lookup"><span data-stu-id="500ec-133">String</span></span>|<span data-ttu-id="500ec-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="500ec-134">Key of the entity.</span></span> <span data-ttu-id="500ec-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="500ec-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="500ec-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="500ec-136">lastModifiedDateTime</span></span>|<span data-ttu-id="500ec-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="500ec-137">DateTimeOffset</span></span>|<span data-ttu-id="500ec-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="500ec-138">DateTime the object was last modified.</span></span> <span data-ttu-id="500ec-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="500ec-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="500ec-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="500ec-140">roleScopeTagIds</span></span>|<span data-ttu-id="500ec-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-141">String collection</span></span>|<span data-ttu-id="500ec-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="500ec-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="500ec-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="500ec-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="500ec-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="500ec-144">supportsScopeTags</span></span>|<span data-ttu-id="500ec-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-145">Boolean</span></span>|<span data-ttu-id="500ec-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="500ec-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="500ec-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="500ec-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="500ec-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="500ec-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="500ec-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="500ec-149">This property is read-only.</span></span> <span data-ttu-id="500ec-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="500ec-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="500ec-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="500ec-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="500ec-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="500ec-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="500ec-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="500ec-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="500ec-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="500ec-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="500ec-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="500ec-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="500ec-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="500ec-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="500ec-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="500ec-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="500ec-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="500ec-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="500ec-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="500ec-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="500ec-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="500ec-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="500ec-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="500ec-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="500ec-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="500ec-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="500ec-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="500ec-163">createdDateTime</span></span>|<span data-ttu-id="500ec-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="500ec-164">DateTimeOffset</span></span>|<span data-ttu-id="500ec-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="500ec-165">DateTime the object was created.</span></span> <span data-ttu-id="500ec-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="500ec-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="500ec-167">description</span><span class="sxs-lookup"><span data-stu-id="500ec-167">description</span></span>|<span data-ttu-id="500ec-168">String</span><span class="sxs-lookup"><span data-stu-id="500ec-168">String</span></span>|<span data-ttu-id="500ec-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="500ec-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="500ec-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="500ec-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="500ec-171">displayName</span><span class="sxs-lookup"><span data-stu-id="500ec-171">displayName</span></span>|<span data-ttu-id="500ec-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-172">String</span></span>|<span data-ttu-id="500ec-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="500ec-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="500ec-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="500ec-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="500ec-175">versão</span><span class="sxs-lookup"><span data-stu-id="500ec-175">version</span></span>|<span data-ttu-id="500ec-176">Int32</span><span class="sxs-lookup"><span data-stu-id="500ec-176">Int32</span></span>|<span data-ttu-id="500ec-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="500ec-177">Version of the device configuration.</span></span> <span data-ttu-id="500ec-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="500ec-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="500ec-179">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="500ec-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="500ec-180">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="500ec-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="500ec-181">Essa política destina-se a fornecer segurança adicional contra dispositivos compatíveis com DMA externo.</span><span class="sxs-lookup"><span data-stu-id="500ec-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="500ec-182">Permite mais controle sobre a enumeração de dispositivos compatíveis com DMA externo incompatíveis com o remapeamento de DMA/isolamento de memória do dispositivo e área restrita.</span><span class="sxs-lookup"><span data-stu-id="500ec-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="500ec-183">Essa política só entra em vigor quando a proteção DMA de kernel é suportada e habilitada pelo firmware do sistema.</span><span class="sxs-lookup"><span data-stu-id="500ec-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="500ec-184">A proteção DMA de kernel é um recurso de plataforma que não pode ser controlado via política ou pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="500ec-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="500ec-185">É preciso ter suporte do sistema no momento da fabricação.</span><span class="sxs-lookup"><span data-stu-id="500ec-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="500ec-186">Para verificar se o sistema suporta a proteção DMA de kernel, verifique o campo proteção DMA de kernel na página Resumo de MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="500ec-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="500ec-187">Os valores possíveis são: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="500ec-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="500ec-188">firewallRules</span><span class="sxs-lookup"><span data-stu-id="500ec-188">firewallRules</span></span>|<span data-ttu-id="500ec-189">coleção [windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="500ec-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="500ec-190">Define as configurações da regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="500ec-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="500ec-191">Essa coleção pode conter um máximo de 150 elementos.</span><span class="sxs-lookup"><span data-stu-id="500ec-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="500ec-192">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="500ec-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="500ec-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-194">Esse direito de usuário é usado pelo Gerenciador de credenciais durante o backup/restauração.</span><span class="sxs-lookup"><span data-stu-id="500ec-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="500ec-195">As credenciais salvas dos usuários podem ser comprometidas se esse privilégio for dado a outras entidades.</span><span class="sxs-lookup"><span data-stu-id="500ec-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="500ec-196">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="500ec-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="500ec-197">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="500ec-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="500ec-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-199">Esse direito de usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="500ec-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="500ec-200">O estado permitido é suportado.</span><span class="sxs-lookup"><span data-stu-id="500ec-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="500ec-201">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="500ec-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="500ec-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-203">Esse direito de usuário determina quais usuários e grupos são bloqueados para se conectarem ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="500ec-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="500ec-204">Há suporte para o bloco de estado.</span><span class="sxs-lookup"><span data-stu-id="500ec-204">State Block is supported.</span></span>|
|<span data-ttu-id="500ec-205">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="500ec-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="500ec-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-207">Esse direito de usuário permite que um processo represente qualquer usuário sem autenticação.</span><span class="sxs-lookup"><span data-stu-id="500ec-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="500ec-208">Portanto, o processo pode ter acesso aos mesmos recursos locais que esse usuário.</span><span class="sxs-lookup"><span data-stu-id="500ec-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="500ec-209">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="500ec-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="500ec-210">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="500ec-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="500ec-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-212">Esse direito de usuário determina quais usuários podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="500ec-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="500ec-213">Estados não configurados, permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="500ec-213">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="500ec-214">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="500ec-214">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="500ec-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-216">Esse direito de usuário determina quais usuários não podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="500ec-216">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="500ec-217">Estados não configurados, bloqueados são suportados</span><span class="sxs-lookup"><span data-stu-id="500ec-217">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="500ec-218">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="500ec-218">userRightsBackupData</span></span>|[<span data-ttu-id="500ec-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-220">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao fazer backup de arquivos e diretórios.</span><span class="sxs-lookup"><span data-stu-id="500ec-220">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="500ec-221">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="500ec-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="500ec-222">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="500ec-222">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="500ec-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-224">Este direito de usuário determina quais usuários e grupos podem alterar a hora e a data no relógio interno do computador.</span><span class="sxs-lookup"><span data-stu-id="500ec-224">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="500ec-225">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="500ec-225">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="500ec-226">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="500ec-226">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="500ec-227">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-227">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-228">Configuração de segurança que determina se os usuários podem criar objetos globais que estão disponíveis para todas as sessões.</span><span class="sxs-lookup"><span data-stu-id="500ec-228">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="500ec-229">Os usuários que podem criar objetos globais podem afetar processos executados em sessões de outros usuários, o que pode levar a falhas de aplicativos ou corrupção de dados.</span><span class="sxs-lookup"><span data-stu-id="500ec-229">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="500ec-230">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="500ec-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="500ec-231">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="500ec-231">userRightsCreatePageFile</span></span>|[<span data-ttu-id="500ec-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-233">Esse direito de usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de paginação.</span><span class="sxs-lookup"><span data-stu-id="500ec-233">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="500ec-234">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="500ec-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="500ec-235">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="500ec-235">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="500ec-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-237">Este direito de usuário determina quais contas podem ser usadas por processos para criar um objeto de diretório usando o Gerenciador de objetos.</span><span class="sxs-lookup"><span data-stu-id="500ec-237">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="500ec-238">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="500ec-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="500ec-239">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="500ec-239">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="500ec-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-241">Esse direito de usuário determina se o usuário pode criar um link simbólico do computador no qual está conectado.</span><span class="sxs-lookup"><span data-stu-id="500ec-241">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="500ec-242">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="500ec-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="500ec-243">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="500ec-243">userRightsCreateToken</span></span>|[<span data-ttu-id="500ec-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-245">Esse direito de usuário determina quais usuários/grupos podem ser usados por processos para criar um token que pode ser usado para obter acesso a qualquer recurso local quando o processo usa uma API interna para criar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="500ec-245">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="500ec-246">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="500ec-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="500ec-247">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="500ec-247">userRightsDebugPrograms</span></span>|[<span data-ttu-id="500ec-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-249">Esse direito de usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel.</span><span class="sxs-lookup"><span data-stu-id="500ec-249">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="500ec-250">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="500ec-250">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="500ec-251">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="500ec-251">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="500ec-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-253">Este direito de usuário determina quais usuários e grupos estão proibidos de fazer logon como um cliente de serviços de área de trabalho remota.</span><span class="sxs-lookup"><span data-stu-id="500ec-253">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="500ec-254">Há suporte apenas para os Estados não configurados e bloqueados</span><span class="sxs-lookup"><span data-stu-id="500ec-254">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="500ec-255">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="500ec-255">userRightsDelegation</span></span>|[<span data-ttu-id="500ec-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-257">Este direito de usuário determina quais usuários podem definir a configuração confiável para delegação em um objeto de usuário ou computador.</span><span class="sxs-lookup"><span data-stu-id="500ec-257">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="500ec-258">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-258">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-259">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="500ec-259">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="500ec-260">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-260">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-261">Este direito de usuário determina quais contas podem ser usadas por um processo para adicionar entradas ao log de segurança.</span><span class="sxs-lookup"><span data-stu-id="500ec-261">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="500ec-262">O log de segurança é usado para rastrear o acesso de sistema não autorizado.</span><span class="sxs-lookup"><span data-stu-id="500ec-262">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="500ec-263">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-263">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-264">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="500ec-264">userRightsImpersonateClient</span></span>|[<span data-ttu-id="500ec-265">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-265">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-266">A atribuição desse direito de usuário a um usuário permite que programas executados em nome desse usuário representem um cliente.</span><span class="sxs-lookup"><span data-stu-id="500ec-266">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="500ec-267">A exigência desse direito de usuário para esse tipo de representação impede que um usuário não autorizado convença um cliente a se conectar a um serviço que ele criou e, em seguida, representando esse cliente, o que pode elevar as permissões do usuário não autorizado para níveis administrativos ou de sistema.</span><span class="sxs-lookup"><span data-stu-id="500ec-267">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="500ec-268">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-269">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="500ec-269">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="500ec-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-271">Este direito de usuário determina quais contas podem usar um processo com acesso de propriedade de gravação a outro processo para aumentar a prioridade de execução atribuída ao outro processo.</span><span class="sxs-lookup"><span data-stu-id="500ec-271">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="500ec-272">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-273">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="500ec-273">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="500ec-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-275">Esse direito de usuário determina quais usuários podem carregar e descarregar dinamicamente drivers de dispositivo ou outro código no modo kernel.</span><span class="sxs-lookup"><span data-stu-id="500ec-275">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="500ec-276">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-277">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="500ec-277">userRightsLockMemory</span></span>|[<span data-ttu-id="500ec-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-279">Esse direito de usuário determina quais contas podem usar um processo para manter os dados na memória física, o que impede que o sistema pagine os dados para a memória virtual em disco.</span><span class="sxs-lookup"><span data-stu-id="500ec-279">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="500ec-280">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-281">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="500ec-281">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="500ec-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-283">Esse direito de usuário determina quais usuários podem especificar opções de auditoria de acesso a objetos para recursos individuais, como arquivos, objetos do Active Directory e chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="500ec-283">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="500ec-284">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-285">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="500ec-285">userRightsManageVolumes</span></span>|[<span data-ttu-id="500ec-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-287">Esse direito de usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como a desfragmentação remota.</span><span class="sxs-lookup"><span data-stu-id="500ec-287">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="500ec-288">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-289">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="500ec-289">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="500ec-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-291">Esse direito de usuário determina quem pode modificar os valores de ambiente de firmware.</span><span class="sxs-lookup"><span data-stu-id="500ec-291">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="500ec-292">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-293">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="500ec-293">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="500ec-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-295">Este direito de usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves de registro ou processos pertencentes a outros usuários.</span><span class="sxs-lookup"><span data-stu-id="500ec-295">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="500ec-296">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-297">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="500ec-297">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="500ec-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-299">Esse direito de usuário determina quais usuários podem usar ferramentas de monitoramento de desempenho para monitorar o desempenho de processos do sistema.</span><span class="sxs-lookup"><span data-stu-id="500ec-299">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="500ec-300">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-300">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-301">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="500ec-301">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="500ec-302">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-302">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-303">Esse direito de usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede.</span><span class="sxs-lookup"><span data-stu-id="500ec-303">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="500ec-304">O mau uso desse direito de usuário pode resultar em uma negação de serviço.</span><span class="sxs-lookup"><span data-stu-id="500ec-304">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="500ec-305">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-306">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="500ec-306">userRightsRestoreData</span></span>|[<span data-ttu-id="500ec-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-308">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao restaurar backups de arquivos e diretórios e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto.</span><span class="sxs-lookup"><span data-stu-id="500ec-308">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="500ec-309">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-310">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="500ec-310">userRightsTakeOwnership</span></span>|[<span data-ttu-id="500ec-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="500ec-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="500ec-312">Esse direito de usuário determina quais usuários podem assumir a propriedade de qualquer objeto protegível no sistema, incluindo objetos do Active Directory, arquivos e pastas, impressoras, chaves do registro, processos e threads.</span><span class="sxs-lookup"><span data-stu-id="500ec-312">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="500ec-313">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-313">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="500ec-314">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="500ec-314">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="500ec-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-315">Boolean</span></span>|<span data-ttu-id="500ec-316">Essa configuração determina se o salvamento de jogos do Xbox está habilitado (1) ou desabilitado (0).</span><span class="sxs-lookup"><span data-stu-id="500ec-316">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="500ec-317">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="500ec-317">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="500ec-318">instarttype</span><span class="sxs-lookup"><span data-stu-id="500ec-318">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="500ec-319">Esta configuração determina se o tipo de início do serviço de gerenciamento de acessórios é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="500ec-319">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="500ec-320">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="500ec-320">Default: Manual.</span></span> <span data-ttu-id="500ec-321">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="500ec-321">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="500ec-322">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="500ec-322">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="500ec-323">instarttype</span><span class="sxs-lookup"><span data-stu-id="500ec-323">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="500ec-324">Essa configuração determina se o tipo de início do serviço do Live Authentication Manager é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="500ec-324">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="500ec-325">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="500ec-325">Default: Manual.</span></span> <span data-ttu-id="500ec-326">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="500ec-326">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="500ec-327">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="500ec-327">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="500ec-328">instarttype</span><span class="sxs-lookup"><span data-stu-id="500ec-328">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="500ec-329">Essa configuração determina se o tipo de início do serviço de salvamento do Live Game é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="500ec-329">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="500ec-330">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="500ec-330">Default: Manual.</span></span> <span data-ttu-id="500ec-331">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="500ec-331">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="500ec-332">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="500ec-332">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="500ec-333">instarttype</span><span class="sxs-lookup"><span data-stu-id="500ec-333">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="500ec-334">Esta configuração determina se o tipo de início do serviço de rede é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="500ec-334">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="500ec-335">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="500ec-335">Default: Manual.</span></span> <span data-ttu-id="500ec-336">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="500ec-336">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="500ec-337">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="500ec-337">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="500ec-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-338">Boolean</span></span>|<span data-ttu-id="500ec-339">Impedir que os usuários adicionem novas contas da Microsoft a este computador.</span><span class="sxs-lookup"><span data-stu-id="500ec-339">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="500ec-340">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="500ec-340">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="500ec-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-341">Boolean</span></span>|<span data-ttu-id="500ec-342">Habilitar contas locais que não estão protegidas por senha para fazer logon de locais diferentes do dispositivo físico. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="500ec-342">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="500ec-343">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="500ec-343">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="500ec-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-344">Boolean</span></span>|<span data-ttu-id="500ec-345">Determina se a conta de administrador local está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="500ec-345">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="500ec-346">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="500ec-346">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="500ec-347">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-347">String</span></span>|<span data-ttu-id="500ec-348">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "administrador".</span><span class="sxs-lookup"><span data-stu-id="500ec-348">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="500ec-349">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="500ec-349">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="500ec-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-350">Boolean</span></span>|<span data-ttu-id="500ec-351">Determina se a conta de convidado está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="500ec-351">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="500ec-352">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="500ec-352">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="500ec-353">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-353">String</span></span>|<span data-ttu-id="500ec-354">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "convidado".</span><span class="sxs-lookup"><span data-stu-id="500ec-354">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="500ec-355">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="500ec-355">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="500ec-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-356">Boolean</span></span>|<span data-ttu-id="500ec-357">Impedir que um computador portátil seja desencaixado sem ter que fazer logon.</span><span class="sxs-lookup"><span data-stu-id="500ec-357">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="500ec-358">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="500ec-358">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="500ec-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-359">Boolean</span></span>|<span data-ttu-id="500ec-360">Restringir a instalação dos drivers de impressora como parte da conexão a uma impressora compartilhada somente para administradores.</span><span class="sxs-lookup"><span data-stu-id="500ec-360">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="500ec-361">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="500ec-361">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="500ec-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-362">Boolean</span></span>|<span data-ttu-id="500ec-363">Habilitar essa configuração permite que somente o usuário conectado interativamente acesse a mídia de CD-ROM.</span><span class="sxs-lookup"><span data-stu-id="500ec-363">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="500ec-364">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="500ec-364">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="500ec-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="500ec-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="500ec-366">Defina quem tem permissão para formatar e ejetar a mídia NTFS removível.</span><span class="sxs-lookup"><span data-stu-id="500ec-366">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="500ec-367">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="500ec-367">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="500ec-368">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="500ec-368">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="500ec-369">Int32</span><span class="sxs-lookup"><span data-stu-id="500ec-369">Int32</span></span>|<span data-ttu-id="500ec-370">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="500ec-370">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="500ec-371">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="500ec-371">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="500ec-372">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="500ec-372">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="500ec-373">Int32</span><span class="sxs-lookup"><span data-stu-id="500ec-373">Int32</span></span>|<span data-ttu-id="500ec-374">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="500ec-374">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="500ec-375">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="500ec-375">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="500ec-376">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="500ec-376">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="500ec-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-377">Boolean</span></span>|<span data-ttu-id="500ec-378">Exigir CTRL + ALT + DEL para ser pressionada para que um usuário possa fazer logon.</span><span class="sxs-lookup"><span data-stu-id="500ec-378">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="500ec-379">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="500ec-379">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="500ec-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-380">Boolean</span></span>|<span data-ttu-id="500ec-381">Não exibe o nome de usuário da última pessoa que entrou neste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="500ec-381">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="500ec-382">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="500ec-382">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="500ec-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-383">Boolean</span></span>|<span data-ttu-id="500ec-384">Não exibe o nome de usuário da pessoa que está entrando neste dispositivo depois que as credenciais são inseridas e antes da área de trabalho do dispositivo ser exibida.</span><span class="sxs-lookup"><span data-stu-id="500ec-384">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="500ec-385">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="500ec-385">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="500ec-386">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-386">String</span></span>|<span data-ttu-id="500ec-387">Defina o título da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="500ec-387">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="500ec-388">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="500ec-388">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="500ec-389">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-389">String</span></span>|<span data-ttu-id="500ec-390">Definir o texto da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="500ec-390">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="500ec-391">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="500ec-391">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="500ec-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-392">Boolean</span></span>|<span data-ttu-id="500ec-393">Bloquear solicitações de autenticação PKU2U para este dispositivo para usar identidades online.</span><span class="sxs-lookup"><span data-stu-id="500ec-393">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="500ec-394">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="500ec-394">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="500ec-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-395">Boolean</span></span>|<span data-ttu-id="500ec-396">Boolean do auxiliar da interface do usuário para entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="500ec-396">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="500ec-397">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="500ec-397">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="500ec-398">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-398">String</span></span>|<span data-ttu-id="500ec-399">Edite a cadeia de caracteres de definição de descritor de segurança padrão para permitir ou impedir que usuários e grupos façam chamadas remotas para o SAM.</span><span class="sxs-lookup"><span data-stu-id="500ec-399">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="500ec-400">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="500ec-400">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="500ec-401">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="500ec-401">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="500ec-402">Essa configuração de segurança permite que um cliente exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="500ec-402">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="500ec-403">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="500ec-403">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="500ec-404">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="500ec-404">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="500ec-405">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="500ec-405">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="500ec-406">Essa configuração de segurança permite que um servidor exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="500ec-406">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="500ec-407">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="500ec-407">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="500ec-408">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="500ec-408">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="500ec-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="500ec-409">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="500ec-410">Essa configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede.</span><span class="sxs-lookup"><span data-stu-id="500ec-410">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="500ec-411">Os possíveis valores são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="500ec-411">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="500ec-412">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="500ec-412">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="500ec-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-413">Boolean</span></span>|<span data-ttu-id="500ec-414">Se for habilitada, o cliente SMB permitirá logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="500ec-414">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="500ec-415">Se não configurada, o cliente SMB rejeitará logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="500ec-415">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="500ec-416">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="500ec-416">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="500ec-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-417">Boolean</span></span>|<span data-ttu-id="500ec-418">Configuração de segurança que determina se o arquivo de paginação de memória virtual será limpo quando o sistema for desligado.</span><span class="sxs-lookup"><span data-stu-id="500ec-418">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="500ec-419">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="500ec-419">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="500ec-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-420">Boolean</span></span>|<span data-ttu-id="500ec-421">Configuração de segurança que determina se um computador pode ser desligado sem a necessidade de fazer logon no Windows.</span><span class="sxs-lookup"><span data-stu-id="500ec-421">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="500ec-422">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="500ec-422">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="500ec-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-423">Boolean</span></span>|<span data-ttu-id="500ec-424">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="500ec-424">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="500ec-425">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="500ec-425">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="500ec-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-426">Boolean</span></span>|<span data-ttu-id="500ec-427">Virtualizar falhas de gravação de arquivo e registro para locais por usuário</span><span class="sxs-lookup"><span data-stu-id="500ec-427">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="500ec-428">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="500ec-428">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="500ec-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-429">Boolean</span></span>|<span data-ttu-id="500ec-430">Impor a validação de caminho de certificação PKI para um determinado arquivo executável antes que seja permitido executar.</span><span class="sxs-lookup"><span data-stu-id="500ec-430">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="500ec-431">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="500ec-431">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="500ec-432">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="500ec-432">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="500ec-433">Definir o comportamento do prompt de elevação para administradores no modo de aprovação de administrador.</span><span class="sxs-lookup"><span data-stu-id="500ec-433">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="500ec-434">Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="500ec-434">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="500ec-435">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="500ec-435">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="500ec-436">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="500ec-436">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="500ec-437">Definir o comportamento do prompt de elevação para usuários padrão.</span><span class="sxs-lookup"><span data-stu-id="500ec-437">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="500ec-438">Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="500ec-438">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="500ec-439">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="500ec-439">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="500ec-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-440">Boolean</span></span>|<span data-ttu-id="500ec-441">Habilite todas as solicitações de elevação para ir para a área de trabalho do usuário interativo, e não para a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="500ec-441">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="500ec-442">As configurações de política de comportamento de prompt para administradores e usuários padrão são usadas.</span><span class="sxs-lookup"><span data-stu-id="500ec-442">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="500ec-443">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="500ec-443">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="500ec-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-444">Boolean</span></span>|<span data-ttu-id="500ec-445">Instalações de aplicativos que exigem privilégios elevados solicitarão credenciais de administrador. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="500ec-445">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="500ec-446">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="500ec-446">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="500ec-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-447">Boolean</span></span>|<span data-ttu-id="500ec-448">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="500ec-448">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="500ec-449">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="500ec-449">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="500ec-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-450">Boolean</span></span>|<span data-ttu-id="500ec-451">Define se a conta de administrador interna usa o modo de aprovação de administrador ou executa todos os aplicativos com privilégios de administrador completo. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="500ec-451">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="500ec-452">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="500ec-452">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="500ec-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-453">Boolean</span></span>|<span data-ttu-id="500ec-454">Definir se o modo de aprovação de administrador e todas as configurações de política de UAC estão habilitados, o padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="500ec-454">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="500ec-455">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="500ec-455">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="500ec-456">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="500ec-456">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="500ec-457">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="500ec-457">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="500ec-458">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-458">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="500ec-459">Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="500ec-459">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="500ec-460">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="500ec-460">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="500ec-461">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="500ec-461">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="500ec-462">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="500ec-462">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="500ec-463">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="500ec-463">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="500ec-464">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="500ec-464">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="500ec-465">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="500ec-465">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="500ec-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-466">Boolean</span></span>|<span data-ttu-id="500ec-467">Configuração de segurança que determina se o cliente SMB tentará negociar assinatura de pacote SMB.</span><span class="sxs-lookup"><span data-stu-id="500ec-467">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="500ec-468">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="500ec-468">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="500ec-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-469">Boolean</span></span>|<span data-ttu-id="500ec-470">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do cliente SMB.</span><span class="sxs-lookup"><span data-stu-id="500ec-470">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="500ec-471">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="500ec-471">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="500ec-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-472">Boolean</span></span>|<span data-ttu-id="500ec-473">Se essa configuração de segurança estiver habilitada, o redirecionador de bloco de mensagens de servidor (SMB) terá permissão para enviar senhas de texto não criptografado para servidores SMB não Microsoft que não ofereçam suporte à criptografia de senha durante a autenticação.</span><span class="sxs-lookup"><span data-stu-id="500ec-473">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="500ec-474">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="500ec-474">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="500ec-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-475">Boolean</span></span>|<span data-ttu-id="500ec-476">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do servidor SMB.</span><span class="sxs-lookup"><span data-stu-id="500ec-476">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="500ec-477">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="500ec-477">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="500ec-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-478">Boolean</span></span>|<span data-ttu-id="500ec-479">Configuração de segurança que determina se o servidor SMB negociará assinatura de pacote SMB com clientes que solicitarem.</span><span class="sxs-lookup"><span data-stu-id="500ec-479">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="500ec-480">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="500ec-480">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="500ec-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-481">Boolean</span></span>|<span data-ttu-id="500ec-482">Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e pipes para as configurações de pipes nomeados que podem ser acessados anonimamente e compartilhamentos que podem ser acessados anonimamente</span><span class="sxs-lookup"><span data-stu-id="500ec-482">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="500ec-483">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="500ec-483">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="500ec-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-484">Boolean</span></span>|<span data-ttu-id="500ec-485">Essa configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas com o computador.</span><span class="sxs-lookup"><span data-stu-id="500ec-485">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="500ec-486">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="500ec-486">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="500ec-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-487">Boolean</span></span>|<span data-ttu-id="500ec-488">Configuração de segurança que determina se os usuários anônimos devem executar determinadas atividades, como enumeração de nomes de contas de domínio e compartilhamentos de rede.</span><span class="sxs-lookup"><span data-stu-id="500ec-488">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="500ec-489">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="500ec-489">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="500ec-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-490">Boolean</span></span>|<span data-ttu-id="500ec-491">Essa configuração de segurança determina se, na próxima alteração de senha, o valor de hash do LM (LAN Manager) para a nova senha é armazenado.</span><span class="sxs-lookup"><span data-stu-id="500ec-491">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="500ec-492">Ele não é armazenado por padrão.</span><span class="sxs-lookup"><span data-stu-id="500ec-492">It’s not stored by default.</span></span>|
|<span data-ttu-id="500ec-493">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="500ec-493">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="500ec-494">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="500ec-494">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="500ec-495">Essa configuração de segurança determina o que acontece quando o cartão inteligente de um usuário conectado é removido do leitor de cartão inteligente.</span><span class="sxs-lookup"><span data-stu-id="500ec-495">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="500ec-496">Os valores possíveis são: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="500ec-496">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="500ec-497">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="500ec-497">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="500ec-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-498">Boolean</span></span>|<span data-ttu-id="500ec-499">Usado para desabilitar a exibição da área de proteção de aplicativo e navegador.</span><span class="sxs-lookup"><span data-stu-id="500ec-499">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="500ec-500">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="500ec-500">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="500ec-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-501">Boolean</span></span>|<span data-ttu-id="500ec-502">Usado para desabilitar a exibição da área de opções da família.</span><span class="sxs-lookup"><span data-stu-id="500ec-502">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="500ec-503">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="500ec-503">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="500ec-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-504">Boolean</span></span>|<span data-ttu-id="500ec-505">Usado para desabilitar a exibição da área de desempenho e integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="500ec-505">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="500ec-506">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="500ec-506">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="500ec-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-507">Boolean</span></span>|<span data-ttu-id="500ec-508">Usado para desabilitar a exibição da área de firewall e proteção de rede.</span><span class="sxs-lookup"><span data-stu-id="500ec-508">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="500ec-509">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="500ec-509">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="500ec-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-510">Boolean</span></span>|<span data-ttu-id="500ec-511">Usado para desabilitar a exibição da área de proteção contra vírus e ameaças.</span><span class="sxs-lookup"><span data-stu-id="500ec-511">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="500ec-512">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="500ec-512">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="500ec-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-513">Boolean</span></span>|<span data-ttu-id="500ec-514">Usado para desabilitar a exibição da área de proteção da conta.</span><span class="sxs-lookup"><span data-stu-id="500ec-514">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="500ec-515">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="500ec-515">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="500ec-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-516">Boolean</span></span>|<span data-ttu-id="500ec-517">Usado para desabilitar a exibição do botão limpar TPM.</span><span class="sxs-lookup"><span data-stu-id="500ec-517">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="500ec-518">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="500ec-518">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="500ec-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-519">Boolean</span></span>|<span data-ttu-id="500ec-520">Usado para desabilitar a exibição da área de proteção de hardware.</span><span class="sxs-lookup"><span data-stu-id="500ec-520">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="500ec-521">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="500ec-521">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="500ec-522">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-522">Boolean</span></span>|<span data-ttu-id="500ec-523">Usado para desabilitar a exibição do controle da área de notificação.</span><span class="sxs-lookup"><span data-stu-id="500ec-523">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="500ec-524">O usuário precisa sair e entrar ou reiniciar o computador para que essa configuração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="500ec-524">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="500ec-525">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="500ec-525">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="500ec-526">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-526">Boolean</span></span>|<span data-ttu-id="500ec-527">Usado para desabilitar a exibição da área de proteção contra ransomware.</span><span class="sxs-lookup"><span data-stu-id="500ec-527">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="500ec-528">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="500ec-528">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="500ec-529">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-529">Boolean</span></span>|<span data-ttu-id="500ec-530">Usado para desabilitar a exibição da área de inicialização segura sob segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="500ec-530">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="500ec-531">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="500ec-531">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="500ec-532">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-532">Boolean</span></span>|<span data-ttu-id="500ec-533">Usado para desabilitar a exibição do processo de segurança Solucionando problemas de segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="500ec-533">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="500ec-534">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="500ec-534">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="500ec-535">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-535">Boolean</span></span>|<span data-ttu-id="500ec-536">Usado para desabilitar a exibição de atualizar o firmware do TPM quando um firmware vulnerável é detectado.</span><span class="sxs-lookup"><span data-stu-id="500ec-536">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="500ec-537">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="500ec-537">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="500ec-538">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-538">String</span></span>|<span data-ttu-id="500ec-539">O nome da empresa que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="500ec-539">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="500ec-540">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="500ec-540">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="500ec-541">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-541">String</span></span>|<span data-ttu-id="500ec-542">O endereço de email que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="500ec-542">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="500ec-543">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="500ec-543">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="500ec-544">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-544">String</span></span>|<span data-ttu-id="500ec-545">O número de telefone ou Skype ID que é exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="500ec-545">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="500ec-546">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="500ec-546">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="500ec-547">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-547">String</span></span>|<span data-ttu-id="500ec-548">A URL do portal da ajuda que é exibida para os usuários.</span><span class="sxs-lookup"><span data-stu-id="500ec-548">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="500ec-549">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="500ec-549">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="500ec-550">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="500ec-550">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="500ec-551">Notificações para mostrar das áreas de aplicativo exibidas.</span><span class="sxs-lookup"><span data-stu-id="500ec-551">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="500ec-552">Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="500ec-552">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="500ec-553">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="500ec-553">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="500ec-554">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="500ec-554">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="500ec-555">Configurar onde exibir informações de contato de ti para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="500ec-555">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="500ec-556">Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="500ec-556">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="500ec-557">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="500ec-557">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="500ec-558">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="500ec-558">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="500ec-559">Defina as configurações do Windows Defender TamperProtection.</span><span class="sxs-lookup"><span data-stu-id="500ec-559">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="500ec-560">Os valores possíveis são: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="500ec-560">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="500ec-561">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="500ec-561">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="500ec-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-562">Boolean</span></span>|<span data-ttu-id="500ec-563">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="500ec-563">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="500ec-564">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="500ec-564">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="500ec-565">Int32</span><span class="sxs-lookup"><span data-stu-id="500ec-565">Int32</span></span>|<span data-ttu-id="500ec-566">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="500ec-566">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="500ec-567">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="500ec-567">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="500ec-568">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="500ec-568">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="500ec-569">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="500ec-569">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="500ec-570">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="500ec-570">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="500ec-571">Selecione a codificação de chave pré-compartilhada a ser usada.</span><span class="sxs-lookup"><span data-stu-id="500ec-571">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="500ec-572">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="500ec-572">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="500ec-573">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="500ec-573">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="500ec-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-574">Boolean</span></span>|<span data-ttu-id="500ec-575">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="500ec-575">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="500ec-576">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="500ec-576">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="500ec-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-577">Boolean</span></span>|<span data-ttu-id="500ec-578">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="500ec-578">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="500ec-579">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="500ec-579">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="500ec-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-580">Boolean</span></span>|<span data-ttu-id="500ec-581">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="500ec-581">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="500ec-582">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="500ec-582">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="500ec-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-583">Boolean</span></span>|<span data-ttu-id="500ec-584">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="500ec-584">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="500ec-585">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="500ec-585">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="500ec-586">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="500ec-586">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="500ec-587">Especifique como a lista de certificados revogados será imposta.</span><span class="sxs-lookup"><span data-stu-id="500ec-587">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="500ec-588">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="500ec-588">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="500ec-589">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="500ec-589">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="500ec-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-590">Boolean</span></span>|<span data-ttu-id="500ec-591">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="500ec-591">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="500ec-592">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="500ec-592">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="500ec-593">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="500ec-593">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="500ec-594">Configura como o enfileiramento de pacotes deve ser aplicado no cenário de gateway de túnel.</span><span class="sxs-lookup"><span data-stu-id="500ec-594">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="500ec-595">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="500ec-595">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="500ec-596">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="500ec-596">firewallProfileDomain</span></span>|[<span data-ttu-id="500ec-597">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="500ec-597">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="500ec-598">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="500ec-598">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="500ec-599">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="500ec-599">firewallProfilePublic</span></span>|[<span data-ttu-id="500ec-600">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="500ec-600">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="500ec-601">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="500ec-601">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="500ec-602">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="500ec-602">firewallProfilePrivate</span></span>|[<span data-ttu-id="500ec-603">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="500ec-603">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="500ec-604">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="500ec-604">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="500ec-605">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="500ec-605">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="500ec-606">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-606">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-607">O valor que indica o comportamento do Adobe Reader de criar processos filhos.</span><span class="sxs-lookup"><span data-stu-id="500ec-607">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="500ec-608">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-608">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-609">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="500ec-609">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="500ec-610">String collection</span><span class="sxs-lookup"><span data-stu-id="500ec-610">String collection</span></span>|<span data-ttu-id="500ec-611">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="500ec-611">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="500ec-612">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-612">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="500ec-613">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="500ec-613">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="500ec-614">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="500ec-614">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="500ec-615">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-615">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-616">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="500ec-616">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="500ec-617">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-617">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-618">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="500ec-618">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="500ec-619">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-619">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-620">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="500ec-620">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="500ec-621">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-621">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-622">O valor que indica o comportamento dos aplicativos de comunicação do Office, incluindo o Microsoft Outlook, da criação de processos filhos.</span><span class="sxs-lookup"><span data-stu-id="500ec-622">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="500ec-623">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-623">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-624">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="500ec-624">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="500ec-625">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="500ec-625">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="500ec-626">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="500ec-626">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="500ec-627">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-627">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-628">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="500ec-628">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="500ec-629">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-629">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-630">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="500ec-630">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="500ec-631">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-631">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-632">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="500ec-632">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="500ec-633">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="500ec-633">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="500ec-634">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="500ec-634">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="500ec-635">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-635">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-636">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="500ec-636">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="500ec-637">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-637">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-638">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="500ec-638">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="500ec-639">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-639">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-640">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="500ec-640">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="500ec-641">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="500ec-641">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="500ec-642">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="500ec-642">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="500ec-643">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-643">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-644">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="500ec-644">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="500ec-645">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-645">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-646">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="500ec-646">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="500ec-647">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-647">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-648">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="500ec-648">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="500ec-649">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="500ec-649">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="500ec-650">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="500ec-650">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="500ec-651">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-651">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-652">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="500ec-652">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="500ec-653">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-653">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-654">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="500ec-654">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="500ec-655">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-655">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-656">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="500ec-656">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="500ec-657">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="500ec-657">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="500ec-658">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="500ec-658">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="500ec-659">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-659">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-660">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="500ec-660">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="500ec-661">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-661">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-662">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="500ec-662">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="500ec-663">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-663">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-664">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="500ec-664">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="500ec-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-666">Valor que indica se a credencial que está sendo roubada do subsistema de autoridade de segurança local do Windows é permitida.</span><span class="sxs-lookup"><span data-stu-id="500ec-666">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="500ec-667">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-667">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-668">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="500ec-668">defenderProcessCreationType</span></span>|[<span data-ttu-id="500ec-669">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="500ec-669">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="500ec-670">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="500ec-670">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="500ec-671">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-671">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-672">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="500ec-672">defenderProcessCreation</span></span>|[<span data-ttu-id="500ec-673">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-673">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-674">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="500ec-674">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="500ec-675">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-675">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-676">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="500ec-676">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="500ec-677">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="500ec-677">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="500ec-678">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="500ec-678">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="500ec-679">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-679">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-680">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="500ec-680">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="500ec-681">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-681">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-682">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="500ec-682">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="500ec-683">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-683">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-684">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="500ec-684">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="500ec-685">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="500ec-685">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="500ec-686">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="500ec-686">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="500ec-687">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-687">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-688">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="500ec-688">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="500ec-689">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-689">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-690">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="500ec-690">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="500ec-691">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-691">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-692">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="500ec-692">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="500ec-693">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="500ec-693">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="500ec-694">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="500ec-694">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="500ec-695">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-695">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-696">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="500ec-696">defenderEmailContentExecution</span></span>|[<span data-ttu-id="500ec-697">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-697">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-698">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="500ec-698">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="500ec-699">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-699">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-700">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-700">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="500ec-701">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-701">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-702">O valor que indica o uso da proteção avançada contra o Ransomeware.</span><span class="sxs-lookup"><span data-stu-id="500ec-702">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="500ec-703">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-703">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-704">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="500ec-704">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="500ec-705">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-705">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="500ec-706">Valor que indica o comportamento das pastas protegidas.</span><span class="sxs-lookup"><span data-stu-id="500ec-706">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="500ec-707">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="500ec-707">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="500ec-708">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="500ec-708">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="500ec-709">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-709">String collection</span></span>|<span data-ttu-id="500ec-710">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="500ec-710">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="500ec-711">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="500ec-711">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="500ec-712">String collection</span><span class="sxs-lookup"><span data-stu-id="500ec-712">String collection</span></span>|<span data-ttu-id="500ec-713">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="500ec-713">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="500ec-714">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-714">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="500ec-715">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-715">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-716">Valor que indica o comportamento de NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="500ec-716">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="500ec-717">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-717">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-718">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="500ec-718">defenderExploitProtectionXml</span></span>|<span data-ttu-id="500ec-719">Binária</span><span class="sxs-lookup"><span data-stu-id="500ec-719">Binary</span></span>|<span data-ttu-id="500ec-720">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="500ec-720">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="500ec-721">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="500ec-721">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="500ec-722">String</span><span class="sxs-lookup"><span data-stu-id="500ec-722">String</span></span>|<span data-ttu-id="500ec-723">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="500ec-723">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="500ec-724">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="500ec-724">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="500ec-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-725">Boolean</span></span>|<span data-ttu-id="500ec-726">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="500ec-726">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="500ec-727">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="500ec-727">appLockerApplicationControl</span></span>|[<span data-ttu-id="500ec-728">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="500ec-728">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="500ec-729">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="500ec-729">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="500ec-730">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="500ec-730">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="500ec-731">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="500ec-731">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="500ec-732">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="500ec-732">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="500ec-733">Ative o Credential Guard quando o nível de segurança da plataforma com segurança baseada em inicialização e virtualização segura estiverem habilitados.</span><span class="sxs-lookup"><span data-stu-id="500ec-733">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="500ec-734">Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="500ec-734">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="500ec-735">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="500ec-735">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="500ec-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-736">Boolean</span></span>|<span data-ttu-id="500ec-737">Ativa a segurança baseada em virtualização (VBS).</span><span class="sxs-lookup"><span data-stu-id="500ec-737">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="500ec-738">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="500ec-738">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="500ec-739">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-739">Boolean</span></span>|<span data-ttu-id="500ec-740">Essa propriedade será substituída em maio de 2019 e será substituída pela propriedade DeviceGuardSecureBootWithDMA.</span><span class="sxs-lookup"><span data-stu-id="500ec-740">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="500ec-741">Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="500ec-741">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="500ec-742">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="500ec-742">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="500ec-743">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="500ec-743">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="500ec-744">Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="500ec-744">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="500ec-745">Os valores possíveis são: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="500ec-745">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="500ec-746">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="500ec-746">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="500ec-747">habilitação</span><span class="sxs-lookup"><span data-stu-id="500ec-747">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="500ec-748">Permite que o administrador de ti configure o lançamento do System Guard.</span><span class="sxs-lookup"><span data-stu-id="500ec-748">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="500ec-749">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="500ec-749">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="500ec-750">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="500ec-750">smartScreenEnableInShell</span></span>|<span data-ttu-id="500ec-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-751">Boolean</span></span>|<span data-ttu-id="500ec-752">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="500ec-752">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="500ec-753">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="500ec-753">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="500ec-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-754">Boolean</span></span>|<span data-ttu-id="500ec-755">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="500ec-755">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="500ec-756">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="500ec-756">applicationGuardEnabled</span></span>|<span data-ttu-id="500ec-757">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-757">Boolean</span></span>|<span data-ttu-id="500ec-758">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="500ec-758">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="500ec-759">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="500ec-759">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="500ec-760">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="500ec-760">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="500ec-761">Habilitar o Windows Defender Application Guard para novas versões do Windows.</span><span class="sxs-lookup"><span data-stu-id="500ec-761">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="500ec-762">Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="500ec-762">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="500ec-763">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="500ec-763">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="500ec-764">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="500ec-764">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="500ec-765">Bloquear a área de transferência para transferir o arquivo de imagem, o arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="500ec-765">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="500ec-766">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="500ec-766">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="500ec-767">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="500ec-767">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="500ec-768">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-768">Boolean</span></span>|<span data-ttu-id="500ec-769">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="500ec-769">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="500ec-770">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="500ec-770">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="500ec-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-771">Boolean</span></span>|<span data-ttu-id="500ec-772">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="500ec-772">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="500ec-773">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="500ec-773">applicationGuardForceAuditing</span></span>|<span data-ttu-id="500ec-774">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-774">Boolean</span></span>|<span data-ttu-id="500ec-775">A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)</span><span class="sxs-lookup"><span data-stu-id="500ec-775">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="500ec-776">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="500ec-776">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="500ec-777">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="500ec-777">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="500ec-778">Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="500ec-778">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="500ec-779">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="500ec-779">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="500ec-780">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="500ec-780">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="500ec-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-781">Boolean</span></span>|<span data-ttu-id="500ec-782">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="500ec-782">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="500ec-783">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="500ec-783">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="500ec-784">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-784">Boolean</span></span>|<span data-ttu-id="500ec-785">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="500ec-785">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="500ec-786">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="500ec-786">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="500ec-787">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-787">Boolean</span></span>|<span data-ttu-id="500ec-788">Permitir a impressão em impressoras locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="500ec-788">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="500ec-789">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="500ec-789">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="500ec-790">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-790">Boolean</span></span>|<span data-ttu-id="500ec-791">Permitir a impressão em impressoras da rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="500ec-791">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="500ec-792">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="500ec-792">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="500ec-793">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-793">Boolean</span></span>|<span data-ttu-id="500ec-794">Permitir que o Application Guard use virtual GPU</span><span class="sxs-lookup"><span data-stu-id="500ec-794">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="500ec-795">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="500ec-795">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="500ec-796">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-796">Boolean</span></span>|<span data-ttu-id="500ec-797">Permitir que os usuários baixem arquivos da borda no contêiner do Application Guard e salve-os no sistema de arquivos host</span><span class="sxs-lookup"><span data-stu-id="500ec-797">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="500ec-798">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="500ec-798">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="500ec-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-799">Boolean</span></span>|<span data-ttu-id="500ec-800">Permite que o administrador permita que os usuários padrão habilitem o encrpytion durante o ingresso no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="500ec-800">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="500ec-801">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="500ec-801">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="500ec-802">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-802">Boolean</span></span>|<span data-ttu-id="500ec-803">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="500ec-803">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="500ec-804">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="500ec-804">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="500ec-805">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-805">Boolean</span></span>|<span data-ttu-id="500ec-806">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="500ec-806">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="500ec-807">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="500ec-807">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="500ec-808">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="500ec-808">bitLockerEncryptDevice</span></span>|<span data-ttu-id="500ec-809">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-809">Boolean</span></span>|<span data-ttu-id="500ec-810">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="500ec-810">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="500ec-811">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="500ec-811">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="500ec-812">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="500ec-812">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="500ec-813">Política de unidade de sistema BitLocker.</span><span class="sxs-lookup"><span data-stu-id="500ec-813">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="500ec-814">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="500ec-814">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="500ec-815">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="500ec-815">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="500ec-816">Política de unidade fixa do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="500ec-816">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="500ec-817">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="500ec-817">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="500ec-818">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="500ec-818">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="500ec-819">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="500ec-819">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="500ec-820">bitLockerRecoveryPasswordRotation</span><span class="sxs-lookup"><span data-stu-id="500ec-820">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="500ec-821">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="500ec-821">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-shared-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="500ec-822">Essa configuração inicia uma rotação de senha de recuperação voltada para o cliente após uma recuperação de unidade de sistema operacional (seja usando bootmgr ou WinRE).</span><span class="sxs-lookup"><span data-stu-id="500ec-822">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="500ec-823">Os valores possíveis são: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span><span class="sxs-lookup"><span data-stu-id="500ec-823">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|
|<span data-ttu-id="500ec-824">defenderDisableScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="500ec-824">defenderDisableScanArchiveFiles</span></span>|<span data-ttu-id="500ec-825">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-825">Boolean</span></span>|<span data-ttu-id="500ec-826">Permite ou proíbe a verificação de arquivos mortos.</span><span class="sxs-lookup"><span data-stu-id="500ec-826">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="500ec-827">defenderDisableBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="500ec-827">defenderDisableBehaviorMonitoring</span></span>|<span data-ttu-id="500ec-828">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-828">Boolean</span></span>|<span data-ttu-id="500ec-829">Permite ou proíbe a funcionalidade de monitoramento de comportamento do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="500ec-829">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="500ec-830">defenderDisableCloudProtection</span><span class="sxs-lookup"><span data-stu-id="500ec-830">defenderDisableCloudProtection</span></span>|<span data-ttu-id="500ec-831">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-831">Boolean</span></span>|<span data-ttu-id="500ec-832">Para melhor proteger seu computador, o Windows Defender enviará informações à Microsoft sobre qualquer problema encontrado.</span><span class="sxs-lookup"><span data-stu-id="500ec-832">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="500ec-833">A Microsoft analisará essas informações, aprenderá mais sobre problemas que afetam você e outros clientes e oferecem soluções aprimoradas.</span><span class="sxs-lookup"><span data-stu-id="500ec-833">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="500ec-834">defenderEnableScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="500ec-834">defenderEnableScanIncomingMail</span></span>|<span data-ttu-id="500ec-835">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-835">Boolean</span></span>|<span data-ttu-id="500ec-836">Permite ou proíbe a verificação de email.</span><span class="sxs-lookup"><span data-stu-id="500ec-836">Allows or disallows scanning of email.</span></span>|
|<span data-ttu-id="500ec-837">defenderEnableScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="500ec-837">defenderEnableScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="500ec-838">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-838">Boolean</span></span>|<span data-ttu-id="500ec-839">Permite ou proíbe uma verificação completa de unidades de rede mapeadas.</span><span class="sxs-lookup"><span data-stu-id="500ec-839">Allows or disallows a full scan of mapped network drives.</span></span>|
|<span data-ttu-id="500ec-840">defenderDisableScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="500ec-840">defenderDisableScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="500ec-841">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-841">Boolean</span></span>|<span data-ttu-id="500ec-842">Permite ou proíbe uma verificação completa de unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="500ec-842">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="500ec-843">Durante uma verificação rápida, as unidades removíveis ainda podem ser verificadas.</span><span class="sxs-lookup"><span data-stu-id="500ec-843">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="500ec-844">defenderDisableScanDownloads</span><span class="sxs-lookup"><span data-stu-id="500ec-844">defenderDisableScanDownloads</span></span>|<span data-ttu-id="500ec-845">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-845">Boolean</span></span>|<span data-ttu-id="500ec-846">Permite ou proíbe a funcionalidade de proteção do Windows Defender IOAVP.</span><span class="sxs-lookup"><span data-stu-id="500ec-846">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="500ec-847">defenderDisableIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="500ec-847">defenderDisableIntrusionPreventionSystem</span></span>|<span data-ttu-id="500ec-848">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-848">Boolean</span></span>|<span data-ttu-id="500ec-849">Permite ou proíbe a funcionalidade de prevenção de invasão do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="500ec-849">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="500ec-850">defenderDisableOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="500ec-850">defenderDisableOnAccessProtection</span></span>|<span data-ttu-id="500ec-851">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-851">Boolean</span></span>|<span data-ttu-id="500ec-852">Permite ou proíbe a funcionalidade de proteção de acesso do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="500ec-852">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="500ec-853">defenderDisableRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="500ec-853">defenderDisableRealTimeMonitoring</span></span>|<span data-ttu-id="500ec-854">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-854">Boolean</span></span>|<span data-ttu-id="500ec-855">Permite ou proíbe a funcionalidade de monitoramento em tempo real do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="500ec-855">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="500ec-856">defenderDisableScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="500ec-856">defenderDisableScanNetworkFiles</span></span>|<span data-ttu-id="500ec-857">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-857">Boolean</span></span>|<span data-ttu-id="500ec-858">Permite ou não a verificação de arquivos de rede.</span><span class="sxs-lookup"><span data-stu-id="500ec-858">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="500ec-859">defenderDisableScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="500ec-859">defenderDisableScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="500ec-860">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-860">Boolean</span></span>|<span data-ttu-id="500ec-861">Permite ou proíbe a funcionalidade de verificação de scripts do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="500ec-861">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="500ec-862">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="500ec-862">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="500ec-863">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-863">Boolean</span></span>|<span data-ttu-id="500ec-864">Permite ou proíbe o acesso do usuário à interface de usuário do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="500ec-864">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="500ec-865">Se não permitido, todas as notificações do Windows Defender também serão suprimidas.</span><span class="sxs-lookup"><span data-stu-id="500ec-865">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="500ec-866">defenderScanMaxCpuPercentage</span><span class="sxs-lookup"><span data-stu-id="500ec-866">defenderScanMaxCpuPercentage</span></span>|<span data-ttu-id="500ec-867">Int32</span><span class="sxs-lookup"><span data-stu-id="500ec-867">Int32</span></span>|<span data-ttu-id="500ec-868">Representa o fator de carga de CPU médio para a verificação do Windows Defender (em porcentagem).</span><span class="sxs-lookup"><span data-stu-id="500ec-868">Represents the average CPU load factor for the Windows Defender scan (in percent).</span></span> <span data-ttu-id="500ec-869">O valor padrão é 50.</span><span class="sxs-lookup"><span data-stu-id="500ec-869">The default value is 50.</span></span> <span data-ttu-id="500ec-870">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="500ec-870">Valid values 0 to 100</span></span>|
|<span data-ttu-id="500ec-871">defenderCheckForSignaturesBeforeRunningScan</span><span class="sxs-lookup"><span data-stu-id="500ec-871">defenderCheckForSignaturesBeforeRunningScan</span></span>|<span data-ttu-id="500ec-872">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-872">Boolean</span></span>|<span data-ttu-id="500ec-873">Essa configuração de política permite que você gerencie se uma verificação de novas definições de vírus e spyware ocorrerá antes de executar uma verificação.</span><span class="sxs-lookup"><span data-stu-id="500ec-873">This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.</span></span>|
|<span data-ttu-id="500ec-874">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="500ec-874">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="500ec-875">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="500ec-875">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="500ec-876">Adicionado no Windows 10, versão 1709.</span><span class="sxs-lookup"><span data-stu-id="500ec-876">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="500ec-877">Essa configuração de política determina o quanto o Windows Defender antivírus agressivo estará no bloqueio e na verificação de arquivos suspeitos.</span><span class="sxs-lookup"><span data-stu-id="500ec-877">This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files.</span></span> <span data-ttu-id="500ec-878">Tipo de valor é inteiro.</span><span class="sxs-lookup"><span data-stu-id="500ec-878">Value type is integer.</span></span> <span data-ttu-id="500ec-879">Este recurso requer a configuração "ingressar no Microsoft MAPS" habilitada para funcionar.</span><span class="sxs-lookup"><span data-stu-id="500ec-879">This feature requires the "Join Microsoft MAPS" setting enabled in order to function.</span></span> <span data-ttu-id="500ec-880">Os valores possíveis são: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span><span class="sxs-lookup"><span data-stu-id="500ec-880">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="500ec-881">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="500ec-881">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="500ec-882">Int32</span><span class="sxs-lookup"><span data-stu-id="500ec-882">Int32</span></span>|<span data-ttu-id="500ec-883">Adicionado no Windows 10, versão 1709.</span><span class="sxs-lookup"><span data-stu-id="500ec-883">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="500ec-884">Este recurso permite que o Windows Defender antivírus bloqueie um arquivo suspeito por até 60 segundos e examine-o na nuvem para garantir que ele seja seguro.</span><span class="sxs-lookup"><span data-stu-id="500ec-884">This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe.</span></span> <span data-ttu-id="500ec-885">Tipo de valor é inteiro, intervalo é 0-50.</span><span class="sxs-lookup"><span data-stu-id="500ec-885">Value type is integer, range is 0 - 50.</span></span> <span data-ttu-id="500ec-886">Esse recurso depende de três outras configurações de mapas que devem ser todos habilitadas-"Configure o bloqueio na primeira vista"; Ingresse no Microsoft MAPS "; "Enviar amostras de arquivo quando uma análise adicional é necessária".</span><span class="sxs-lookup"><span data-stu-id="500ec-886">This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required".</span></span> <span data-ttu-id="500ec-887">Valores válidos de 0 a 50</span><span class="sxs-lookup"><span data-stu-id="500ec-887">Valid values 0 to 50</span></span>|
|<span data-ttu-id="500ec-888">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="500ec-888">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="500ec-889">Int32</span><span class="sxs-lookup"><span data-stu-id="500ec-889">Int32</span></span>|<span data-ttu-id="500ec-890">Período de tempo (em dias) em que os itens de quarentena serão armazenados no sistema.</span><span class="sxs-lookup"><span data-stu-id="500ec-890">Time period (in days) that quarantine items will be stored on the system.</span></span> <span data-ttu-id="500ec-891">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="500ec-891">Valid values 0 to 90</span></span>|
|<span data-ttu-id="500ec-892">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="500ec-892">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="500ec-893">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-893">Boolean</span></span>|<span data-ttu-id="500ec-894">Essa configuração de política permite configurar verificações de atualização para verificações completas agendadas.</span><span class="sxs-lookup"><span data-stu-id="500ec-894">This policy setting allows you to configure catch-up scans for scheduled full scans.</span></span> <span data-ttu-id="500ec-895">Uma verificação de atualização é uma verificação iniciada porque uma verificação agendada regularmente foi perdida.</span><span class="sxs-lookup"><span data-stu-id="500ec-895">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="500ec-896">Normalmente, essas verificações agendadas são perdidas porque o computador foi desligado no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="500ec-896">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="500ec-897">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="500ec-897">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="500ec-898">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-898">Boolean</span></span>|<span data-ttu-id="500ec-899">Essa configuração de política permite que você configure verificações de atualização para verificações rápidas agendadas.</span><span class="sxs-lookup"><span data-stu-id="500ec-899">This policy setting allows you to configure catch-up scans for scheduled quick scans.</span></span> <span data-ttu-id="500ec-900">Uma verificação de atualização é uma verificação iniciada porque uma verificação agendada regularmente foi perdida.</span><span class="sxs-lookup"><span data-stu-id="500ec-900">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="500ec-901">Normalmente, essas verificações agendadas são perdidas porque o computador foi desligado no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="500ec-901">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="500ec-902">defenderEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="500ec-902">defenderEnableLowCpuPriority</span></span>|<span data-ttu-id="500ec-903">Boolean</span><span class="sxs-lookup"><span data-stu-id="500ec-903">Boolean</span></span>|<span data-ttu-id="500ec-904">Essa configuração de política permite habilitar ou desabilitar a baixa prioridade de CPU para verificações agendadas.</span><span class="sxs-lookup"><span data-stu-id="500ec-904">This policy setting allows you to enable or disable low CPU priority for scheduled scans.</span></span>|
|<span data-ttu-id="500ec-905">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="500ec-905">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="500ec-906">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-906">String collection</span></span>|<span data-ttu-id="500ec-907">Extensões de arquivo a serem excluídas das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="500ec-907">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="500ec-908">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="500ec-908">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="500ec-909">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="500ec-909">String collection</span></span>|<span data-ttu-id="500ec-910">Arquivos e pastas a serem excluídos das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="500ec-910">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="500ec-911">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="500ec-911">defenderProcessesToExclude</span></span>|<span data-ttu-id="500ec-912">String collection</span><span class="sxs-lookup"><span data-stu-id="500ec-912">String collection</span></span>|<span data-ttu-id="500ec-913">Processos a serem excluídos das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="500ec-913">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="500ec-914">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="500ec-914">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="500ec-915">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="500ec-915">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="500ec-916">Adicionado no Windows 10, versão 1607.</span><span class="sxs-lookup"><span data-stu-id="500ec-916">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="500ec-917">Especifica o nível de detecção para aplicativos potencialmente indesejados (PUAs).</span><span class="sxs-lookup"><span data-stu-id="500ec-917">Specifies the level of detection for potentially unwanted applications (PUAs).</span></span> <span data-ttu-id="500ec-918">O Windows Defender alerta você quando um software potencialmente indesejado está sendo baixado ou tenta se instalar em seu computador.</span><span class="sxs-lookup"><span data-stu-id="500ec-918">Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer.</span></span> <span data-ttu-id="500ec-919">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="500ec-919">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="500ec-920">defenderScanDirection</span><span class="sxs-lookup"><span data-stu-id="500ec-920">defenderScanDirection</span></span>|[<span data-ttu-id="500ec-921">defenderRealtimeScanDirection</span><span class="sxs-lookup"><span data-stu-id="500ec-921">defenderRealtimeScanDirection</span></span>](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|<span data-ttu-id="500ec-922">Controla quais conjuntos de arquivos devem ser monitorados.</span><span class="sxs-lookup"><span data-stu-id="500ec-922">Controls which sets of files should be monitored.</span></span> <span data-ttu-id="500ec-923">Os valores possíveis são: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span><span class="sxs-lookup"><span data-stu-id="500ec-923">Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="500ec-924">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="500ec-924">defenderScanType</span></span>|[<span data-ttu-id="500ec-925">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="500ec-925">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="500ec-926">Seleciona se deseja executar uma verificação rápida ou uma verificação completa.</span><span class="sxs-lookup"><span data-stu-id="500ec-926">Selects whether to perform a quick scan or full scan.</span></span> <span data-ttu-id="500ec-927">Os valores possíveis são: `userDefined`, `disabled`, `quick`, `full`.</span><span class="sxs-lookup"><span data-stu-id="500ec-927">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="500ec-928">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="500ec-928">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="500ec-929">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="500ec-929">TimeOfDay</span></span>|<span data-ttu-id="500ec-930">Seleciona a hora do dia em que a verificação rápida do Windows Defender deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="500ec-930">Selects the time of day that the Windows Defender quick scan should run.</span></span> <span data-ttu-id="500ec-931">Por exemplo, um valor de 0 = 12:00AM, um valor de 60 = 1:00AM, um valor de 120 = 2:00 e assim por diante, até um valor de 1380 = 11:00PM.</span><span class="sxs-lookup"><span data-stu-id="500ec-931">For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM.</span></span> <span data-ttu-id="500ec-932">O valor padrão é 120</span><span class="sxs-lookup"><span data-stu-id="500ec-932">The default value is 120</span></span>|
|<span data-ttu-id="500ec-933">defenderScheduledScanDay</span><span class="sxs-lookup"><span data-stu-id="500ec-933">defenderScheduledScanDay</span></span>|[<span data-ttu-id="500ec-934">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="500ec-934">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="500ec-935">Seleciona o dia em que a verificação do Windows Defender deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="500ec-935">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="500ec-936">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="500ec-936">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="500ec-937">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="500ec-937">defenderScheduledScanTime</span></span>|<span data-ttu-id="500ec-938">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="500ec-938">TimeOfDay</span></span>|<span data-ttu-id="500ec-939">Seleciona a hora do dia em que a verificação do Windows Defender deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="500ec-939">Selects the time of day that the Windows Defender scan should run.</span></span>|
|<span data-ttu-id="500ec-940">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="500ec-940">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="500ec-941">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="500ec-941">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="500ec-942">Verifica se o nível de consentimento do usuário no Windows Defender deve enviar dados.</span><span class="sxs-lookup"><span data-stu-id="500ec-942">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="500ec-943">Os valores possíveis são: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span><span class="sxs-lookup"><span data-stu-id="500ec-943">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="500ec-944">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="500ec-944">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="500ec-945">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="500ec-945">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="500ec-946">Permite que um administrador especifique quaisquer níveis de severidade de ameaças válidos e a ID de ação padrão correspondente a ser executada.</span><span class="sxs-lookup"><span data-stu-id="500ec-946">Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.</span></span>|



## <a name="response"></a><span data-ttu-id="500ec-947">Resposta</span><span class="sxs-lookup"><span data-stu-id="500ec-947">Response</span></span>
<span data-ttu-id="500ec-948">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="500ec-948">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="500ec-949">Exemplo</span><span class="sxs-lookup"><span data-stu-id="500ec-949">Example</span></span>

### <a name="request"></a><span data-ttu-id="500ec-950">Solicitação</span><span class="sxs-lookup"><span data-stu-id="500ec-950">Request</span></span>
<span data-ttu-id="500ec-951">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="500ec-951">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 30451

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
  },
  "bitLockerRecoveryPasswordRotation": "disabled",
  "defenderDisableScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderScanMaxCpuPercentage": 12,
  "defenderCheckForSignaturesBeforeRunningScan": true,
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDisableCatchupFullScan": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderEnableLowCpuPriority": true,
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPotentiallyUnwantedAppAction": "enable",
  "defenderScanDirection": "monitorIncomingFilesOnly",
  "defenderScanType": "disabled",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScheduledScanDay": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  }
}
```

### <a name="response"></a><span data-ttu-id="500ec-952">Resposta</span><span class="sxs-lookup"><span data-stu-id="500ec-952">Response</span></span>
<span data-ttu-id="500ec-p221">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="500ec-p221">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 30623

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
  },
  "bitLockerRecoveryPasswordRotation": "disabled",
  "defenderDisableScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderScanMaxCpuPercentage": 12,
  "defenderCheckForSignaturesBeforeRunningScan": true,
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDisableCatchupFullScan": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderEnableLowCpuPriority": true,
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPotentiallyUnwantedAppAction": "enable",
  "defenderScanDirection": "monitorIncomingFilesOnly",
  "defenderScanType": "disabled",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderScheduledScanDay": "everyday",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  }
}
```





