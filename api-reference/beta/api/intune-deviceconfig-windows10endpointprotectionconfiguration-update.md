---
title: Atualizar windows10EndpointProtectionConfiguration
description: Atualizar as propriedades de um objeto windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 19593b4e70b839513c305c153324c868f4adcc1d
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43431193"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="9ffcd-103">Atualizar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="9ffcd-103">Update windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="9ffcd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ffcd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ffcd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ffcd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ffcd-107">Atualizar as propriedades de um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-107">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ffcd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ffcd-108">Prerequisites</span></span>
<span data-ttu-id="9ffcd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ffcd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ffcd-111">Permission type</span></span>|<span data-ttu-id="9ffcd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ffcd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ffcd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ffcd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ffcd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ffcd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-116">Not supported.</span></span>|
|<span data-ttu-id="9ffcd-117">Application</span><span class="sxs-lookup"><span data-stu-id="9ffcd-117">Application</span></span>|<span data-ttu-id="9ffcd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ffcd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ffcd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ffcd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9ffcd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ffcd-120">Request headers</span></span>
|<span data-ttu-id="9ffcd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ffcd-121">Header</span></span>|<span data-ttu-id="9ffcd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9ffcd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ffcd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ffcd-123">Authorization</span></span>|<span data-ttu-id="9ffcd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ffcd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9ffcd-125">Accept</span></span>|<span data-ttu-id="9ffcd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ffcd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ffcd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ffcd-127">Request body</span></span>
<span data-ttu-id="9ffcd-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-128">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="9ffcd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-129">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="9ffcd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ffcd-130">Property</span></span>|<span data-ttu-id="9ffcd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ffcd-131">Type</span></span>|<span data-ttu-id="9ffcd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ffcd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ffcd-133">id</span><span class="sxs-lookup"><span data-stu-id="9ffcd-133">id</span></span>|<span data-ttu-id="9ffcd-134">String</span><span class="sxs-lookup"><span data-stu-id="9ffcd-134">String</span></span>|<span data-ttu-id="9ffcd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-135">Key of the entity.</span></span> <span data-ttu-id="9ffcd-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ffcd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ffcd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9ffcd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ffcd-138">DateTimeOffset</span></span>|<span data-ttu-id="9ffcd-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9ffcd-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ffcd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ffcd-141">roleScopeTagIds</span></span>|<span data-ttu-id="9ffcd-142">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ffcd-142">String collection</span></span>|<span data-ttu-id="9ffcd-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ffcd-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ffcd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9ffcd-145">supportsScopeTags</span></span>|<span data-ttu-id="9ffcd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-146">Boolean</span></span>|<span data-ttu-id="9ffcd-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9ffcd-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9ffcd-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9ffcd-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-150">This property is read-only.</span></span> <span data-ttu-id="9ffcd-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ffcd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ffcd-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9ffcd-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ffcd-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9ffcd-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9ffcd-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ffcd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ffcd-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9ffcd-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ffcd-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9ffcd-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9ffcd-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ffcd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9ffcd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9ffcd-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9ffcd-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9ffcd-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9ffcd-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ffcd-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ffcd-164">createdDateTime</span></span>|<span data-ttu-id="9ffcd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ffcd-165">DateTimeOffset</span></span>|<span data-ttu-id="9ffcd-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-166">DateTime the object was created.</span></span> <span data-ttu-id="9ffcd-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ffcd-168">description</span><span class="sxs-lookup"><span data-stu-id="9ffcd-168">description</span></span>|<span data-ttu-id="9ffcd-169">String</span><span class="sxs-lookup"><span data-stu-id="9ffcd-169">String</span></span>|<span data-ttu-id="9ffcd-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ffcd-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ffcd-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9ffcd-172">displayName</span></span>|<span data-ttu-id="9ffcd-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ffcd-173">String</span></span>|<span data-ttu-id="9ffcd-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ffcd-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ffcd-176">versão</span><span class="sxs-lookup"><span data-stu-id="9ffcd-176">version</span></span>|<span data-ttu-id="9ffcd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9ffcd-177">Int32</span></span>|<span data-ttu-id="9ffcd-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-178">Version of the device configuration.</span></span> <span data-ttu-id="9ffcd-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ffcd-180">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="9ffcd-180">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="9ffcd-181">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-181">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="9ffcd-182">Essa política destina-se a fornecer segurança adicional contra dispositivos compatíveis com DMA externo.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-182">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="9ffcd-183">Permite mais controle sobre a enumeração de dispositivos compatíveis com DMA externo incompatíveis com o remapeamento de DMA/isolamento de memória do dispositivo e área restrita.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-183">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="9ffcd-184">Essa política só entra em vigor quando a proteção DMA de kernel é suportada e habilitada pelo firmware do sistema.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-184">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="9ffcd-185">A proteção DMA de kernel é um recurso de plataforma que não pode ser controlado via política ou pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-185">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="9ffcd-186">É preciso ter suporte do sistema no momento da fabricação.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-186">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="9ffcd-187">Para verificar se o sistema suporta a proteção DMA de kernel, verifique o campo proteção DMA de kernel na página Resumo de MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-187">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="9ffcd-188">Os valores possíveis são: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-188">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="9ffcd-189">firewallRules</span><span class="sxs-lookup"><span data-stu-id="9ffcd-189">firewallRules</span></span>|<span data-ttu-id="9ffcd-190">coleção [windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-190">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="9ffcd-191">Define as configurações da regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-191">Configures the firewall rule settings.</span></span> <span data-ttu-id="9ffcd-192">Essa coleção pode conter um máximo de 150 elementos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-192">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="9ffcd-193">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="9ffcd-193">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="9ffcd-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-195">Esse direito de usuário é usado pelo Gerenciador de credenciais durante o backup/restauração.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-195">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="9ffcd-196">As credenciais salvas dos usuários podem ser comprometidas se esse privilégio for dado a outras entidades.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-196">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="9ffcd-197">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9ffcd-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9ffcd-198">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="9ffcd-198">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="9ffcd-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-200">Esse direito de usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-200">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="9ffcd-201">O estado permitido é suportado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-201">State Allowed is supported.</span></span>|
|<span data-ttu-id="9ffcd-202">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="9ffcd-202">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="9ffcd-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-204">Esse direito de usuário determina quais usuários e grupos são bloqueados para se conectarem ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-204">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="9ffcd-205">Há suporte para o bloco de estado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-205">State Block is supported.</span></span>|
|<span data-ttu-id="9ffcd-206">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9ffcd-206">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="9ffcd-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-208">Esse direito de usuário permite que um processo represente qualquer usuário sem autenticação.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-208">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="9ffcd-209">Portanto, o processo pode ter acesso aos mesmos recursos locais que esse usuário.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-209">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="9ffcd-210">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9ffcd-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9ffcd-211">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="9ffcd-211">userRightsLocalLogOn</span></span>|[<span data-ttu-id="9ffcd-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-213">Esse direito de usuário determina quais usuários podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-213">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="9ffcd-214">Estados não configurados, permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="9ffcd-214">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="9ffcd-215">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="9ffcd-215">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="9ffcd-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-217">Esse direito de usuário determina quais usuários não podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-217">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="9ffcd-218">Estados não configurados, bloqueados são suportados</span><span class="sxs-lookup"><span data-stu-id="9ffcd-218">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="9ffcd-219">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="9ffcd-219">userRightsBackupData</span></span>|[<span data-ttu-id="9ffcd-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-221">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao fazer backup de arquivos e diretórios.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-221">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="9ffcd-222">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9ffcd-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9ffcd-223">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="9ffcd-223">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="9ffcd-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-225">Este direito de usuário determina quais usuários e grupos podem alterar a hora e a data no relógio interno do computador.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-225">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="9ffcd-226">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9ffcd-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9ffcd-227">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="9ffcd-227">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="9ffcd-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-229">Configuração de segurança que determina se os usuários podem criar objetos globais que estão disponíveis para todas as sessões.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-229">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="9ffcd-230">Os usuários que podem criar objetos globais podem afetar processos executados em sessões de outros usuários, o que pode levar a falhas de aplicativos ou corrupção de dados.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-230">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="9ffcd-231">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9ffcd-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9ffcd-232">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="9ffcd-232">userRightsCreatePageFile</span></span>|[<span data-ttu-id="9ffcd-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-234">Esse direito de usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de paginação.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-234">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="9ffcd-235">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9ffcd-235">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9ffcd-236">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="9ffcd-236">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="9ffcd-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-238">Este direito de usuário determina quais contas podem ser usadas por processos para criar um objeto de diretório usando o Gerenciador de objetos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-238">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="9ffcd-239">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9ffcd-239">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9ffcd-240">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="9ffcd-240">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="9ffcd-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-242">Esse direito de usuário determina se o usuário pode criar um link simbólico do computador no qual está conectado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-242">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="9ffcd-243">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9ffcd-243">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9ffcd-244">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="9ffcd-244">userRightsCreateToken</span></span>|[<span data-ttu-id="9ffcd-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-246">Esse direito de usuário determina quais usuários/grupos podem ser usados por processos para criar um token que pode ser usado para obter acesso a qualquer recurso local quando o processo usa uma API interna para criar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-246">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="9ffcd-247">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9ffcd-247">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9ffcd-248">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="9ffcd-248">userRightsDebugPrograms</span></span>|[<span data-ttu-id="9ffcd-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-250">Esse direito de usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-250">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="9ffcd-251">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9ffcd-251">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9ffcd-252">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="9ffcd-252">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="9ffcd-253">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-253">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-254">Este direito de usuário determina quais usuários e grupos estão proibidos de fazer logon como um cliente de serviços de área de trabalho remota.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-254">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="9ffcd-255">Há suporte apenas para os Estados não configurados e bloqueados</span><span class="sxs-lookup"><span data-stu-id="9ffcd-255">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="9ffcd-256">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="9ffcd-256">userRightsDelegation</span></span>|[<span data-ttu-id="9ffcd-257">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-257">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-258">Este direito de usuário determina quais usuários podem definir a configuração confiável para delegação em um objeto de usuário ou computador.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-258">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="9ffcd-259">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-260">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="9ffcd-260">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="9ffcd-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-262">Este direito de usuário determina quais contas podem ser usadas por um processo para adicionar entradas ao log de segurança.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-262">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="9ffcd-263">O log de segurança é usado para rastrear o acesso de sistema não autorizado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-263">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="9ffcd-264">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-265">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="9ffcd-265">userRightsImpersonateClient</span></span>|[<span data-ttu-id="9ffcd-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-267">A atribuição desse direito de usuário a um usuário permite que programas executados em nome desse usuário representem um cliente.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-267">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="9ffcd-268">A exigência desse direito de usuário para esse tipo de representação impede que um usuário não autorizado convença um cliente a se conectar a um serviço que ele criou e, em seguida, representando esse cliente, o que pode elevar as permissões do usuário não autorizado aos níveis administrativos ou do sistema.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-268">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="9ffcd-269">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-270">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="9ffcd-270">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="9ffcd-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-272">Este direito de usuário determina quais contas podem usar um processo com acesso de propriedade de gravação a outro processo para aumentar a prioridade de execução atribuída ao outro processo.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-272">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="9ffcd-273">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-274">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="9ffcd-274">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="9ffcd-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-276">Esse direito de usuário determina quais usuários podem carregar e descarregar dinamicamente drivers de dispositivo ou outro código no modo kernel.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-276">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="9ffcd-277">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-278">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="9ffcd-278">userRightsLockMemory</span></span>|[<span data-ttu-id="9ffcd-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-280">Esse direito de usuário determina quais contas podem usar um processo para manter os dados na memória física, o que impede que o sistema pagine os dados para a memória virtual em disco.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-280">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="9ffcd-281">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-282">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="9ffcd-282">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="9ffcd-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-284">Esse direito de usuário determina quais usuários podem especificar opções de auditoria de acesso a objetos para recursos individuais, como arquivos, objetos do Active Directory e chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-284">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="9ffcd-285">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-286">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="9ffcd-286">userRightsManageVolumes</span></span>|[<span data-ttu-id="9ffcd-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-288">Esse direito de usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como a desfragmentação remota.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-288">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="9ffcd-289">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-290">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="9ffcd-290">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="9ffcd-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-292">Esse direito de usuário determina quem pode modificar os valores de ambiente de firmware.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-292">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="9ffcd-293">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-294">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="9ffcd-294">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="9ffcd-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-296">Este direito de usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves de registro ou processos pertencentes a outros usuários.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-296">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="9ffcd-297">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-298">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="9ffcd-298">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="9ffcd-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-300">Esse direito de usuário determina quais usuários podem usar ferramentas de monitoramento de desempenho para monitorar o desempenho de processos do sistema.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-300">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="9ffcd-301">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-301">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-302">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="9ffcd-302">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="9ffcd-303">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-303">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-304">Esse direito de usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-304">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="9ffcd-305">O mau uso desse direito de usuário pode resultar em uma negação de serviço.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-305">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="9ffcd-306">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-306">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-307">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="9ffcd-307">userRightsRestoreData</span></span>|[<span data-ttu-id="9ffcd-308">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-308">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-309">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao restaurar backups de arquivos e diretórios e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-309">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="9ffcd-310">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-310">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-311">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="9ffcd-311">userRightsTakeOwnership</span></span>|[<span data-ttu-id="9ffcd-312">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9ffcd-312">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9ffcd-313">Esse direito de usuário determina quais usuários podem assumir a propriedade de qualquer objeto protegível no sistema, incluindo objetos do Active Directory, arquivos e pastas, impressoras, chaves do registro, processos e threads.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-313">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="9ffcd-314">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-314">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9ffcd-315">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="9ffcd-315">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="9ffcd-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-316">Boolean</span></span>|<span data-ttu-id="9ffcd-317">Essa configuração determina se o salvamento de jogos do Xbox está habilitado (1) ou desabilitado (0).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-317">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="9ffcd-318">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="9ffcd-318">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="9ffcd-319">instarttype</span><span class="sxs-lookup"><span data-stu-id="9ffcd-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="9ffcd-320">Esta configuração determina se o tipo de início do serviço de gerenciamento de acessórios é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-320">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="9ffcd-321">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-321">Default: Manual.</span></span> <span data-ttu-id="9ffcd-322">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="9ffcd-323">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="9ffcd-323">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="9ffcd-324">instarttype</span><span class="sxs-lookup"><span data-stu-id="9ffcd-324">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="9ffcd-325">Essa configuração determina se o tipo de início do serviço do Live Authentication Manager é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-325">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="9ffcd-326">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-326">Default: Manual.</span></span> <span data-ttu-id="9ffcd-327">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-327">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="9ffcd-328">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="9ffcd-328">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="9ffcd-329">instarttype</span><span class="sxs-lookup"><span data-stu-id="9ffcd-329">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="9ffcd-330">Essa configuração determina se o tipo de início do serviço de salvamento do Live Game é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-330">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="9ffcd-331">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-331">Default: Manual.</span></span> <span data-ttu-id="9ffcd-332">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-332">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="9ffcd-333">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="9ffcd-333">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="9ffcd-334">instarttype</span><span class="sxs-lookup"><span data-stu-id="9ffcd-334">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="9ffcd-335">Esta configuração determina se o tipo de início do serviço de rede é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-335">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="9ffcd-336">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-336">Default: Manual.</span></span> <span data-ttu-id="9ffcd-337">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-337">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="9ffcd-338">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="9ffcd-338">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="9ffcd-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-339">Boolean</span></span>|<span data-ttu-id="9ffcd-340">Impedir que os usuários adicionem novas contas da Microsoft a este computador.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-340">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="9ffcd-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="9ffcd-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="9ffcd-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-342">Boolean</span></span>|<span data-ttu-id="9ffcd-343">Habilitar contas locais que não estão protegidas por senha para fazer logon de locais diferentes do dispositivo físico. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="9ffcd-343">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="9ffcd-344">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="9ffcd-344">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="9ffcd-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-345">Boolean</span></span>|<span data-ttu-id="9ffcd-346">Determina se a conta de administrador local está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-346">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="9ffcd-347">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="9ffcd-347">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="9ffcd-348">String</span><span class="sxs-lookup"><span data-stu-id="9ffcd-348">String</span></span>|<span data-ttu-id="9ffcd-349">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "administrador".</span><span class="sxs-lookup"><span data-stu-id="9ffcd-349">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="9ffcd-350">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="9ffcd-350">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="9ffcd-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-351">Boolean</span></span>|<span data-ttu-id="9ffcd-352">Determina se a conta de convidado está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-352">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="9ffcd-353">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="9ffcd-353">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="9ffcd-354">String</span><span class="sxs-lookup"><span data-stu-id="9ffcd-354">String</span></span>|<span data-ttu-id="9ffcd-355">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "convidado".</span><span class="sxs-lookup"><span data-stu-id="9ffcd-355">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="9ffcd-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="9ffcd-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="9ffcd-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-357">Boolean</span></span>|<span data-ttu-id="9ffcd-358">Impedir que um computador portátil seja desencaixado sem ter que fazer logon.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-358">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="9ffcd-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="9ffcd-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="9ffcd-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-360">Boolean</span></span>|<span data-ttu-id="9ffcd-361">Restringir a instalação dos drivers de impressora como parte da conexão a uma impressora compartilhada somente para administradores.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-361">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="9ffcd-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="9ffcd-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="9ffcd-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-363">Boolean</span></span>|<span data-ttu-id="9ffcd-364">Habilitar essa configuração permite que somente o usuário conectado interativamente acesse a mídia de CD-ROM.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-364">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="9ffcd-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="9ffcd-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="9ffcd-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="9ffcd-367">Defina quem tem permissão para formatar e ejetar a mídia NTFS removível.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-367">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="9ffcd-368">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-368">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="9ffcd-369">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="9ffcd-369">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="9ffcd-370">Int32</span><span class="sxs-lookup"><span data-stu-id="9ffcd-370">Int32</span></span>|<span data-ttu-id="9ffcd-371">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-371">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="9ffcd-372">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="9ffcd-372">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="9ffcd-373">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="9ffcd-373">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="9ffcd-374">Int32</span><span class="sxs-lookup"><span data-stu-id="9ffcd-374">Int32</span></span>|<span data-ttu-id="9ffcd-375">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="9ffcd-376">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="9ffcd-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="9ffcd-377">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="9ffcd-377">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="9ffcd-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-378">Boolean</span></span>|<span data-ttu-id="9ffcd-379">Exigir CTRL + ALT + DEL para ser pressionada para que um usuário possa fazer logon.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-379">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="9ffcd-380">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="9ffcd-380">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="9ffcd-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-381">Boolean</span></span>|<span data-ttu-id="9ffcd-382">Não exibe o nome de usuário da última pessoa que entrou neste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-382">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="9ffcd-383">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="9ffcd-383">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="9ffcd-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-384">Boolean</span></span>|<span data-ttu-id="9ffcd-385">Não exibe o nome de usuário da pessoa que está entrando neste dispositivo depois que as credenciais são inseridas e antes da área de trabalho do dispositivo ser exibida.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-385">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="9ffcd-386">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="9ffcd-386">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="9ffcd-387">String</span><span class="sxs-lookup"><span data-stu-id="9ffcd-387">String</span></span>|<span data-ttu-id="9ffcd-388">Defina o título da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-388">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="9ffcd-389">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="9ffcd-389">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="9ffcd-390">String</span><span class="sxs-lookup"><span data-stu-id="9ffcd-390">String</span></span>|<span data-ttu-id="9ffcd-391">Definir o texto da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-391">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="9ffcd-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="9ffcd-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="9ffcd-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-393">Boolean</span></span>|<span data-ttu-id="9ffcd-394">Bloquear solicitações de autenticação PKU2U para este dispositivo para usar identidades online.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-394">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="9ffcd-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="9ffcd-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="9ffcd-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-396">Boolean</span></span>|<span data-ttu-id="9ffcd-397">Boolean do auxiliar da interface do usuário para entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="9ffcd-397">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="9ffcd-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="9ffcd-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="9ffcd-399">String</span><span class="sxs-lookup"><span data-stu-id="9ffcd-399">String</span></span>|<span data-ttu-id="9ffcd-400">Edite a cadeia de caracteres de definição de descritor de segurança padrão para permitir ou impedir que usuários e grupos façam chamadas remotas para o SAM.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-400">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="9ffcd-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="9ffcd-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="9ffcd-402">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="9ffcd-402">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="9ffcd-403">Essa configuração de segurança permite que um cliente exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-403">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="9ffcd-404">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-404">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="9ffcd-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="9ffcd-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="9ffcd-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="9ffcd-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="9ffcd-407">Essa configuração de segurança permite que um servidor exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-407">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="9ffcd-408">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="9ffcd-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="9ffcd-409">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="9ffcd-410">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="9ffcd-410">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="9ffcd-411">Essa configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-411">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="9ffcd-412">Os possíveis valores são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-412">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="9ffcd-413">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="9ffcd-413">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="9ffcd-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-414">Boolean</span></span>|<span data-ttu-id="9ffcd-415">Se for habilitada, o cliente SMB permitirá logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-415">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="9ffcd-416">Se não configurada, o cliente SMB rejeitará logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-416">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="9ffcd-417">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="9ffcd-417">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="9ffcd-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-418">Boolean</span></span>|<span data-ttu-id="9ffcd-419">Configuração de segurança que determina se o arquivo de paginação de memória virtual será limpo quando o sistema for desligado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-419">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="9ffcd-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="9ffcd-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="9ffcd-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-421">Boolean</span></span>|<span data-ttu-id="9ffcd-422">Configuração de segurança que determina se um computador pode ser desligado sem a necessidade de fazer logon no Windows.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-422">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="9ffcd-423">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="9ffcd-423">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="9ffcd-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-424">Boolean</span></span>|<span data-ttu-id="9ffcd-425">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="9ffcd-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="9ffcd-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="9ffcd-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-427">Boolean</span></span>|<span data-ttu-id="9ffcd-428">Virtualizar falhas de gravação de arquivo e registro para locais por usuário</span><span class="sxs-lookup"><span data-stu-id="9ffcd-428">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="9ffcd-429">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="9ffcd-429">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="9ffcd-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-430">Boolean</span></span>|<span data-ttu-id="9ffcd-431">Impor a validação de caminho de certificação PKI para um determinado arquivo executável antes que seja permitido executar.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-431">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="9ffcd-432">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="9ffcd-432">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="9ffcd-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="9ffcd-434">Definir o comportamento do prompt de elevação para administradores no modo de aprovação de administrador.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-434">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="9ffcd-435">Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-435">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="9ffcd-436">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="9ffcd-436">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="9ffcd-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="9ffcd-438">Definir o comportamento do prompt de elevação para usuários padrão.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-438">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="9ffcd-439">Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-439">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="9ffcd-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="9ffcd-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="9ffcd-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-441">Boolean</span></span>|<span data-ttu-id="9ffcd-442">Habilite todas as solicitações de elevação para ir para a área de trabalho do usuário interativo, e não para a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-442">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="9ffcd-443">As configurações de política de comportamento de prompt para administradores e usuários padrão são usadas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-443">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="9ffcd-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="9ffcd-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="9ffcd-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-445">Boolean</span></span>|<span data-ttu-id="9ffcd-446">Instalações de aplicativos que exigem privilégios elevados solicitarão credenciais de administrador. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="9ffcd-446">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="9ffcd-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="9ffcd-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="9ffcd-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-448">Boolean</span></span>|<span data-ttu-id="9ffcd-449">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="9ffcd-449">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="9ffcd-450">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="9ffcd-450">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="9ffcd-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-451">Boolean</span></span>|<span data-ttu-id="9ffcd-452">Define se a conta de administrador interna usa o modo de aprovação de administrador ou executa todos os aplicativos com privilégios de administrador completo. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="9ffcd-452">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="9ffcd-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="9ffcd-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="9ffcd-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-454">Boolean</span></span>|<span data-ttu-id="9ffcd-455">Definir se o modo de aprovação de administrador e todas as configurações de política de UAC estão habilitados, o padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="9ffcd-455">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="9ffcd-456">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="9ffcd-456">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="9ffcd-457">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-457">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="9ffcd-458">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-458">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="9ffcd-459">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-459">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="9ffcd-460">Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-460">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="9ffcd-461">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="9ffcd-461">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="9ffcd-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="9ffcd-463">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-463">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="9ffcd-464">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-464">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="9ffcd-465">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-465">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="9ffcd-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="9ffcd-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="9ffcd-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-467">Boolean</span></span>|<span data-ttu-id="9ffcd-468">Configuração de segurança que determina se o cliente SMB tentará negociar assinatura de pacote SMB.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-468">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="9ffcd-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="9ffcd-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="9ffcd-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-470">Boolean</span></span>|<span data-ttu-id="9ffcd-471">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do cliente SMB.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-471">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="9ffcd-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="9ffcd-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="9ffcd-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-473">Boolean</span></span>|<span data-ttu-id="9ffcd-474">Se essa configuração de segurança estiver habilitada, o redirecionador de bloco de mensagens de servidor (SMB) terá permissão para enviar senhas de texto não criptografado para servidores SMB não Microsoft que não ofereçam suporte à criptografia de senha durante a autenticação.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-474">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="9ffcd-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="9ffcd-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="9ffcd-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-476">Boolean</span></span>|<span data-ttu-id="9ffcd-477">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do servidor SMB.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-477">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="9ffcd-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="9ffcd-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="9ffcd-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-479">Boolean</span></span>|<span data-ttu-id="9ffcd-480">Configuração de segurança que determina se o servidor SMB negociará assinatura de pacote SMB com clientes que solicitarem.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-480">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="9ffcd-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="9ffcd-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="9ffcd-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-482">Boolean</span></span>|<span data-ttu-id="9ffcd-483">Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e pipes para as configurações de pipes nomeados que podem ser acessados anonimamente e compartilhamentos que podem ser acessados anonimamente</span><span class="sxs-lookup"><span data-stu-id="9ffcd-483">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="9ffcd-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="9ffcd-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="9ffcd-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-485">Boolean</span></span>|<span data-ttu-id="9ffcd-486">Essa configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas com o computador.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-486">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="9ffcd-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="9ffcd-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="9ffcd-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-488">Boolean</span></span>|<span data-ttu-id="9ffcd-489">Configuração de segurança que determina se os usuários anônimos devem executar determinadas atividades, como enumeração de nomes de contas de domínio e compartilhamentos de rede.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-489">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="9ffcd-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="9ffcd-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="9ffcd-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-491">Boolean</span></span>|<span data-ttu-id="9ffcd-492">Essa configuração de segurança determina se, na próxima alteração de senha, o valor de hash do LM (LAN Manager) para a nova senha é armazenado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-492">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="9ffcd-493">Ele não é armazenado por padrão.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-493">It’s not stored by default.</span></span>|
|<span data-ttu-id="9ffcd-494">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="9ffcd-494">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="9ffcd-495">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-495">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="9ffcd-496">Essa configuração de segurança determina o que acontece quando o cartão inteligente de um usuário conectado é removido do leitor de cartão inteligente.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-496">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="9ffcd-497">Os valores possíveis são: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-497">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="9ffcd-498">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-498">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="9ffcd-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-499">Boolean</span></span>|<span data-ttu-id="9ffcd-500">Usado para desabilitar a exibição da área de proteção de aplicativo e navegador.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-500">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="9ffcd-501">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-501">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="9ffcd-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-502">Boolean</span></span>|<span data-ttu-id="9ffcd-503">Usado para desabilitar a exibição da área de opções da família.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-503">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="9ffcd-504">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-504">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="9ffcd-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-505">Boolean</span></span>|<span data-ttu-id="9ffcd-506">Usado para desabilitar a exibição da área de desempenho e integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-506">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="9ffcd-507">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-507">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="9ffcd-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-508">Boolean</span></span>|<span data-ttu-id="9ffcd-509">Usado para desabilitar a exibição da área de firewall e proteção de rede.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-509">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="9ffcd-510">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-510">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="9ffcd-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-511">Boolean</span></span>|<span data-ttu-id="9ffcd-512">Usado para desabilitar a exibição da área de proteção contra vírus e ameaças.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-512">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="9ffcd-513">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-513">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="9ffcd-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-514">Boolean</span></span>|<span data-ttu-id="9ffcd-515">Usado para desabilitar a exibição da área de proteção da conta.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-515">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="9ffcd-516">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-516">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="9ffcd-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-517">Boolean</span></span>|<span data-ttu-id="9ffcd-518">Usado para desabilitar a exibição do botão limpar TPM.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-518">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="9ffcd-519">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-519">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="9ffcd-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-520">Boolean</span></span>|<span data-ttu-id="9ffcd-521">Usado para desabilitar a exibição da área de proteção de hardware.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-521">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="9ffcd-522">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-522">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="9ffcd-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-523">Boolean</span></span>|<span data-ttu-id="9ffcd-524">Usado para desabilitar a exibição do controle da área de notificação.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-524">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="9ffcd-525">O usuário precisa sair e entrar ou reiniciar o computador para que essa configuração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-525">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="9ffcd-526">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-526">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="9ffcd-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-527">Boolean</span></span>|<span data-ttu-id="9ffcd-528">Usado para desabilitar a exibição da área de proteção contra ransomware.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-528">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="9ffcd-529">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-529">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="9ffcd-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-530">Boolean</span></span>|<span data-ttu-id="9ffcd-531">Usado para desabilitar a exibição da área de inicialização segura sob segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-531">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="9ffcd-532">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-532">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="9ffcd-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-533">Boolean</span></span>|<span data-ttu-id="9ffcd-534">Usado para desabilitar a exibição do processo de segurança Solucionando problemas de segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-534">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="9ffcd-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="9ffcd-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="9ffcd-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-536">Boolean</span></span>|<span data-ttu-id="9ffcd-537">Usado para desabilitar a exibição de atualizar o firmware do TPM quando um firmware vulnerável é detectado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-537">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="9ffcd-538">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="9ffcd-538">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="9ffcd-539">String</span><span class="sxs-lookup"><span data-stu-id="9ffcd-539">String</span></span>|<span data-ttu-id="9ffcd-540">O nome da empresa que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-540">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="9ffcd-541">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="9ffcd-541">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="9ffcd-542">String</span><span class="sxs-lookup"><span data-stu-id="9ffcd-542">String</span></span>|<span data-ttu-id="9ffcd-543">O endereço de email que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-543">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="9ffcd-544">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="9ffcd-544">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="9ffcd-545">String</span><span class="sxs-lookup"><span data-stu-id="9ffcd-545">String</span></span>|<span data-ttu-id="9ffcd-546">O número de telefone ou Skype ID que é exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-546">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="9ffcd-547">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="9ffcd-547">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="9ffcd-548">String</span><span class="sxs-lookup"><span data-stu-id="9ffcd-548">String</span></span>|<span data-ttu-id="9ffcd-549">A URL do portal da ajuda que é exibida para os usuários.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-549">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="9ffcd-550">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="9ffcd-550">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="9ffcd-551">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-551">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="9ffcd-552">Notificações para mostrar das áreas de aplicativo exibidas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-552">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="9ffcd-553">Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-553">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="9ffcd-554">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="9ffcd-554">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="9ffcd-555">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-555">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="9ffcd-556">Configurar onde exibir informações de contato de ti para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-556">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="9ffcd-557">Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-557">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="9ffcd-558">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="9ffcd-558">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="9ffcd-559">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="9ffcd-559">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="9ffcd-560">Defina as configurações do Windows Defender TamperProtection.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-560">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="9ffcd-561">Os valores possíveis são: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-561">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="9ffcd-562">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="9ffcd-562">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="9ffcd-563">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-563">Boolean</span></span>|<span data-ttu-id="9ffcd-564">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="9ffcd-564">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="9ffcd-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="9ffcd-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="9ffcd-566">Int32</span><span class="sxs-lookup"><span data-stu-id="9ffcd-566">Int32</span></span>|<span data-ttu-id="9ffcd-567">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-567">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="9ffcd-568">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-568">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="9ffcd-569">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="9ffcd-569">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="9ffcd-570">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="9ffcd-570">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="9ffcd-571">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-571">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="9ffcd-572">Selecione a codificação de chave pré-compartilhada a ser usada.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-572">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="9ffcd-573">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-573">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="9ffcd-574">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="9ffcd-574">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="9ffcd-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-575">Boolean</span></span>|<span data-ttu-id="9ffcd-576">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="9ffcd-576">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="9ffcd-577">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="9ffcd-577">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="9ffcd-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-578">Boolean</span></span>|<span data-ttu-id="9ffcd-579">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="9ffcd-579">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="9ffcd-580">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="9ffcd-580">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="9ffcd-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-581">Boolean</span></span>|<span data-ttu-id="9ffcd-582">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="9ffcd-582">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="9ffcd-583">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="9ffcd-583">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="9ffcd-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-584">Boolean</span></span>|<span data-ttu-id="9ffcd-585">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="9ffcd-585">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="9ffcd-586">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="9ffcd-586">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="9ffcd-587">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-587">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="9ffcd-588">Especifique como a lista de certificados revogados será imposta.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-588">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="9ffcd-589">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-589">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="9ffcd-590">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="9ffcd-590">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="9ffcd-591">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-591">Boolean</span></span>|<span data-ttu-id="9ffcd-592">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="9ffcd-592">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="9ffcd-593">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="9ffcd-593">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="9ffcd-594">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-594">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="9ffcd-595">Configura como o enfileiramento de pacotes deve ser aplicado no cenário de gateway de túnel.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-595">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="9ffcd-596">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-596">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="9ffcd-597">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="9ffcd-597">firewallProfileDomain</span></span>|[<span data-ttu-id="9ffcd-598">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9ffcd-598">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="9ffcd-599">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="9ffcd-599">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="9ffcd-600">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="9ffcd-600">firewallProfilePublic</span></span>|[<span data-ttu-id="9ffcd-601">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9ffcd-601">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="9ffcd-602">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="9ffcd-602">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="9ffcd-603">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="9ffcd-603">firewallProfilePrivate</span></span>|[<span data-ttu-id="9ffcd-604">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9ffcd-604">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="9ffcd-605">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="9ffcd-605">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="9ffcd-606">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="9ffcd-606">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="9ffcd-607">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-607">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-608">O valor que indica o comportamento do Adobe Reader de criar processos filhos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-608">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="9ffcd-609">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-609">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-610">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="9ffcd-610">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="9ffcd-611">String collection</span><span class="sxs-lookup"><span data-stu-id="9ffcd-611">String collection</span></span>|<span data-ttu-id="9ffcd-612">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="9ffcd-612">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="9ffcd-613">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-613">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="9ffcd-614">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-614">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9ffcd-615">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-615">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="9ffcd-616">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-616">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-617">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="9ffcd-617">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="9ffcd-618">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-618">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-619">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-619">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="9ffcd-620">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-620">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-621">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="9ffcd-621">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="9ffcd-622">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-623">O valor que indica o comportamento dos aplicativos de comunicação do Office, incluindo o Microsoft Outlook, da criação de processos filhos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-623">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="9ffcd-624">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-625">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-625">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="9ffcd-626">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-626">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9ffcd-627">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-627">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="9ffcd-628">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-628">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-629">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="9ffcd-629">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="9ffcd-630">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-630">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-631">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-631">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="9ffcd-632">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-632">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-633">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-633">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="9ffcd-634">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-634">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9ffcd-635">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-635">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="9ffcd-636">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-636">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-637">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="9ffcd-637">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="9ffcd-638">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-638">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-639">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-639">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="9ffcd-640">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-640">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-641">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-641">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="9ffcd-642">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-642">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9ffcd-643">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-643">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="9ffcd-644">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-644">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-645">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="9ffcd-645">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="9ffcd-646">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-647">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-647">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="9ffcd-648">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-649">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-649">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="9ffcd-650">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-650">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9ffcd-651">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-651">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="9ffcd-652">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-652">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-653">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="9ffcd-653">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="9ffcd-654">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-654">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-655">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-655">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="9ffcd-656">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-656">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-657">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-657">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="9ffcd-658">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-658">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9ffcd-659">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-659">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="9ffcd-660">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-660">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-661">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="9ffcd-661">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="9ffcd-662">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-662">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-663">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-663">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="9ffcd-664">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-664">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-665">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-665">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="9ffcd-666">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-667">Valor que indica se a credencial que está sendo roubada do subsistema de autoridade de segurança local do Windows é permitida.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-667">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="9ffcd-668">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-669">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-669">defenderProcessCreationType</span></span>|[<span data-ttu-id="9ffcd-670">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-670">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9ffcd-671">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-671">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="9ffcd-672">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-672">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-673">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="9ffcd-673">defenderProcessCreation</span></span>|[<span data-ttu-id="9ffcd-674">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-674">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-675">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-675">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="9ffcd-676">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-676">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-677">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-677">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="9ffcd-678">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-678">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9ffcd-679">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-679">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="9ffcd-680">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-680">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-681">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="9ffcd-681">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="9ffcd-682">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-683">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-683">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="9ffcd-684">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-685">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-685">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="9ffcd-686">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-686">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9ffcd-687">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-687">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="9ffcd-688">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-688">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-689">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="9ffcd-689">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="9ffcd-690">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-690">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-691">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-691">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="9ffcd-692">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-692">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-693">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-693">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="9ffcd-694">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-694">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9ffcd-695">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-695">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="9ffcd-696">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-696">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-697">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="9ffcd-697">defenderEmailContentExecution</span></span>|[<span data-ttu-id="9ffcd-698">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-698">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-699">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-699">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="9ffcd-700">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-700">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-701">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-701">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="9ffcd-702">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-702">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-703">O valor que indica o uso da proteção avançada contra o Ransomeware.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-703">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="9ffcd-704">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-704">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-705">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-705">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="9ffcd-706">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-706">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="9ffcd-707">Valor que indica o comportamento das pastas protegidas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-707">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="9ffcd-708">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-708">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="9ffcd-709">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="9ffcd-709">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="9ffcd-710">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ffcd-710">String collection</span></span>|<span data-ttu-id="9ffcd-711">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="9ffcd-711">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="9ffcd-712">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="9ffcd-712">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="9ffcd-713">String collection</span><span class="sxs-lookup"><span data-stu-id="9ffcd-713">String collection</span></span>|<span data-ttu-id="9ffcd-714">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="9ffcd-714">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="9ffcd-715">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-715">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="9ffcd-716">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-716">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-717">Valor que indica o comportamento de NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-717">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="9ffcd-718">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-718">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-719">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="9ffcd-719">defenderExploitProtectionXml</span></span>|<span data-ttu-id="9ffcd-720">Binária</span><span class="sxs-lookup"><span data-stu-id="9ffcd-720">Binary</span></span>|<span data-ttu-id="9ffcd-721">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-721">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="9ffcd-722">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="9ffcd-722">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="9ffcd-723">String</span><span class="sxs-lookup"><span data-stu-id="9ffcd-723">String</span></span>|<span data-ttu-id="9ffcd-724">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-724">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="9ffcd-725">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="9ffcd-725">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="9ffcd-726">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-726">Boolean</span></span>|<span data-ttu-id="9ffcd-727">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-727">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="9ffcd-728">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="9ffcd-728">appLockerApplicationControl</span></span>|[<span data-ttu-id="9ffcd-729">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-729">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="9ffcd-730">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-730">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="9ffcd-731">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-731">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="9ffcd-732">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="9ffcd-732">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="9ffcd-733">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-733">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="9ffcd-734">Ative o Credential Guard quando o nível de segurança da plataforma com segurança baseada em inicialização e virtualização segura estiverem habilitados.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-734">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="9ffcd-735">Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-735">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="9ffcd-736">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="9ffcd-736">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="9ffcd-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-737">Boolean</span></span>|<span data-ttu-id="9ffcd-738">Ativa a segurança baseada em virtualização (VBS).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-738">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="9ffcd-739">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="9ffcd-739">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="9ffcd-740">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-740">Boolean</span></span>|<span data-ttu-id="9ffcd-741">Essa propriedade será substituída em maio de 2019 e será substituída pela propriedade DeviceGuardSecureBootWithDMA.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-741">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="9ffcd-742">Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-742">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="9ffcd-743">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="9ffcd-743">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="9ffcd-744">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-744">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="9ffcd-745">Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-745">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="9ffcd-746">Os valores possíveis são: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-746">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="9ffcd-747">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="9ffcd-747">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="9ffcd-748">habilitação</span><span class="sxs-lookup"><span data-stu-id="9ffcd-748">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9ffcd-749">Permite que o administrador de ti configure o lançamento do System Guard.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-749">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="9ffcd-750">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-750">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9ffcd-751">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="9ffcd-751">smartScreenEnableInShell</span></span>|<span data-ttu-id="9ffcd-752">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-752">Boolean</span></span>|<span data-ttu-id="9ffcd-753">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-753">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="9ffcd-754">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="9ffcd-754">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="9ffcd-755">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-755">Boolean</span></span>|<span data-ttu-id="9ffcd-756">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-756">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="9ffcd-757">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="9ffcd-757">applicationGuardEnabled</span></span>|<span data-ttu-id="9ffcd-758">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-758">Boolean</span></span>|<span data-ttu-id="9ffcd-759">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="9ffcd-759">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="9ffcd-760">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="9ffcd-760">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="9ffcd-761">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="9ffcd-761">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="9ffcd-762">Habilitar o Windows Defender Application Guard para novas versões do Windows.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-762">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="9ffcd-763">Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-763">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="9ffcd-764">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="9ffcd-764">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="9ffcd-765">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-765">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="9ffcd-766">Bloquear a área de transferência para transferir o arquivo de imagem, o arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-766">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="9ffcd-767">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-767">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="9ffcd-768">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="9ffcd-768">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="9ffcd-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-769">Boolean</span></span>|<span data-ttu-id="9ffcd-770">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="9ffcd-770">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="9ffcd-771">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="9ffcd-771">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="9ffcd-772">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-772">Boolean</span></span>|<span data-ttu-id="9ffcd-773">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-773">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="9ffcd-774">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="9ffcd-774">applicationGuardForceAuditing</span></span>|<span data-ttu-id="9ffcd-775">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-775">Boolean</span></span>|<span data-ttu-id="9ffcd-776">A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)</span><span class="sxs-lookup"><span data-stu-id="9ffcd-776">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="9ffcd-777">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="9ffcd-777">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="9ffcd-778">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-778">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="9ffcd-779">Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-779">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="9ffcd-780">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-780">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="9ffcd-781">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="9ffcd-781">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="9ffcd-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-782">Boolean</span></span>|<span data-ttu-id="9ffcd-783">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="9ffcd-783">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="9ffcd-784">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="9ffcd-784">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="9ffcd-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-785">Boolean</span></span>|<span data-ttu-id="9ffcd-786">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="9ffcd-786">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="9ffcd-787">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="9ffcd-787">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="9ffcd-788">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-788">Boolean</span></span>|<span data-ttu-id="9ffcd-789">Permitir a impressão em impressoras locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="9ffcd-789">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="9ffcd-790">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="9ffcd-790">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="9ffcd-791">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-791">Boolean</span></span>|<span data-ttu-id="9ffcd-792">Permitir a impressão em impressoras da rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="9ffcd-792">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="9ffcd-793">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="9ffcd-793">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="9ffcd-794">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-794">Boolean</span></span>|<span data-ttu-id="9ffcd-795">Permitir que o Application Guard use virtual GPU</span><span class="sxs-lookup"><span data-stu-id="9ffcd-795">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="9ffcd-796">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="9ffcd-796">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="9ffcd-797">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-797">Boolean</span></span>|<span data-ttu-id="9ffcd-798">Permitir que os usuários baixem arquivos da borda no contêiner do Application Guard e salve-os no sistema de arquivos host</span><span class="sxs-lookup"><span data-stu-id="9ffcd-798">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="9ffcd-799">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="9ffcd-799">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="9ffcd-800">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-800">Boolean</span></span>|<span data-ttu-id="9ffcd-801">Permite que o administrador permita que os usuários padrão habilitem o encrpytion durante o ingresso no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-801">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="9ffcd-802">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="9ffcd-802">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="9ffcd-803">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-803">Boolean</span></span>|<span data-ttu-id="9ffcd-804">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-804">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="9ffcd-805">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="9ffcd-805">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="9ffcd-806">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-806">Boolean</span></span>|<span data-ttu-id="9ffcd-807">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-807">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="9ffcd-808">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-808">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="9ffcd-809">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="9ffcd-809">bitLockerEncryptDevice</span></span>|<span data-ttu-id="9ffcd-810">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-810">Boolean</span></span>|<span data-ttu-id="9ffcd-811">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-811">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="9ffcd-812">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9ffcd-812">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="9ffcd-813">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9ffcd-813">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="9ffcd-814">Política de unidade de sistema BitLocker.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-814">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="9ffcd-815">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9ffcd-815">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="9ffcd-816">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9ffcd-816">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="9ffcd-817">Política de unidade fixa do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-817">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="9ffcd-818">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9ffcd-818">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="9ffcd-819">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9ffcd-819">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="9ffcd-820">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-820">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="9ffcd-821">bitLockerRecoveryPasswordRotation</span><span class="sxs-lookup"><span data-stu-id="9ffcd-821">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="9ffcd-822">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-822">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="9ffcd-823">Essa configuração inicia uma rotação de senha de recuperação voltada para o cliente após uma recuperação de unidade de sistema operacional (seja usando bootmgr ou WinRE).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-823">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="9ffcd-824">Os valores possíveis são: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-824">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|
|<span data-ttu-id="9ffcd-825">defenderDisableScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="9ffcd-825">defenderDisableScanArchiveFiles</span></span>|<span data-ttu-id="9ffcd-826">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-826">Boolean</span></span>|<span data-ttu-id="9ffcd-827">Permite ou proíbe a verificação de arquivos mortos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-827">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="9ffcd-828">defenderAllowScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="9ffcd-828">defenderAllowScanArchiveFiles</span></span>|<span data-ttu-id="9ffcd-829">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-829">Boolean</span></span>|<span data-ttu-id="9ffcd-830">Permite ou proíbe a verificação de arquivos mortos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-830">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="9ffcd-831">defenderDisableBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="9ffcd-831">defenderDisableBehaviorMonitoring</span></span>|<span data-ttu-id="9ffcd-832">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-832">Boolean</span></span>|<span data-ttu-id="9ffcd-833">Permite ou proíbe a funcionalidade de monitoramento de comportamento do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-833">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="9ffcd-834">defenderAllowBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="9ffcd-834">defenderAllowBehaviorMonitoring</span></span>|<span data-ttu-id="9ffcd-835">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-835">Boolean</span></span>|<span data-ttu-id="9ffcd-836">Permite ou proíbe a funcionalidade de monitoramento de comportamento do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-836">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="9ffcd-837">defenderDisableCloudProtection</span><span class="sxs-lookup"><span data-stu-id="9ffcd-837">defenderDisableCloudProtection</span></span>|<span data-ttu-id="9ffcd-838">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-838">Boolean</span></span>|<span data-ttu-id="9ffcd-839">Para melhor proteger seu computador, o Windows Defender enviará informações à Microsoft sobre qualquer problema encontrado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-839">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="9ffcd-840">A Microsoft analisará essas informações, aprenderá mais sobre problemas que afetam você e outros clientes e oferecem soluções aprimoradas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-840">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="9ffcd-841">defenderAllowCloudProtection</span><span class="sxs-lookup"><span data-stu-id="9ffcd-841">defenderAllowCloudProtection</span></span>|<span data-ttu-id="9ffcd-842">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-842">Boolean</span></span>|<span data-ttu-id="9ffcd-843">Para melhor proteger seu computador, o Windows Defender enviará informações à Microsoft sobre qualquer problema encontrado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-843">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="9ffcd-844">A Microsoft analisará essas informações, aprenderá mais sobre problemas que afetam você e outros clientes e oferecem soluções aprimoradas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-844">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="9ffcd-845">defenderEnableScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="9ffcd-845">defenderEnableScanIncomingMail</span></span>|<span data-ttu-id="9ffcd-846">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-846">Boolean</span></span>|<span data-ttu-id="9ffcd-847">Permite ou proíbe a verificação de email.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-847">Allows or disallows scanning of email.</span></span>|
|<span data-ttu-id="9ffcd-848">defenderEnableScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="9ffcd-848">defenderEnableScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="9ffcd-849">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-849">Boolean</span></span>|<span data-ttu-id="9ffcd-850">Permite ou proíbe uma verificação completa de unidades de rede mapeadas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-850">Allows or disallows a full scan of mapped network drives.</span></span>|
|<span data-ttu-id="9ffcd-851">defenderDisableScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="9ffcd-851">defenderDisableScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="9ffcd-852">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-852">Boolean</span></span>|<span data-ttu-id="9ffcd-853">Permite ou proíbe uma verificação completa de unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-853">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="9ffcd-854">Durante uma verificação rápida, as unidades removíveis ainda podem ser verificadas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-854">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="9ffcd-855">defenderAllowScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="9ffcd-855">defenderAllowScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="9ffcd-856">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-856">Boolean</span></span>|<span data-ttu-id="9ffcd-857">Permite ou proíbe uma verificação completa de unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-857">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="9ffcd-858">Durante uma verificação rápida, as unidades removíveis ainda podem ser verificadas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-858">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="9ffcd-859">defenderDisableScanDownloads</span><span class="sxs-lookup"><span data-stu-id="9ffcd-859">defenderDisableScanDownloads</span></span>|<span data-ttu-id="9ffcd-860">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-860">Boolean</span></span>|<span data-ttu-id="9ffcd-861">Permite ou proíbe a funcionalidade de proteção do Windows Defender IOAVP.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-861">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="9ffcd-862">defenderAllowScanDownloads</span><span class="sxs-lookup"><span data-stu-id="9ffcd-862">defenderAllowScanDownloads</span></span>|<span data-ttu-id="9ffcd-863">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-863">Boolean</span></span>|<span data-ttu-id="9ffcd-864">Permite ou proíbe a funcionalidade de proteção do Windows Defender IOAVP.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-864">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="9ffcd-865">defenderDisableIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="9ffcd-865">defenderDisableIntrusionPreventionSystem</span></span>|<span data-ttu-id="9ffcd-866">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-866">Boolean</span></span>|<span data-ttu-id="9ffcd-867">Permite ou proíbe a funcionalidade de prevenção de invasão do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-867">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="9ffcd-868">defenderAllowIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="9ffcd-868">defenderAllowIntrusionPreventionSystem</span></span>|<span data-ttu-id="9ffcd-869">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-869">Boolean</span></span>|<span data-ttu-id="9ffcd-870">Permite ou proíbe a funcionalidade de prevenção de invasão do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-870">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="9ffcd-871">defenderDisableOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="9ffcd-871">defenderDisableOnAccessProtection</span></span>|<span data-ttu-id="9ffcd-872">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-872">Boolean</span></span>|<span data-ttu-id="9ffcd-873">Permite ou proíbe a funcionalidade de proteção de acesso do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-873">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="9ffcd-874">defenderAllowOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="9ffcd-874">defenderAllowOnAccessProtection</span></span>|<span data-ttu-id="9ffcd-875">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-875">Boolean</span></span>|<span data-ttu-id="9ffcd-876">Permite ou proíbe a funcionalidade de proteção de acesso do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-876">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="9ffcd-877">defenderDisableRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="9ffcd-877">defenderDisableRealTimeMonitoring</span></span>|<span data-ttu-id="9ffcd-878">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-878">Boolean</span></span>|<span data-ttu-id="9ffcd-879">Permite ou proíbe a funcionalidade de monitoramento em tempo real do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-879">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="9ffcd-880">defenderAllowRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="9ffcd-880">defenderAllowRealTimeMonitoring</span></span>|<span data-ttu-id="9ffcd-881">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-881">Boolean</span></span>|<span data-ttu-id="9ffcd-882">Permite ou proíbe a funcionalidade de monitoramento em tempo real do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-882">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="9ffcd-883">defenderDisableScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="9ffcd-883">defenderDisableScanNetworkFiles</span></span>|<span data-ttu-id="9ffcd-884">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-884">Boolean</span></span>|<span data-ttu-id="9ffcd-885">Permite ou não a verificação de arquivos de rede.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-885">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="9ffcd-886">defenderAllowScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="9ffcd-886">defenderAllowScanNetworkFiles</span></span>|<span data-ttu-id="9ffcd-887">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-887">Boolean</span></span>|<span data-ttu-id="9ffcd-888">Permite ou não a verificação de arquivos de rede.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-888">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="9ffcd-889">defenderDisableScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="9ffcd-889">defenderDisableScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="9ffcd-890">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-890">Boolean</span></span>|<span data-ttu-id="9ffcd-891">Permite ou proíbe a funcionalidade de verificação de scripts do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-891">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="9ffcd-892">defenderAllowScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="9ffcd-892">defenderAllowScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="9ffcd-893">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-893">Boolean</span></span>|<span data-ttu-id="9ffcd-894">Permite ou proíbe a funcionalidade de verificação de scripts do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-894">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="9ffcd-895">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="9ffcd-895">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="9ffcd-896">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-896">Boolean</span></span>|<span data-ttu-id="9ffcd-897">Permite ou proíbe o acesso do usuário à interface de usuário do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-897">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="9ffcd-898">Se não permitido, todas as notificações do Windows Defender também serão suprimidas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-898">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="9ffcd-899">defenderAllowEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="9ffcd-899">defenderAllowEndUserAccess</span></span>|<span data-ttu-id="9ffcd-900">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-900">Boolean</span></span>|<span data-ttu-id="9ffcd-901">Permite ou proíbe o acesso do usuário à interface de usuário do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-901">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="9ffcd-902">Se não permitido, todas as notificações do Windows Defender também serão suprimidas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-902">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="9ffcd-903">defenderScanMaxCpuPercentage</span><span class="sxs-lookup"><span data-stu-id="9ffcd-903">defenderScanMaxCpuPercentage</span></span>|<span data-ttu-id="9ffcd-904">Int32</span><span class="sxs-lookup"><span data-stu-id="9ffcd-904">Int32</span></span>|<span data-ttu-id="9ffcd-905">Representa o fator de carga de CPU médio para a verificação do Windows Defender (em porcentagem).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-905">Represents the average CPU load factor for the Windows Defender scan (in percent).</span></span> <span data-ttu-id="9ffcd-906">O valor padrão é 50.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-906">The default value is 50.</span></span> <span data-ttu-id="9ffcd-907">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="9ffcd-907">Valid values 0 to 100</span></span>|
|<span data-ttu-id="9ffcd-908">defenderCheckForSignaturesBeforeRunningScan</span><span class="sxs-lookup"><span data-stu-id="9ffcd-908">defenderCheckForSignaturesBeforeRunningScan</span></span>|<span data-ttu-id="9ffcd-909">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-909">Boolean</span></span>|<span data-ttu-id="9ffcd-910">Essa configuração de política permite que você gerencie se uma verificação de novas definições de vírus e spyware ocorrerá antes de executar uma verificação.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-910">This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.</span></span>|
|<span data-ttu-id="9ffcd-911">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="9ffcd-911">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="9ffcd-912">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-912">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="9ffcd-913">Adicionado no Windows 10, versão 1709.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-913">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="9ffcd-914">Essa configuração de política determina o quanto o Windows Defender antivírus agressivo estará no bloqueio e na verificação de arquivos suspeitos.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-914">This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files.</span></span> <span data-ttu-id="9ffcd-915">Tipo de valor é inteiro.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-915">Value type is integer.</span></span> <span data-ttu-id="9ffcd-916">Este recurso requer a configuração "ingressar no Microsoft MAPS" habilitada para funcionar.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-916">This feature requires the "Join Microsoft MAPS" setting enabled in order to function.</span></span> <span data-ttu-id="9ffcd-917">Os valores possíveis são: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-917">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="9ffcd-918">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="9ffcd-918">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="9ffcd-919">Int32</span><span class="sxs-lookup"><span data-stu-id="9ffcd-919">Int32</span></span>|<span data-ttu-id="9ffcd-920">Adicionado no Windows 10, versão 1709.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-920">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="9ffcd-921">Este recurso permite que o Windows Defender antivírus bloqueie um arquivo suspeito por até 60 segundos e examine-o na nuvem para garantir que ele seja seguro.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-921">This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe.</span></span> <span data-ttu-id="9ffcd-922">Tipo de valor é inteiro, intervalo é 0-50.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-922">Value type is integer, range is 0 - 50.</span></span> <span data-ttu-id="9ffcd-923">Esse recurso depende de três outras configurações de mapas que devem ser todos habilitadas-"Configure o bloqueio na primeira vista"; Ingresse no Microsoft MAPS "; "Enviar amostras de arquivo quando uma análise adicional é necessária".</span><span class="sxs-lookup"><span data-stu-id="9ffcd-923">This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required".</span></span> <span data-ttu-id="9ffcd-924">Valores válidos de 0 a 50</span><span class="sxs-lookup"><span data-stu-id="9ffcd-924">Valid values 0 to 50</span></span>|
|<span data-ttu-id="9ffcd-925">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="9ffcd-925">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="9ffcd-926">Int32</span><span class="sxs-lookup"><span data-stu-id="9ffcd-926">Int32</span></span>|<span data-ttu-id="9ffcd-927">Período de tempo (em dias) em que os itens de quarentena serão armazenados no sistema.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-927">Time period (in days) that quarantine items will be stored on the system.</span></span> <span data-ttu-id="9ffcd-928">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="9ffcd-928">Valid values 0 to 90</span></span>|
|<span data-ttu-id="9ffcd-929">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="9ffcd-929">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="9ffcd-930">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-930">Boolean</span></span>|<span data-ttu-id="9ffcd-931">Essa configuração de política permite configurar verificações de atualização para verificações completas agendadas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-931">This policy setting allows you to configure catch-up scans for scheduled full scans.</span></span> <span data-ttu-id="9ffcd-932">Uma verificação de atualização é uma verificação iniciada porque uma verificação agendada regularmente foi perdida.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-932">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="9ffcd-933">Normalmente, essas verificações agendadas são perdidas porque o computador foi desligado no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-933">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="9ffcd-934">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="9ffcd-934">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="9ffcd-935">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-935">Boolean</span></span>|<span data-ttu-id="9ffcd-936">Essa configuração de política permite que você configure verificações de atualização para verificações rápidas agendadas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-936">This policy setting allows you to configure catch-up scans for scheduled quick scans.</span></span> <span data-ttu-id="9ffcd-937">Uma verificação de atualização é uma verificação iniciada porque uma verificação agendada regularmente foi perdida.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-937">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="9ffcd-938">Normalmente, essas verificações agendadas são perdidas porque o computador foi desligado no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-938">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="9ffcd-939">defenderEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="9ffcd-939">defenderEnableLowCpuPriority</span></span>|<span data-ttu-id="9ffcd-940">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ffcd-940">Boolean</span></span>|<span data-ttu-id="9ffcd-941">Essa configuração de política permite habilitar ou desabilitar a baixa prioridade de CPU para verificações agendadas.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-941">This policy setting allows you to enable or disable low CPU priority for scheduled scans.</span></span>|
|<span data-ttu-id="9ffcd-942">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="9ffcd-942">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="9ffcd-943">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ffcd-943">String collection</span></span>|<span data-ttu-id="9ffcd-944">Extensões de arquivo a serem excluídas das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-944">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="9ffcd-945">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="9ffcd-945">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="9ffcd-946">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ffcd-946">String collection</span></span>|<span data-ttu-id="9ffcd-947">Arquivos e pastas a serem excluídos das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-947">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="9ffcd-948">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="9ffcd-948">defenderProcessesToExclude</span></span>|<span data-ttu-id="9ffcd-949">String collection</span><span class="sxs-lookup"><span data-stu-id="9ffcd-949">String collection</span></span>|<span data-ttu-id="9ffcd-950">Processos a serem excluídos das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-950">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="9ffcd-951">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="9ffcd-951">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="9ffcd-952">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-952">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9ffcd-953">Adicionado no Windows 10, versão 1607.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-953">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="9ffcd-954">Especifica o nível de detecção para aplicativos potencialmente indesejados (PUAs).</span><span class="sxs-lookup"><span data-stu-id="9ffcd-954">Specifies the level of detection for potentially unwanted applications (PUAs).</span></span> <span data-ttu-id="9ffcd-955">O Windows Defender alerta você quando um software potencialmente indesejado está sendo baixado ou tenta se instalar em seu computador.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-955">Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer.</span></span> <span data-ttu-id="9ffcd-956">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-956">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9ffcd-957">defenderScanDirection</span><span class="sxs-lookup"><span data-stu-id="9ffcd-957">defenderScanDirection</span></span>|[<span data-ttu-id="9ffcd-958">defenderRealtimeScanDirection</span><span class="sxs-lookup"><span data-stu-id="9ffcd-958">defenderRealtimeScanDirection</span></span>](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|<span data-ttu-id="9ffcd-959">Controla quais conjuntos de arquivos devem ser monitorados.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-959">Controls which sets of files should be monitored.</span></span> <span data-ttu-id="9ffcd-960">Os valores possíveis são: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-960">Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="9ffcd-961">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-961">defenderScanType</span></span>|[<span data-ttu-id="9ffcd-962">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-962">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="9ffcd-963">Seleciona se deseja executar uma verificação rápida ou uma verificação completa.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-963">Selects whether to perform a quick scan or full scan.</span></span> <span data-ttu-id="9ffcd-964">Os valores possíveis são: `userDefined`, `disabled`, `quick`, `full`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-964">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="9ffcd-965">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="9ffcd-965">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="9ffcd-966">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9ffcd-966">TimeOfDay</span></span>|<span data-ttu-id="9ffcd-967">Seleciona a hora do dia em que a verificação rápida do Windows Defender deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-967">Selects the time of day that the Windows Defender quick scan should run.</span></span> <span data-ttu-id="9ffcd-968">Por exemplo, um valor de 0 = 12:00AM, um valor de 60 = 1:00AM, um valor de 120 = 2:00 e assim por diante, até um valor de 1380 = 11:00PM.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-968">For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM.</span></span> <span data-ttu-id="9ffcd-969">O valor padrão é 120</span><span class="sxs-lookup"><span data-stu-id="9ffcd-969">The default value is 120</span></span>|
|<span data-ttu-id="9ffcd-970">defenderScheduledScanDay</span><span class="sxs-lookup"><span data-stu-id="9ffcd-970">defenderScheduledScanDay</span></span>|[<span data-ttu-id="9ffcd-971">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="9ffcd-971">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="9ffcd-972">Seleciona o dia em que a verificação do Windows Defender deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-972">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="9ffcd-973">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-973">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="9ffcd-974">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="9ffcd-974">defenderScheduledScanTime</span></span>|<span data-ttu-id="9ffcd-975">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9ffcd-975">TimeOfDay</span></span>|<span data-ttu-id="9ffcd-976">Seleciona a hora do dia em que a verificação do Windows Defender deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-976">Selects the time of day that the Windows Defender scan should run.</span></span>|
|<span data-ttu-id="9ffcd-977">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="9ffcd-977">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="9ffcd-978">Int32</span><span class="sxs-lookup"><span data-stu-id="9ffcd-978">Int32</span></span>|<span data-ttu-id="9ffcd-979">Especifica o intervalo (em horas) que será usado para verificar assinaturas, portanto, em vez de usar o ScheduleDay e Scheduletime, a verificação de novas assinaturas será definida de acordo com o intervalo.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-979">Specifies the interval (in hours) that will be used to check for signatures, so instead of using the ScheduleDay and ScheduleTime the check for new signatures will be set according to the interval.</span></span> <span data-ttu-id="9ffcd-980">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="9ffcd-980">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9ffcd-981">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-981">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="9ffcd-982">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="9ffcd-982">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="9ffcd-983">Verifica se o nível de consentimento do usuário no Windows Defender deve enviar dados.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-983">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="9ffcd-984">Os valores possíveis são: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-984">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="9ffcd-985">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="9ffcd-985">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="9ffcd-986">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="9ffcd-986">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="9ffcd-987">Permite que um administrador especifique quaisquer níveis de severidade de ameaças válidos e a ID de ação padrão correspondente a ser executada.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-987">Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.</span></span>|



## <a name="response"></a><span data-ttu-id="9ffcd-988">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ffcd-988">Response</span></span>
<span data-ttu-id="9ffcd-989">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-989">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ffcd-990">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ffcd-990">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ffcd-991">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ffcd-991">Request</span></span>
<span data-ttu-id="9ffcd-992">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-992">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 31005

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
  "defenderAllowScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderAllowBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderAllowCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderAllowScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderAllowScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderAllowIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderAllowOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderAllowRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderAllowScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderAllowScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderAllowEndUserAccess": true,
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
  "defenderSignatureUpdateIntervalInHours": 6,
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

### <a name="response"></a><span data-ttu-id="9ffcd-993">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ffcd-993">Response</span></span>
<span data-ttu-id="9ffcd-p225">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ffcd-p225">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 31177

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
  "defenderAllowScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderAllowBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderAllowCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderAllowScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderAllowScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderAllowIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderAllowOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderAllowRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderAllowScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderAllowScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderAllowEndUserAccess": true,
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
  "defenderSignatureUpdateIntervalInHours": 6,
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



