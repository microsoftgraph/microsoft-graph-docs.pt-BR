---
title: Criar windows10EndpointProtectionConfiguration
description: Criar um novo objeto windows10EndpointProtectionConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d87cd92f225f59325de87961c0cd477c1693e4a3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42740381"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="333df-103">Criar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="333df-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="333df-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="333df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="333df-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="333df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="333df-106">Criar um novo objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="333df-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="333df-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="333df-107">Prerequisites</span></span>
<span data-ttu-id="333df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="333df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="333df-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="333df-110">Permission type</span></span>|<span data-ttu-id="333df-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="333df-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="333df-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="333df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="333df-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="333df-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="333df-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="333df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="333df-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="333df-115">Not supported.</span></span>|
|<span data-ttu-id="333df-116">Application</span><span class="sxs-lookup"><span data-stu-id="333df-116">Application</span></span>|<span data-ttu-id="333df-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="333df-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="333df-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="333df-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="333df-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="333df-119">Request headers</span></span>
|<span data-ttu-id="333df-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="333df-120">Header</span></span>|<span data-ttu-id="333df-121">Valor</span><span class="sxs-lookup"><span data-stu-id="333df-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="333df-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="333df-122">Authorization</span></span>|<span data-ttu-id="333df-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="333df-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="333df-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="333df-124">Accept</span></span>|<span data-ttu-id="333df-125">application/json</span><span class="sxs-lookup"><span data-stu-id="333df-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="333df-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="333df-126">Request body</span></span>
<span data-ttu-id="333df-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="333df-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="333df-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="333df-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="333df-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="333df-129">Property</span></span>|<span data-ttu-id="333df-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="333df-130">Type</span></span>|<span data-ttu-id="333df-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="333df-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="333df-132">id</span><span class="sxs-lookup"><span data-stu-id="333df-132">id</span></span>|<span data-ttu-id="333df-133">String</span><span class="sxs-lookup"><span data-stu-id="333df-133">String</span></span>|<span data-ttu-id="333df-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="333df-134">Key of the entity.</span></span> <span data-ttu-id="333df-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="333df-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="333df-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="333df-136">lastModifiedDateTime</span></span>|<span data-ttu-id="333df-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="333df-137">DateTimeOffset</span></span>|<span data-ttu-id="333df-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="333df-138">DateTime the object was last modified.</span></span> <span data-ttu-id="333df-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="333df-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="333df-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="333df-140">roleScopeTagIds</span></span>|<span data-ttu-id="333df-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="333df-141">String collection</span></span>|<span data-ttu-id="333df-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="333df-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="333df-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="333df-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="333df-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="333df-144">supportsScopeTags</span></span>|<span data-ttu-id="333df-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-145">Boolean</span></span>|<span data-ttu-id="333df-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="333df-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="333df-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="333df-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="333df-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="333df-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="333df-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="333df-149">This property is read-only.</span></span> <span data-ttu-id="333df-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="333df-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="333df-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="333df-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="333df-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="333df-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="333df-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="333df-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="333df-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="333df-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="333df-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="333df-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="333df-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="333df-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="333df-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="333df-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="333df-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="333df-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="333df-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="333df-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="333df-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="333df-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="333df-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="333df-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="333df-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="333df-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="333df-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="333df-163">createdDateTime</span></span>|<span data-ttu-id="333df-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="333df-164">DateTimeOffset</span></span>|<span data-ttu-id="333df-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="333df-165">DateTime the object was created.</span></span> <span data-ttu-id="333df-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="333df-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="333df-167">description</span><span class="sxs-lookup"><span data-stu-id="333df-167">description</span></span>|<span data-ttu-id="333df-168">String</span><span class="sxs-lookup"><span data-stu-id="333df-168">String</span></span>|<span data-ttu-id="333df-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="333df-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="333df-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="333df-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="333df-171">displayName</span><span class="sxs-lookup"><span data-stu-id="333df-171">displayName</span></span>|<span data-ttu-id="333df-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="333df-172">String</span></span>|<span data-ttu-id="333df-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="333df-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="333df-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="333df-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="333df-175">versão</span><span class="sxs-lookup"><span data-stu-id="333df-175">version</span></span>|<span data-ttu-id="333df-176">Int32</span><span class="sxs-lookup"><span data-stu-id="333df-176">Int32</span></span>|<span data-ttu-id="333df-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="333df-177">Version of the device configuration.</span></span> <span data-ttu-id="333df-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="333df-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="333df-179">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="333df-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="333df-180">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="333df-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="333df-181">Essa política destina-se a fornecer segurança adicional contra dispositivos compatíveis com DMA externo.</span><span class="sxs-lookup"><span data-stu-id="333df-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="333df-182">Permite mais controle sobre a enumeração de dispositivos compatíveis com DMA externo incompatíveis com o remapeamento de DMA/isolamento de memória do dispositivo e área restrita.</span><span class="sxs-lookup"><span data-stu-id="333df-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="333df-183">Essa política só entra em vigor quando a proteção DMA de kernel é suportada e habilitada pelo firmware do sistema.</span><span class="sxs-lookup"><span data-stu-id="333df-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="333df-184">A proteção DMA de kernel é um recurso de plataforma que não pode ser controlado via política ou pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="333df-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="333df-185">É preciso ter suporte do sistema no momento da fabricação.</span><span class="sxs-lookup"><span data-stu-id="333df-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="333df-186">Para verificar se o sistema suporta a proteção DMA de kernel, verifique o campo proteção DMA de kernel na página Resumo de MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="333df-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="333df-187">Os valores possíveis são: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="333df-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="333df-188">firewallRules</span><span class="sxs-lookup"><span data-stu-id="333df-188">firewallRules</span></span>|<span data-ttu-id="333df-189">coleção [windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="333df-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="333df-190">Define as configurações da regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="333df-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="333df-191">Essa coleção pode conter um máximo de 150 elementos.</span><span class="sxs-lookup"><span data-stu-id="333df-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="333df-192">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="333df-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="333df-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-194">Esse direito de usuário é usado pelo Gerenciador de credenciais durante o backup/restauração.</span><span class="sxs-lookup"><span data-stu-id="333df-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="333df-195">As credenciais salvas dos usuários podem ser comprometidas se esse privilégio for dado a outras entidades.</span><span class="sxs-lookup"><span data-stu-id="333df-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="333df-196">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="333df-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="333df-197">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="333df-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="333df-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-199">Esse direito de usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="333df-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="333df-200">O estado permitido é suportado.</span><span class="sxs-lookup"><span data-stu-id="333df-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="333df-201">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="333df-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="333df-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-203">Esse direito de usuário determina quais usuários e grupos são bloqueados para se conectarem ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="333df-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="333df-204">Há suporte para o bloco de estado.</span><span class="sxs-lookup"><span data-stu-id="333df-204">State Block is supported.</span></span>|
|<span data-ttu-id="333df-205">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="333df-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="333df-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-207">Esse direito de usuário permite que um processo represente qualquer usuário sem autenticação.</span><span class="sxs-lookup"><span data-stu-id="333df-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="333df-208">Portanto, o processo pode ter acesso aos mesmos recursos locais que esse usuário.</span><span class="sxs-lookup"><span data-stu-id="333df-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="333df-209">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="333df-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="333df-210">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="333df-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="333df-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-212">Esse direito de usuário determina quais usuários podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="333df-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="333df-213">Estados não configurados, permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="333df-213">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="333df-214">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="333df-214">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="333df-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-216">Esse direito de usuário determina quais usuários não podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="333df-216">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="333df-217">Estados não configurados, bloqueados são suportados</span><span class="sxs-lookup"><span data-stu-id="333df-217">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="333df-218">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="333df-218">userRightsBackupData</span></span>|[<span data-ttu-id="333df-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-220">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao fazer backup de arquivos e diretórios.</span><span class="sxs-lookup"><span data-stu-id="333df-220">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="333df-221">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="333df-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="333df-222">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="333df-222">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="333df-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-224">Este direito de usuário determina quais usuários e grupos podem alterar a hora e a data no relógio interno do computador.</span><span class="sxs-lookup"><span data-stu-id="333df-224">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="333df-225">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="333df-225">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="333df-226">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="333df-226">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="333df-227">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-227">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-228">Configuração de segurança que determina se os usuários podem criar objetos globais que estão disponíveis para todas as sessões.</span><span class="sxs-lookup"><span data-stu-id="333df-228">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="333df-229">Os usuários que podem criar objetos globais podem afetar processos executados em sessões de outros usuários, o que pode levar a falhas de aplicativos ou corrupção de dados.</span><span class="sxs-lookup"><span data-stu-id="333df-229">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="333df-230">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="333df-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="333df-231">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="333df-231">userRightsCreatePageFile</span></span>|[<span data-ttu-id="333df-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-233">Esse direito de usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de paginação.</span><span class="sxs-lookup"><span data-stu-id="333df-233">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="333df-234">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="333df-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="333df-235">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="333df-235">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="333df-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-237">Este direito de usuário determina quais contas podem ser usadas por processos para criar um objeto de diretório usando o Gerenciador de objetos.</span><span class="sxs-lookup"><span data-stu-id="333df-237">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="333df-238">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="333df-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="333df-239">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="333df-239">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="333df-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-241">Esse direito de usuário determina se o usuário pode criar um link simbólico do computador no qual está conectado.</span><span class="sxs-lookup"><span data-stu-id="333df-241">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="333df-242">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="333df-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="333df-243">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="333df-243">userRightsCreateToken</span></span>|[<span data-ttu-id="333df-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-245">Esse direito de usuário determina quais usuários/grupos podem ser usados por processos para criar um token que pode ser usado para obter acesso a qualquer recurso local quando o processo usa uma API interna para criar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="333df-245">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="333df-246">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="333df-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="333df-247">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="333df-247">userRightsDebugPrograms</span></span>|[<span data-ttu-id="333df-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-249">Esse direito de usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel.</span><span class="sxs-lookup"><span data-stu-id="333df-249">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="333df-250">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="333df-250">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="333df-251">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="333df-251">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="333df-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-253">Este direito de usuário determina quais usuários e grupos estão proibidos de fazer logon como um cliente de serviços de área de trabalho remota.</span><span class="sxs-lookup"><span data-stu-id="333df-253">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="333df-254">Há suporte apenas para os Estados não configurados e bloqueados</span><span class="sxs-lookup"><span data-stu-id="333df-254">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="333df-255">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="333df-255">userRightsDelegation</span></span>|[<span data-ttu-id="333df-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-257">Este direito de usuário determina quais usuários podem definir a configuração confiável para delegação em um objeto de usuário ou computador.</span><span class="sxs-lookup"><span data-stu-id="333df-257">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="333df-258">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-258">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-259">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="333df-259">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="333df-260">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-260">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-261">Este direito de usuário determina quais contas podem ser usadas por um processo para adicionar entradas ao log de segurança.</span><span class="sxs-lookup"><span data-stu-id="333df-261">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="333df-262">O log de segurança é usado para rastrear o acesso de sistema não autorizado.</span><span class="sxs-lookup"><span data-stu-id="333df-262">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="333df-263">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-263">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-264">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="333df-264">userRightsImpersonateClient</span></span>|[<span data-ttu-id="333df-265">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-265">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-266">A atribuição desse direito de usuário a um usuário permite que programas executados em nome desse usuário representem um cliente.</span><span class="sxs-lookup"><span data-stu-id="333df-266">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="333df-267">A exigência desse direito de usuário para esse tipo de representação impede que um usuário não autorizado convença um cliente a se conectar a um serviço que ele criou e, em seguida, representando esse cliente, o que pode elevar as permissões do usuário não autorizado para níveis administrativos ou de sistema.</span><span class="sxs-lookup"><span data-stu-id="333df-267">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="333df-268">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-269">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="333df-269">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="333df-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-271">Este direito de usuário determina quais contas podem usar um processo com acesso de propriedade de gravação a outro processo para aumentar a prioridade de execução atribuída ao outro processo.</span><span class="sxs-lookup"><span data-stu-id="333df-271">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="333df-272">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-273">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="333df-273">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="333df-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-275">Esse direito de usuário determina quais usuários podem carregar e descarregar dinamicamente drivers de dispositivo ou outro código no modo kernel.</span><span class="sxs-lookup"><span data-stu-id="333df-275">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="333df-276">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-277">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="333df-277">userRightsLockMemory</span></span>|[<span data-ttu-id="333df-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-279">Esse direito de usuário determina quais contas podem usar um processo para manter os dados na memória física, o que impede que o sistema pagine os dados para a memória virtual em disco.</span><span class="sxs-lookup"><span data-stu-id="333df-279">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="333df-280">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-281">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="333df-281">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="333df-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-283">Esse direito de usuário determina quais usuários podem especificar opções de auditoria de acesso a objetos para recursos individuais, como arquivos, objetos do Active Directory e chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="333df-283">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="333df-284">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-285">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="333df-285">userRightsManageVolumes</span></span>|[<span data-ttu-id="333df-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-287">Esse direito de usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como a desfragmentação remota.</span><span class="sxs-lookup"><span data-stu-id="333df-287">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="333df-288">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-289">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="333df-289">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="333df-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-291">Esse direito de usuário determina quem pode modificar os valores de ambiente de firmware.</span><span class="sxs-lookup"><span data-stu-id="333df-291">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="333df-292">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-293">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="333df-293">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="333df-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-295">Este direito de usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves de registro ou processos pertencentes a outros usuários.</span><span class="sxs-lookup"><span data-stu-id="333df-295">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="333df-296">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-297">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="333df-297">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="333df-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-299">Esse direito de usuário determina quais usuários podem usar ferramentas de monitoramento de desempenho para monitorar o desempenho de processos do sistema.</span><span class="sxs-lookup"><span data-stu-id="333df-299">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="333df-300">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-300">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-301">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="333df-301">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="333df-302">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-302">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-303">Esse direito de usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede.</span><span class="sxs-lookup"><span data-stu-id="333df-303">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="333df-304">O mau uso desse direito de usuário pode resultar em uma negação de serviço.</span><span class="sxs-lookup"><span data-stu-id="333df-304">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="333df-305">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-306">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="333df-306">userRightsRestoreData</span></span>|[<span data-ttu-id="333df-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-308">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao restaurar backups de arquivos e diretórios e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto.</span><span class="sxs-lookup"><span data-stu-id="333df-308">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="333df-309">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-310">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="333df-310">userRightsTakeOwnership</span></span>|[<span data-ttu-id="333df-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="333df-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="333df-312">Esse direito de usuário determina quais usuários podem assumir a propriedade de qualquer objeto protegível no sistema, incluindo objetos do Active Directory, arquivos e pastas, impressoras, chaves do registro, processos e threads.</span><span class="sxs-lookup"><span data-stu-id="333df-312">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="333df-313">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="333df-313">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="333df-314">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="333df-314">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="333df-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-315">Boolean</span></span>|<span data-ttu-id="333df-316">Essa configuração determina se o salvamento de jogos do Xbox está habilitado (1) ou desabilitado (0).</span><span class="sxs-lookup"><span data-stu-id="333df-316">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="333df-317">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="333df-317">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="333df-318">instarttype</span><span class="sxs-lookup"><span data-stu-id="333df-318">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="333df-319">Esta configuração determina se o tipo de início do serviço de gerenciamento de acessórios é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="333df-319">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="333df-320">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="333df-320">Default: Manual.</span></span> <span data-ttu-id="333df-321">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="333df-321">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="333df-322">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="333df-322">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="333df-323">instarttype</span><span class="sxs-lookup"><span data-stu-id="333df-323">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="333df-324">Essa configuração determina se o tipo de início do serviço do Live Authentication Manager é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="333df-324">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="333df-325">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="333df-325">Default: Manual.</span></span> <span data-ttu-id="333df-326">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="333df-326">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="333df-327">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="333df-327">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="333df-328">instarttype</span><span class="sxs-lookup"><span data-stu-id="333df-328">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="333df-329">Essa configuração determina se o tipo de início do serviço de salvamento do Live Game é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="333df-329">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="333df-330">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="333df-330">Default: Manual.</span></span> <span data-ttu-id="333df-331">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="333df-331">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="333df-332">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="333df-332">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="333df-333">instarttype</span><span class="sxs-lookup"><span data-stu-id="333df-333">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="333df-334">Esta configuração determina se o tipo de início do serviço de rede é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="333df-334">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="333df-335">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="333df-335">Default: Manual.</span></span> <span data-ttu-id="333df-336">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="333df-336">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="333df-337">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="333df-337">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="333df-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-338">Boolean</span></span>|<span data-ttu-id="333df-339">Impedir que os usuários adicionem novas contas da Microsoft a este computador.</span><span class="sxs-lookup"><span data-stu-id="333df-339">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="333df-340">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="333df-340">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="333df-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-341">Boolean</span></span>|<span data-ttu-id="333df-342">Habilitar contas locais que não estão protegidas por senha para fazer logon de locais diferentes do dispositivo físico. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="333df-342">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="333df-343">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="333df-343">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="333df-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-344">Boolean</span></span>|<span data-ttu-id="333df-345">Determina se a conta de administrador local está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="333df-345">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="333df-346">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="333df-346">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="333df-347">String</span><span class="sxs-lookup"><span data-stu-id="333df-347">String</span></span>|<span data-ttu-id="333df-348">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "administrador".</span><span class="sxs-lookup"><span data-stu-id="333df-348">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="333df-349">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="333df-349">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="333df-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-350">Boolean</span></span>|<span data-ttu-id="333df-351">Determina se a conta de convidado está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="333df-351">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="333df-352">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="333df-352">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="333df-353">String</span><span class="sxs-lookup"><span data-stu-id="333df-353">String</span></span>|<span data-ttu-id="333df-354">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "convidado".</span><span class="sxs-lookup"><span data-stu-id="333df-354">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="333df-355">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="333df-355">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="333df-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-356">Boolean</span></span>|<span data-ttu-id="333df-357">Impedir que um computador portátil seja desencaixado sem ter que fazer logon.</span><span class="sxs-lookup"><span data-stu-id="333df-357">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="333df-358">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="333df-358">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="333df-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-359">Boolean</span></span>|<span data-ttu-id="333df-360">Restringir a instalação dos drivers de impressora como parte da conexão a uma impressora compartilhada somente para administradores.</span><span class="sxs-lookup"><span data-stu-id="333df-360">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="333df-361">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="333df-361">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="333df-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-362">Boolean</span></span>|<span data-ttu-id="333df-363">Habilitar essa configuração permite que somente o usuário conectado interativamente acesse a mídia de CD-ROM.</span><span class="sxs-lookup"><span data-stu-id="333df-363">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="333df-364">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="333df-364">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="333df-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="333df-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="333df-366">Defina quem tem permissão para formatar e ejetar a mídia NTFS removível.</span><span class="sxs-lookup"><span data-stu-id="333df-366">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="333df-367">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="333df-367">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="333df-368">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="333df-368">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="333df-369">Int32</span><span class="sxs-lookup"><span data-stu-id="333df-369">Int32</span></span>|<span data-ttu-id="333df-370">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="333df-370">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="333df-371">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="333df-371">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="333df-372">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="333df-372">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="333df-373">Int32</span><span class="sxs-lookup"><span data-stu-id="333df-373">Int32</span></span>|<span data-ttu-id="333df-374">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="333df-374">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="333df-375">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="333df-375">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="333df-376">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="333df-376">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="333df-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-377">Boolean</span></span>|<span data-ttu-id="333df-378">Exigir CTRL + ALT + DEL para ser pressionada para que um usuário possa fazer logon.</span><span class="sxs-lookup"><span data-stu-id="333df-378">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="333df-379">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="333df-379">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="333df-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-380">Boolean</span></span>|<span data-ttu-id="333df-381">Não exibe o nome de usuário da última pessoa que entrou neste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="333df-381">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="333df-382">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="333df-382">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="333df-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-383">Boolean</span></span>|<span data-ttu-id="333df-384">Não exibe o nome de usuário da pessoa que está entrando neste dispositivo depois que as credenciais são inseridas e antes da área de trabalho do dispositivo ser exibida.</span><span class="sxs-lookup"><span data-stu-id="333df-384">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="333df-385">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="333df-385">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="333df-386">String</span><span class="sxs-lookup"><span data-stu-id="333df-386">String</span></span>|<span data-ttu-id="333df-387">Defina o título da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="333df-387">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="333df-388">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="333df-388">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="333df-389">String</span><span class="sxs-lookup"><span data-stu-id="333df-389">String</span></span>|<span data-ttu-id="333df-390">Definir o texto da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="333df-390">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="333df-391">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="333df-391">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="333df-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-392">Boolean</span></span>|<span data-ttu-id="333df-393">Bloquear solicitações de autenticação PKU2U para este dispositivo para usar identidades online.</span><span class="sxs-lookup"><span data-stu-id="333df-393">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="333df-394">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="333df-394">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="333df-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-395">Boolean</span></span>|<span data-ttu-id="333df-396">Boolean do auxiliar da interface do usuário para entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="333df-396">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="333df-397">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="333df-397">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="333df-398">String</span><span class="sxs-lookup"><span data-stu-id="333df-398">String</span></span>|<span data-ttu-id="333df-399">Edite a cadeia de caracteres de definição de descritor de segurança padrão para permitir ou impedir que usuários e grupos façam chamadas remotas para o SAM.</span><span class="sxs-lookup"><span data-stu-id="333df-399">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="333df-400">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="333df-400">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="333df-401">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="333df-401">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="333df-402">Essa configuração de segurança permite que um cliente exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="333df-402">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="333df-403">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="333df-403">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="333df-404">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="333df-404">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="333df-405">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="333df-405">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="333df-406">Essa configuração de segurança permite que um servidor exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="333df-406">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="333df-407">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="333df-407">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="333df-408">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="333df-408">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="333df-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="333df-409">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="333df-410">Essa configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede.</span><span class="sxs-lookup"><span data-stu-id="333df-410">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="333df-411">Os possíveis valores são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="333df-411">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="333df-412">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="333df-412">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="333df-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-413">Boolean</span></span>|<span data-ttu-id="333df-414">Se for habilitada, o cliente SMB permitirá logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="333df-414">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="333df-415">Se não configurada, o cliente SMB rejeitará logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="333df-415">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="333df-416">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="333df-416">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="333df-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-417">Boolean</span></span>|<span data-ttu-id="333df-418">Configuração de segurança que determina se o arquivo de paginação de memória virtual será limpo quando o sistema for desligado.</span><span class="sxs-lookup"><span data-stu-id="333df-418">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="333df-419">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="333df-419">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="333df-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-420">Boolean</span></span>|<span data-ttu-id="333df-421">Configuração de segurança que determina se um computador pode ser desligado sem a necessidade de fazer logon no Windows.</span><span class="sxs-lookup"><span data-stu-id="333df-421">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="333df-422">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="333df-422">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="333df-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-423">Boolean</span></span>|<span data-ttu-id="333df-424">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="333df-424">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="333df-425">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="333df-425">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="333df-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-426">Boolean</span></span>|<span data-ttu-id="333df-427">Virtualizar falhas de gravação de arquivo e registro para locais por usuário</span><span class="sxs-lookup"><span data-stu-id="333df-427">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="333df-428">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="333df-428">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="333df-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-429">Boolean</span></span>|<span data-ttu-id="333df-430">Impor a validação de caminho de certificação PKI para um determinado arquivo executável antes que seja permitido executar.</span><span class="sxs-lookup"><span data-stu-id="333df-430">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="333df-431">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="333df-431">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="333df-432">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="333df-432">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="333df-433">Definir o comportamento do prompt de elevação para administradores no modo de aprovação de administrador.</span><span class="sxs-lookup"><span data-stu-id="333df-433">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="333df-434">Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="333df-434">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="333df-435">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="333df-435">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="333df-436">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="333df-436">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="333df-437">Definir o comportamento do prompt de elevação para usuários padrão.</span><span class="sxs-lookup"><span data-stu-id="333df-437">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="333df-438">Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="333df-438">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="333df-439">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="333df-439">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="333df-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-440">Boolean</span></span>|<span data-ttu-id="333df-441">Habilite todas as solicitações de elevação para ir para a área de trabalho do usuário interativo, e não para a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="333df-441">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="333df-442">As configurações de política de comportamento de prompt para administradores e usuários padrão são usadas.</span><span class="sxs-lookup"><span data-stu-id="333df-442">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="333df-443">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="333df-443">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="333df-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-444">Boolean</span></span>|<span data-ttu-id="333df-445">Instalações de aplicativos que exigem privilégios elevados solicitarão credenciais de administrador. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="333df-445">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="333df-446">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="333df-446">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="333df-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-447">Boolean</span></span>|<span data-ttu-id="333df-448">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="333df-448">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="333df-449">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="333df-449">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="333df-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-450">Boolean</span></span>|<span data-ttu-id="333df-451">Define se a conta de administrador interna usa o modo de aprovação de administrador ou executa todos os aplicativos com privilégios de administrador completo. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="333df-451">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="333df-452">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="333df-452">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="333df-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-453">Boolean</span></span>|<span data-ttu-id="333df-454">Definir se o modo de aprovação de administrador e todas as configurações de política de UAC estão habilitados, o padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="333df-454">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="333df-455">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="333df-455">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="333df-456">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="333df-456">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="333df-457">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="333df-457">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="333df-458">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="333df-458">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="333df-459">Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="333df-459">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="333df-460">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="333df-460">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="333df-461">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="333df-461">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="333df-462">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="333df-462">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="333df-463">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="333df-463">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="333df-464">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="333df-464">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="333df-465">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="333df-465">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="333df-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-466">Boolean</span></span>|<span data-ttu-id="333df-467">Configuração de segurança que determina se o cliente SMB tentará negociar assinatura de pacote SMB.</span><span class="sxs-lookup"><span data-stu-id="333df-467">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="333df-468">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="333df-468">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="333df-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-469">Boolean</span></span>|<span data-ttu-id="333df-470">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do cliente SMB.</span><span class="sxs-lookup"><span data-stu-id="333df-470">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="333df-471">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="333df-471">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="333df-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-472">Boolean</span></span>|<span data-ttu-id="333df-473">Se essa configuração de segurança estiver habilitada, o redirecionador de bloco de mensagens de servidor (SMB) terá permissão para enviar senhas de texto não criptografado para servidores SMB não Microsoft que não ofereçam suporte à criptografia de senha durante a autenticação.</span><span class="sxs-lookup"><span data-stu-id="333df-473">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="333df-474">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="333df-474">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="333df-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-475">Boolean</span></span>|<span data-ttu-id="333df-476">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do servidor SMB.</span><span class="sxs-lookup"><span data-stu-id="333df-476">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="333df-477">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="333df-477">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="333df-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-478">Boolean</span></span>|<span data-ttu-id="333df-479">Configuração de segurança que determina se o servidor SMB negociará assinatura de pacote SMB com clientes que solicitarem.</span><span class="sxs-lookup"><span data-stu-id="333df-479">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="333df-480">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="333df-480">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="333df-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-481">Boolean</span></span>|<span data-ttu-id="333df-482">Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e pipes para as configurações de pipes nomeados que podem ser acessados anonimamente e compartilhamentos que podem ser acessados anonimamente</span><span class="sxs-lookup"><span data-stu-id="333df-482">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="333df-483">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="333df-483">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="333df-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-484">Boolean</span></span>|<span data-ttu-id="333df-485">Essa configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas com o computador.</span><span class="sxs-lookup"><span data-stu-id="333df-485">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="333df-486">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="333df-486">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="333df-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-487">Boolean</span></span>|<span data-ttu-id="333df-488">Configuração de segurança que determina se os usuários anônimos devem executar determinadas atividades, como enumeração de nomes de contas de domínio e compartilhamentos de rede.</span><span class="sxs-lookup"><span data-stu-id="333df-488">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="333df-489">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="333df-489">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="333df-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-490">Boolean</span></span>|<span data-ttu-id="333df-491">Essa configuração de segurança determina se, na próxima alteração de senha, o valor de hash do LM (LAN Manager) para a nova senha é armazenado.</span><span class="sxs-lookup"><span data-stu-id="333df-491">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="333df-492">Ele não é armazenado por padrão.</span><span class="sxs-lookup"><span data-stu-id="333df-492">It’s not stored by default.</span></span>|
|<span data-ttu-id="333df-493">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="333df-493">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="333df-494">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="333df-494">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="333df-495">Essa configuração de segurança determina o que acontece quando o cartão inteligente de um usuário conectado é removido do leitor de cartão inteligente.</span><span class="sxs-lookup"><span data-stu-id="333df-495">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="333df-496">Os valores possíveis são: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="333df-496">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="333df-497">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="333df-497">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="333df-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-498">Boolean</span></span>|<span data-ttu-id="333df-499">Usado para desabilitar a exibição da área de proteção de aplicativo e navegador.</span><span class="sxs-lookup"><span data-stu-id="333df-499">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="333df-500">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="333df-500">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="333df-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-501">Boolean</span></span>|<span data-ttu-id="333df-502">Usado para desabilitar a exibição da área de opções da família.</span><span class="sxs-lookup"><span data-stu-id="333df-502">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="333df-503">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="333df-503">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="333df-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-504">Boolean</span></span>|<span data-ttu-id="333df-505">Usado para desabilitar a exibição da área de desempenho e integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="333df-505">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="333df-506">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="333df-506">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="333df-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-507">Boolean</span></span>|<span data-ttu-id="333df-508">Usado para desabilitar a exibição da área de firewall e proteção de rede.</span><span class="sxs-lookup"><span data-stu-id="333df-508">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="333df-509">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="333df-509">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="333df-510">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-510">Boolean</span></span>|<span data-ttu-id="333df-511">Usado para desabilitar a exibição da área de proteção contra vírus e ameaças.</span><span class="sxs-lookup"><span data-stu-id="333df-511">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="333df-512">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="333df-512">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="333df-513">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-513">Boolean</span></span>|<span data-ttu-id="333df-514">Usado para desabilitar a exibição da área de proteção da conta.</span><span class="sxs-lookup"><span data-stu-id="333df-514">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="333df-515">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="333df-515">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="333df-516">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-516">Boolean</span></span>|<span data-ttu-id="333df-517">Usado para desabilitar a exibição do botão limpar TPM.</span><span class="sxs-lookup"><span data-stu-id="333df-517">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="333df-518">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="333df-518">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="333df-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-519">Boolean</span></span>|<span data-ttu-id="333df-520">Usado para desabilitar a exibição da área de proteção de hardware.</span><span class="sxs-lookup"><span data-stu-id="333df-520">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="333df-521">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="333df-521">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="333df-522">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-522">Boolean</span></span>|<span data-ttu-id="333df-523">Usado para desabilitar a exibição do controle da área de notificação.</span><span class="sxs-lookup"><span data-stu-id="333df-523">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="333df-524">O usuário precisa sair e entrar ou reiniciar o computador para que essa configuração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="333df-524">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="333df-525">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="333df-525">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="333df-526">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-526">Boolean</span></span>|<span data-ttu-id="333df-527">Usado para desabilitar a exibição da área de proteção contra ransomware.</span><span class="sxs-lookup"><span data-stu-id="333df-527">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="333df-528">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="333df-528">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="333df-529">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-529">Boolean</span></span>|<span data-ttu-id="333df-530">Usado para desabilitar a exibição da área de inicialização segura sob segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="333df-530">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="333df-531">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="333df-531">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="333df-532">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-532">Boolean</span></span>|<span data-ttu-id="333df-533">Usado para desabilitar a exibição do processo de segurança Solucionando problemas de segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="333df-533">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="333df-534">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="333df-534">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="333df-535">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-535">Boolean</span></span>|<span data-ttu-id="333df-536">Usado para desabilitar a exibição de atualizar o firmware do TPM quando um firmware vulnerável é detectado.</span><span class="sxs-lookup"><span data-stu-id="333df-536">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="333df-537">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="333df-537">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="333df-538">String</span><span class="sxs-lookup"><span data-stu-id="333df-538">String</span></span>|<span data-ttu-id="333df-539">O nome da empresa que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="333df-539">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="333df-540">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="333df-540">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="333df-541">String</span><span class="sxs-lookup"><span data-stu-id="333df-541">String</span></span>|<span data-ttu-id="333df-542">O endereço de email que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="333df-542">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="333df-543">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="333df-543">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="333df-544">String</span><span class="sxs-lookup"><span data-stu-id="333df-544">String</span></span>|<span data-ttu-id="333df-545">O número de telefone ou Skype ID que é exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="333df-545">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="333df-546">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="333df-546">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="333df-547">String</span><span class="sxs-lookup"><span data-stu-id="333df-547">String</span></span>|<span data-ttu-id="333df-548">A URL do portal da ajuda que é exibida para os usuários.</span><span class="sxs-lookup"><span data-stu-id="333df-548">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="333df-549">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="333df-549">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="333df-550">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="333df-550">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="333df-551">Notificações para mostrar das áreas de aplicativo exibidas.</span><span class="sxs-lookup"><span data-stu-id="333df-551">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="333df-552">Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="333df-552">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="333df-553">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="333df-553">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="333df-554">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="333df-554">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="333df-555">Configurar onde exibir informações de contato de ti para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="333df-555">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="333df-556">Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="333df-556">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="333df-557">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="333df-557">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="333df-558">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="333df-558">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="333df-559">Defina as configurações do Windows Defender TamperProtection.</span><span class="sxs-lookup"><span data-stu-id="333df-559">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="333df-560">Os valores possíveis são: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="333df-560">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="333df-561">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="333df-561">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="333df-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-562">Boolean</span></span>|<span data-ttu-id="333df-563">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="333df-563">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="333df-564">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="333df-564">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="333df-565">Int32</span><span class="sxs-lookup"><span data-stu-id="333df-565">Int32</span></span>|<span data-ttu-id="333df-566">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="333df-566">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="333df-567">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="333df-567">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="333df-568">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="333df-568">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="333df-569">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="333df-569">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="333df-570">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="333df-570">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="333df-571">Selecione a codificação de chave pré-compartilhada a ser usada.</span><span class="sxs-lookup"><span data-stu-id="333df-571">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="333df-572">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="333df-572">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="333df-573">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="333df-573">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="333df-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-574">Boolean</span></span>|<span data-ttu-id="333df-575">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="333df-575">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="333df-576">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="333df-576">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="333df-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-577">Boolean</span></span>|<span data-ttu-id="333df-578">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="333df-578">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="333df-579">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="333df-579">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="333df-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-580">Boolean</span></span>|<span data-ttu-id="333df-581">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="333df-581">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="333df-582">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="333df-582">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="333df-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-583">Boolean</span></span>|<span data-ttu-id="333df-584">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="333df-584">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="333df-585">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="333df-585">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="333df-586">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="333df-586">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="333df-587">Especifique como a lista de certificados revogados será imposta.</span><span class="sxs-lookup"><span data-stu-id="333df-587">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="333df-588">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="333df-588">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="333df-589">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="333df-589">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="333df-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-590">Boolean</span></span>|<span data-ttu-id="333df-591">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="333df-591">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="333df-592">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="333df-592">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="333df-593">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="333df-593">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="333df-594">Configura como o enfileiramento de pacotes deve ser aplicado no cenário de gateway de túnel.</span><span class="sxs-lookup"><span data-stu-id="333df-594">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="333df-595">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="333df-595">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="333df-596">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="333df-596">firewallProfileDomain</span></span>|[<span data-ttu-id="333df-597">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="333df-597">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="333df-598">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="333df-598">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="333df-599">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="333df-599">firewallProfilePublic</span></span>|[<span data-ttu-id="333df-600">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="333df-600">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="333df-601">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="333df-601">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="333df-602">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="333df-602">firewallProfilePrivate</span></span>|[<span data-ttu-id="333df-603">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="333df-603">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="333df-604">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="333df-604">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="333df-605">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="333df-605">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="333df-606">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-606">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-607">O valor que indica o comportamento do Adobe Reader de criar processos filhos.</span><span class="sxs-lookup"><span data-stu-id="333df-607">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="333df-608">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-608">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-609">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="333df-609">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="333df-610">String collection</span><span class="sxs-lookup"><span data-stu-id="333df-610">String collection</span></span>|<span data-ttu-id="333df-611">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="333df-611">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="333df-612">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="333df-612">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="333df-613">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="333df-613">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="333df-614">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="333df-614">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="333df-615">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-615">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-616">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="333df-616">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="333df-617">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-617">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-618">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="333df-618">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="333df-619">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-619">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-620">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="333df-620">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="333df-621">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-621">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-622">O valor que indica o comportamento dos aplicativos de comunicação do Office, incluindo o Microsoft Outlook, da criação de processos filhos.</span><span class="sxs-lookup"><span data-stu-id="333df-622">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="333df-623">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-623">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-624">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="333df-624">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="333df-625">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="333df-625">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="333df-626">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="333df-626">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="333df-627">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-627">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-628">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="333df-628">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="333df-629">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-629">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-630">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="333df-630">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="333df-631">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-631">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-632">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="333df-632">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="333df-633">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="333df-633">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="333df-634">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="333df-634">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="333df-635">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-635">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-636">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="333df-636">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="333df-637">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-637">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-638">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="333df-638">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="333df-639">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-639">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-640">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="333df-640">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="333df-641">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="333df-641">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="333df-642">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="333df-642">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="333df-643">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-643">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-644">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="333df-644">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="333df-645">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-645">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-646">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="333df-646">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="333df-647">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-647">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-648">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="333df-648">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="333df-649">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="333df-649">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="333df-650">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="333df-650">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="333df-651">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-651">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-652">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="333df-652">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="333df-653">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-653">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-654">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="333df-654">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="333df-655">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-655">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-656">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="333df-656">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="333df-657">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="333df-657">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="333df-658">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="333df-658">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="333df-659">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-659">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-660">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="333df-660">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="333df-661">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-661">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-662">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="333df-662">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="333df-663">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-663">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-664">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="333df-664">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="333df-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-666">Valor que indica se a credencial que está sendo roubada do subsistema de autoridade de segurança local do Windows é permitida.</span><span class="sxs-lookup"><span data-stu-id="333df-666">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="333df-667">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-667">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-668">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="333df-668">defenderProcessCreationType</span></span>|[<span data-ttu-id="333df-669">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="333df-669">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="333df-670">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="333df-670">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="333df-671">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-671">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-672">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="333df-672">defenderProcessCreation</span></span>|[<span data-ttu-id="333df-673">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-673">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-674">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="333df-674">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="333df-675">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-675">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-676">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="333df-676">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="333df-677">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="333df-677">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="333df-678">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="333df-678">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="333df-679">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-679">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-680">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="333df-680">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="333df-681">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-681">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-682">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="333df-682">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="333df-683">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-683">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-684">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="333df-684">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="333df-685">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="333df-685">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="333df-686">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="333df-686">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="333df-687">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-687">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-688">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="333df-688">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="333df-689">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-689">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-690">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="333df-690">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="333df-691">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-691">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-692">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="333df-692">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="333df-693">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="333df-693">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="333df-694">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="333df-694">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="333df-695">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-695">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-696">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="333df-696">defenderEmailContentExecution</span></span>|[<span data-ttu-id="333df-697">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-697">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-698">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="333df-698">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="333df-699">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-699">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-700">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-700">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="333df-701">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-701">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-702">O valor que indica o uso da proteção avançada contra o Ransomeware.</span><span class="sxs-lookup"><span data-stu-id="333df-702">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="333df-703">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-703">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-704">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="333df-704">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="333df-705">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-705">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="333df-706">Valor que indica o comportamento das pastas protegidas.</span><span class="sxs-lookup"><span data-stu-id="333df-706">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="333df-707">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="333df-707">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="333df-708">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="333df-708">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="333df-709">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="333df-709">String collection</span></span>|<span data-ttu-id="333df-710">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="333df-710">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="333df-711">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="333df-711">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="333df-712">String collection</span><span class="sxs-lookup"><span data-stu-id="333df-712">String collection</span></span>|<span data-ttu-id="333df-713">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="333df-713">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="333df-714">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-714">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="333df-715">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-715">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-716">Valor que indica o comportamento de NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="333df-716">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="333df-717">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-717">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-718">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="333df-718">defenderExploitProtectionXml</span></span>|<span data-ttu-id="333df-719">Binária</span><span class="sxs-lookup"><span data-stu-id="333df-719">Binary</span></span>|<span data-ttu-id="333df-720">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="333df-720">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="333df-721">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="333df-721">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="333df-722">String</span><span class="sxs-lookup"><span data-stu-id="333df-722">String</span></span>|<span data-ttu-id="333df-723">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="333df-723">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="333df-724">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="333df-724">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="333df-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-725">Boolean</span></span>|<span data-ttu-id="333df-726">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="333df-726">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="333df-727">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="333df-727">appLockerApplicationControl</span></span>|[<span data-ttu-id="333df-728">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="333df-728">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="333df-729">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="333df-729">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="333df-730">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="333df-730">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="333df-731">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="333df-731">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="333df-732">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="333df-732">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="333df-733">Ative o Credential Guard quando o nível de segurança da plataforma com segurança baseada em inicialização e virtualização segura estiverem habilitados.</span><span class="sxs-lookup"><span data-stu-id="333df-733">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="333df-734">Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="333df-734">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="333df-735">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="333df-735">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="333df-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-736">Boolean</span></span>|<span data-ttu-id="333df-737">Ativa a segurança baseada em virtualização (VBS).</span><span class="sxs-lookup"><span data-stu-id="333df-737">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="333df-738">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="333df-738">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="333df-739">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-739">Boolean</span></span>|<span data-ttu-id="333df-740">Essa propriedade será substituída em maio de 2019 e será substituída pela propriedade DeviceGuardSecureBootWithDMA.</span><span class="sxs-lookup"><span data-stu-id="333df-740">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="333df-741">Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="333df-741">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="333df-742">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="333df-742">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="333df-743">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="333df-743">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="333df-744">Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="333df-744">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="333df-745">Os valores possíveis são: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="333df-745">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="333df-746">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="333df-746">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="333df-747">habilitação</span><span class="sxs-lookup"><span data-stu-id="333df-747">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="333df-748">Permite que o administrador de ti configure o lançamento do System Guard.</span><span class="sxs-lookup"><span data-stu-id="333df-748">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="333df-749">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="333df-749">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="333df-750">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="333df-750">smartScreenEnableInShell</span></span>|<span data-ttu-id="333df-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-751">Boolean</span></span>|<span data-ttu-id="333df-752">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="333df-752">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="333df-753">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="333df-753">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="333df-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-754">Boolean</span></span>|<span data-ttu-id="333df-755">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="333df-755">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="333df-756">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="333df-756">applicationGuardEnabled</span></span>|<span data-ttu-id="333df-757">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-757">Boolean</span></span>|<span data-ttu-id="333df-758">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="333df-758">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="333df-759">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="333df-759">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="333df-760">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="333df-760">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="333df-761">Habilitar o Windows Defender Application Guard para novas versões do Windows.</span><span class="sxs-lookup"><span data-stu-id="333df-761">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="333df-762">Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="333df-762">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="333df-763">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="333df-763">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="333df-764">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="333df-764">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="333df-765">Bloquear a área de transferência para transferir o arquivo de imagem, o arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="333df-765">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="333df-766">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="333df-766">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="333df-767">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="333df-767">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="333df-768">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-768">Boolean</span></span>|<span data-ttu-id="333df-769">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="333df-769">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="333df-770">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="333df-770">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="333df-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-771">Boolean</span></span>|<span data-ttu-id="333df-772">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="333df-772">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="333df-773">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="333df-773">applicationGuardForceAuditing</span></span>|<span data-ttu-id="333df-774">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-774">Boolean</span></span>|<span data-ttu-id="333df-775">A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)</span><span class="sxs-lookup"><span data-stu-id="333df-775">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="333df-776">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="333df-776">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="333df-777">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="333df-777">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="333df-778">Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="333df-778">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="333df-779">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="333df-779">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="333df-780">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="333df-780">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="333df-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-781">Boolean</span></span>|<span data-ttu-id="333df-782">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="333df-782">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="333df-783">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="333df-783">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="333df-784">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-784">Boolean</span></span>|<span data-ttu-id="333df-785">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="333df-785">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="333df-786">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="333df-786">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="333df-787">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-787">Boolean</span></span>|<span data-ttu-id="333df-788">Permitir a impressão em impressoras locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="333df-788">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="333df-789">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="333df-789">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="333df-790">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-790">Boolean</span></span>|<span data-ttu-id="333df-791">Permitir a impressão em impressoras da rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="333df-791">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="333df-792">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="333df-792">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="333df-793">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-793">Boolean</span></span>|<span data-ttu-id="333df-794">Permitir que o Application Guard use virtual GPU</span><span class="sxs-lookup"><span data-stu-id="333df-794">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="333df-795">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="333df-795">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="333df-796">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-796">Boolean</span></span>|<span data-ttu-id="333df-797">Permitir que os usuários baixem arquivos da borda no contêiner do Application Guard e salve-os no sistema de arquivos host</span><span class="sxs-lookup"><span data-stu-id="333df-797">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="333df-798">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="333df-798">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="333df-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-799">Boolean</span></span>|<span data-ttu-id="333df-800">Permite que o administrador permita que os usuários padrão habilitem o encrpytion durante o ingresso no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="333df-800">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="333df-801">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="333df-801">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="333df-802">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-802">Boolean</span></span>|<span data-ttu-id="333df-803">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="333df-803">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="333df-804">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="333df-804">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="333df-805">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-805">Boolean</span></span>|<span data-ttu-id="333df-806">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="333df-806">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="333df-807">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="333df-807">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="333df-808">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="333df-808">bitLockerEncryptDevice</span></span>|<span data-ttu-id="333df-809">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-809">Boolean</span></span>|<span data-ttu-id="333df-810">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="333df-810">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="333df-811">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="333df-811">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="333df-812">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="333df-812">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="333df-813">Política de unidade de sistema BitLocker.</span><span class="sxs-lookup"><span data-stu-id="333df-813">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="333df-814">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="333df-814">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="333df-815">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="333df-815">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="333df-816">Política de unidade fixa do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="333df-816">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="333df-817">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="333df-817">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="333df-818">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="333df-818">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="333df-819">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="333df-819">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="333df-820">bitLockerRecoveryPasswordRotation</span><span class="sxs-lookup"><span data-stu-id="333df-820">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="333df-821">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="333df-821">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="333df-822">Essa configuração inicia uma rotação de senha de recuperação voltada para o cliente após uma recuperação de unidade de sistema operacional (seja usando bootmgr ou WinRE).</span><span class="sxs-lookup"><span data-stu-id="333df-822">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="333df-823">Os valores possíveis são: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span><span class="sxs-lookup"><span data-stu-id="333df-823">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|
|<span data-ttu-id="333df-824">defenderDisableScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="333df-824">defenderDisableScanArchiveFiles</span></span>|<span data-ttu-id="333df-825">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-825">Boolean</span></span>|<span data-ttu-id="333df-826">Permite ou proíbe a verificação de arquivos mortos.</span><span class="sxs-lookup"><span data-stu-id="333df-826">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="333df-827">defenderAllowScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="333df-827">defenderAllowScanArchiveFiles</span></span>|<span data-ttu-id="333df-828">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-828">Boolean</span></span>|<span data-ttu-id="333df-829">Permite ou proíbe a verificação de arquivos mortos.</span><span class="sxs-lookup"><span data-stu-id="333df-829">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="333df-830">defenderDisableBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="333df-830">defenderDisableBehaviorMonitoring</span></span>|<span data-ttu-id="333df-831">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-831">Boolean</span></span>|<span data-ttu-id="333df-832">Permite ou proíbe a funcionalidade de monitoramento de comportamento do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="333df-832">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="333df-833">defenderAllowBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="333df-833">defenderAllowBehaviorMonitoring</span></span>|<span data-ttu-id="333df-834">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-834">Boolean</span></span>|<span data-ttu-id="333df-835">Permite ou proíbe a funcionalidade de monitoramento de comportamento do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="333df-835">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="333df-836">defenderDisableCloudProtection</span><span class="sxs-lookup"><span data-stu-id="333df-836">defenderDisableCloudProtection</span></span>|<span data-ttu-id="333df-837">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-837">Boolean</span></span>|<span data-ttu-id="333df-838">Para melhor proteger seu computador, o Windows Defender enviará informações à Microsoft sobre qualquer problema encontrado.</span><span class="sxs-lookup"><span data-stu-id="333df-838">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="333df-839">A Microsoft analisará essas informações, aprenderá mais sobre problemas que afetam você e outros clientes e oferecem soluções aprimoradas.</span><span class="sxs-lookup"><span data-stu-id="333df-839">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="333df-840">defenderAllowCloudProtection</span><span class="sxs-lookup"><span data-stu-id="333df-840">defenderAllowCloudProtection</span></span>|<span data-ttu-id="333df-841">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-841">Boolean</span></span>|<span data-ttu-id="333df-842">Para melhor proteger seu computador, o Windows Defender enviará informações à Microsoft sobre qualquer problema encontrado.</span><span class="sxs-lookup"><span data-stu-id="333df-842">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="333df-843">A Microsoft analisará essas informações, aprenderá mais sobre problemas que afetam você e outros clientes e oferecem soluções aprimoradas.</span><span class="sxs-lookup"><span data-stu-id="333df-843">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="333df-844">defenderEnableScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="333df-844">defenderEnableScanIncomingMail</span></span>|<span data-ttu-id="333df-845">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-845">Boolean</span></span>|<span data-ttu-id="333df-846">Permite ou proíbe a verificação de email.</span><span class="sxs-lookup"><span data-stu-id="333df-846">Allows or disallows scanning of email.</span></span>|
|<span data-ttu-id="333df-847">defenderEnableScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="333df-847">defenderEnableScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="333df-848">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-848">Boolean</span></span>|<span data-ttu-id="333df-849">Permite ou proíbe uma verificação completa de unidades de rede mapeadas.</span><span class="sxs-lookup"><span data-stu-id="333df-849">Allows or disallows a full scan of mapped network drives.</span></span>|
|<span data-ttu-id="333df-850">defenderDisableScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="333df-850">defenderDisableScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="333df-851">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-851">Boolean</span></span>|<span data-ttu-id="333df-852">Permite ou proíbe uma verificação completa de unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="333df-852">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="333df-853">Durante uma verificação rápida, as unidades removíveis ainda podem ser verificadas.</span><span class="sxs-lookup"><span data-stu-id="333df-853">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="333df-854">defenderAllowScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="333df-854">defenderAllowScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="333df-855">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-855">Boolean</span></span>|<span data-ttu-id="333df-856">Permite ou proíbe uma verificação completa de unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="333df-856">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="333df-857">Durante uma verificação rápida, as unidades removíveis ainda podem ser verificadas.</span><span class="sxs-lookup"><span data-stu-id="333df-857">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="333df-858">defenderDisableScanDownloads</span><span class="sxs-lookup"><span data-stu-id="333df-858">defenderDisableScanDownloads</span></span>|<span data-ttu-id="333df-859">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-859">Boolean</span></span>|<span data-ttu-id="333df-860">Permite ou proíbe a funcionalidade de proteção do Windows Defender IOAVP.</span><span class="sxs-lookup"><span data-stu-id="333df-860">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="333df-861">defenderAllowScanDownloads</span><span class="sxs-lookup"><span data-stu-id="333df-861">defenderAllowScanDownloads</span></span>|<span data-ttu-id="333df-862">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-862">Boolean</span></span>|<span data-ttu-id="333df-863">Permite ou proíbe a funcionalidade de proteção do Windows Defender IOAVP.</span><span class="sxs-lookup"><span data-stu-id="333df-863">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="333df-864">defenderDisableIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="333df-864">defenderDisableIntrusionPreventionSystem</span></span>|<span data-ttu-id="333df-865">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-865">Boolean</span></span>|<span data-ttu-id="333df-866">Permite ou proíbe a funcionalidade de prevenção de invasão do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="333df-866">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="333df-867">defenderAllowIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="333df-867">defenderAllowIntrusionPreventionSystem</span></span>|<span data-ttu-id="333df-868">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-868">Boolean</span></span>|<span data-ttu-id="333df-869">Permite ou proíbe a funcionalidade de prevenção de invasão do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="333df-869">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="333df-870">defenderDisableOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="333df-870">defenderDisableOnAccessProtection</span></span>|<span data-ttu-id="333df-871">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-871">Boolean</span></span>|<span data-ttu-id="333df-872">Permite ou proíbe a funcionalidade de proteção de acesso do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="333df-872">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="333df-873">defenderAllowOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="333df-873">defenderAllowOnAccessProtection</span></span>|<span data-ttu-id="333df-874">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-874">Boolean</span></span>|<span data-ttu-id="333df-875">Permite ou proíbe a funcionalidade de proteção de acesso do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="333df-875">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="333df-876">defenderDisableRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="333df-876">defenderDisableRealTimeMonitoring</span></span>|<span data-ttu-id="333df-877">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-877">Boolean</span></span>|<span data-ttu-id="333df-878">Permite ou proíbe a funcionalidade de monitoramento em tempo real do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="333df-878">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="333df-879">defenderAllowRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="333df-879">defenderAllowRealTimeMonitoring</span></span>|<span data-ttu-id="333df-880">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-880">Boolean</span></span>|<span data-ttu-id="333df-881">Permite ou proíbe a funcionalidade de monitoramento em tempo real do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="333df-881">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="333df-882">defenderDisableScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="333df-882">defenderDisableScanNetworkFiles</span></span>|<span data-ttu-id="333df-883">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-883">Boolean</span></span>|<span data-ttu-id="333df-884">Permite ou não a verificação de arquivos de rede.</span><span class="sxs-lookup"><span data-stu-id="333df-884">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="333df-885">defenderAllowScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="333df-885">defenderAllowScanNetworkFiles</span></span>|<span data-ttu-id="333df-886">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-886">Boolean</span></span>|<span data-ttu-id="333df-887">Permite ou não a verificação de arquivos de rede.</span><span class="sxs-lookup"><span data-stu-id="333df-887">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="333df-888">defenderDisableScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="333df-888">defenderDisableScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="333df-889">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-889">Boolean</span></span>|<span data-ttu-id="333df-890">Permite ou proíbe a funcionalidade de verificação de scripts do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="333df-890">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="333df-891">defenderAllowScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="333df-891">defenderAllowScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="333df-892">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-892">Boolean</span></span>|<span data-ttu-id="333df-893">Permite ou proíbe a funcionalidade de verificação de scripts do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="333df-893">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="333df-894">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="333df-894">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="333df-895">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-895">Boolean</span></span>|<span data-ttu-id="333df-896">Permite ou proíbe o acesso do usuário à interface de usuário do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="333df-896">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="333df-897">Se não permitido, todas as notificações do Windows Defender também serão suprimidas.</span><span class="sxs-lookup"><span data-stu-id="333df-897">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="333df-898">defenderAllowEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="333df-898">defenderAllowEndUserAccess</span></span>|<span data-ttu-id="333df-899">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-899">Boolean</span></span>|<span data-ttu-id="333df-900">Permite ou proíbe o acesso do usuário à interface de usuário do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="333df-900">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="333df-901">Se não permitido, todas as notificações do Windows Defender também serão suprimidas.</span><span class="sxs-lookup"><span data-stu-id="333df-901">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="333df-902">defenderScanMaxCpuPercentage</span><span class="sxs-lookup"><span data-stu-id="333df-902">defenderScanMaxCpuPercentage</span></span>|<span data-ttu-id="333df-903">Int32</span><span class="sxs-lookup"><span data-stu-id="333df-903">Int32</span></span>|<span data-ttu-id="333df-904">Representa o fator de carga de CPU médio para a verificação do Windows Defender (em porcentagem).</span><span class="sxs-lookup"><span data-stu-id="333df-904">Represents the average CPU load factor for the Windows Defender scan (in percent).</span></span> <span data-ttu-id="333df-905">O valor padrão é 50.</span><span class="sxs-lookup"><span data-stu-id="333df-905">The default value is 50.</span></span> <span data-ttu-id="333df-906">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="333df-906">Valid values 0 to 100</span></span>|
|<span data-ttu-id="333df-907">defenderCheckForSignaturesBeforeRunningScan</span><span class="sxs-lookup"><span data-stu-id="333df-907">defenderCheckForSignaturesBeforeRunningScan</span></span>|<span data-ttu-id="333df-908">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-908">Boolean</span></span>|<span data-ttu-id="333df-909">Essa configuração de política permite que você gerencie se uma verificação de novas definições de vírus e spyware ocorrerá antes de executar uma verificação.</span><span class="sxs-lookup"><span data-stu-id="333df-909">This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.</span></span>|
|<span data-ttu-id="333df-910">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="333df-910">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="333df-911">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="333df-911">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="333df-912">Adicionado no Windows 10, versão 1709.</span><span class="sxs-lookup"><span data-stu-id="333df-912">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="333df-913">Essa configuração de política determina o quanto o Windows Defender antivírus agressivo estará no bloqueio e na verificação de arquivos suspeitos.</span><span class="sxs-lookup"><span data-stu-id="333df-913">This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files.</span></span> <span data-ttu-id="333df-914">Tipo de valor é inteiro.</span><span class="sxs-lookup"><span data-stu-id="333df-914">Value type is integer.</span></span> <span data-ttu-id="333df-915">Este recurso requer a configuração "ingressar no Microsoft MAPS" habilitada para funcionar.</span><span class="sxs-lookup"><span data-stu-id="333df-915">This feature requires the "Join Microsoft MAPS" setting enabled in order to function.</span></span> <span data-ttu-id="333df-916">Os valores possíveis são: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span><span class="sxs-lookup"><span data-stu-id="333df-916">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="333df-917">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="333df-917">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="333df-918">Int32</span><span class="sxs-lookup"><span data-stu-id="333df-918">Int32</span></span>|<span data-ttu-id="333df-919">Adicionado no Windows 10, versão 1709.</span><span class="sxs-lookup"><span data-stu-id="333df-919">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="333df-920">Este recurso permite que o Windows Defender antivírus bloqueie um arquivo suspeito por até 60 segundos e examine-o na nuvem para garantir que ele seja seguro.</span><span class="sxs-lookup"><span data-stu-id="333df-920">This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe.</span></span> <span data-ttu-id="333df-921">Tipo de valor é inteiro, intervalo é 0-50.</span><span class="sxs-lookup"><span data-stu-id="333df-921">Value type is integer, range is 0 - 50.</span></span> <span data-ttu-id="333df-922">Esse recurso depende de três outras configurações de mapas que devem ser todos habilitadas-"Configure o bloqueio na primeira vista"; Ingresse no Microsoft MAPS "; "Enviar amostras de arquivo quando uma análise adicional é necessária".</span><span class="sxs-lookup"><span data-stu-id="333df-922">This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required".</span></span> <span data-ttu-id="333df-923">Valores válidos de 0 a 50</span><span class="sxs-lookup"><span data-stu-id="333df-923">Valid values 0 to 50</span></span>|
|<span data-ttu-id="333df-924">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="333df-924">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="333df-925">Int32</span><span class="sxs-lookup"><span data-stu-id="333df-925">Int32</span></span>|<span data-ttu-id="333df-926">Período de tempo (em dias) em que os itens de quarentena serão armazenados no sistema.</span><span class="sxs-lookup"><span data-stu-id="333df-926">Time period (in days) that quarantine items will be stored on the system.</span></span> <span data-ttu-id="333df-927">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="333df-927">Valid values 0 to 90</span></span>|
|<span data-ttu-id="333df-928">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="333df-928">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="333df-929">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-929">Boolean</span></span>|<span data-ttu-id="333df-930">Essa configuração de política permite configurar verificações de atualização para verificações completas agendadas.</span><span class="sxs-lookup"><span data-stu-id="333df-930">This policy setting allows you to configure catch-up scans for scheduled full scans.</span></span> <span data-ttu-id="333df-931">Uma verificação de atualização é uma verificação iniciada porque uma verificação agendada regularmente foi perdida.</span><span class="sxs-lookup"><span data-stu-id="333df-931">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="333df-932">Normalmente, essas verificações agendadas são perdidas porque o computador foi desligado no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="333df-932">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="333df-933">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="333df-933">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="333df-934">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-934">Boolean</span></span>|<span data-ttu-id="333df-935">Essa configuração de política permite que você configure verificações de atualização para verificações rápidas agendadas.</span><span class="sxs-lookup"><span data-stu-id="333df-935">This policy setting allows you to configure catch-up scans for scheduled quick scans.</span></span> <span data-ttu-id="333df-936">Uma verificação de atualização é uma verificação iniciada porque uma verificação agendada regularmente foi perdida.</span><span class="sxs-lookup"><span data-stu-id="333df-936">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="333df-937">Normalmente, essas verificações agendadas são perdidas porque o computador foi desligado no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="333df-937">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="333df-938">defenderEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="333df-938">defenderEnableLowCpuPriority</span></span>|<span data-ttu-id="333df-939">Boolean</span><span class="sxs-lookup"><span data-stu-id="333df-939">Boolean</span></span>|<span data-ttu-id="333df-940">Essa configuração de política permite habilitar ou desabilitar a baixa prioridade de CPU para verificações agendadas.</span><span class="sxs-lookup"><span data-stu-id="333df-940">This policy setting allows you to enable or disable low CPU priority for scheduled scans.</span></span>|
|<span data-ttu-id="333df-941">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="333df-941">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="333df-942">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="333df-942">String collection</span></span>|<span data-ttu-id="333df-943">Extensões de arquivo a serem excluídas das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="333df-943">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="333df-944">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="333df-944">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="333df-945">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="333df-945">String collection</span></span>|<span data-ttu-id="333df-946">Arquivos e pastas a serem excluídos das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="333df-946">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="333df-947">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="333df-947">defenderProcessesToExclude</span></span>|<span data-ttu-id="333df-948">String collection</span><span class="sxs-lookup"><span data-stu-id="333df-948">String collection</span></span>|<span data-ttu-id="333df-949">Processos a serem excluídos das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="333df-949">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="333df-950">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="333df-950">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="333df-951">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="333df-951">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="333df-952">Adicionado no Windows 10, versão 1607.</span><span class="sxs-lookup"><span data-stu-id="333df-952">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="333df-953">Especifica o nível de detecção para aplicativos potencialmente indesejados (PUAs).</span><span class="sxs-lookup"><span data-stu-id="333df-953">Specifies the level of detection for potentially unwanted applications (PUAs).</span></span> <span data-ttu-id="333df-954">O Windows Defender alerta você quando um software potencialmente indesejado está sendo baixado ou tenta se instalar em seu computador.</span><span class="sxs-lookup"><span data-stu-id="333df-954">Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer.</span></span> <span data-ttu-id="333df-955">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="333df-955">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="333df-956">defenderScanDirection</span><span class="sxs-lookup"><span data-stu-id="333df-956">defenderScanDirection</span></span>|[<span data-ttu-id="333df-957">defenderRealtimeScanDirection</span><span class="sxs-lookup"><span data-stu-id="333df-957">defenderRealtimeScanDirection</span></span>](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|<span data-ttu-id="333df-958">Controla quais conjuntos de arquivos devem ser monitorados.</span><span class="sxs-lookup"><span data-stu-id="333df-958">Controls which sets of files should be monitored.</span></span> <span data-ttu-id="333df-959">Os valores possíveis são: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span><span class="sxs-lookup"><span data-stu-id="333df-959">Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="333df-960">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="333df-960">defenderScanType</span></span>|[<span data-ttu-id="333df-961">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="333df-961">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="333df-962">Seleciona se deseja executar uma verificação rápida ou uma verificação completa.</span><span class="sxs-lookup"><span data-stu-id="333df-962">Selects whether to perform a quick scan or full scan.</span></span> <span data-ttu-id="333df-963">Os valores possíveis são: `userDefined`, `disabled`, `quick`, `full`.</span><span class="sxs-lookup"><span data-stu-id="333df-963">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="333df-964">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="333df-964">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="333df-965">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="333df-965">TimeOfDay</span></span>|<span data-ttu-id="333df-966">Seleciona a hora do dia em que a verificação rápida do Windows Defender deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="333df-966">Selects the time of day that the Windows Defender quick scan should run.</span></span> <span data-ttu-id="333df-967">Por exemplo, um valor de 0 = 12:00AM, um valor de 60 = 1:00AM, um valor de 120 = 2:00 e assim por diante, até um valor de 1380 = 11:00PM.</span><span class="sxs-lookup"><span data-stu-id="333df-967">For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM.</span></span> <span data-ttu-id="333df-968">O valor padrão é 120</span><span class="sxs-lookup"><span data-stu-id="333df-968">The default value is 120</span></span>|
|<span data-ttu-id="333df-969">defenderScheduledScanDay</span><span class="sxs-lookup"><span data-stu-id="333df-969">defenderScheduledScanDay</span></span>|[<span data-ttu-id="333df-970">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="333df-970">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="333df-971">Seleciona o dia em que a verificação do Windows Defender deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="333df-971">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="333df-972">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="333df-972">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="333df-973">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="333df-973">defenderScheduledScanTime</span></span>|<span data-ttu-id="333df-974">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="333df-974">TimeOfDay</span></span>|<span data-ttu-id="333df-975">Seleciona a hora do dia em que a verificação do Windows Defender deve ser executada.</span><span class="sxs-lookup"><span data-stu-id="333df-975">Selects the time of day that the Windows Defender scan should run.</span></span>|
|<span data-ttu-id="333df-976">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="333df-976">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="333df-977">Int32</span><span class="sxs-lookup"><span data-stu-id="333df-977">Int32</span></span>|<span data-ttu-id="333df-978">Especifica o intervalo (em horas) que será usado para verificar assinaturas, portanto, em vez de usar o ScheduleDay e Scheduletime, a verificação de novas assinaturas será definida de acordo com o intervalo.</span><span class="sxs-lookup"><span data-stu-id="333df-978">Specifies the interval (in hours) that will be used to check for signatures, so instead of using the ScheduleDay and ScheduleTime the check for new signatures will be set according to the interval.</span></span> <span data-ttu-id="333df-979">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="333df-979">Valid values 0 to 24</span></span>|
|<span data-ttu-id="333df-980">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="333df-980">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="333df-981">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="333df-981">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="333df-982">Verifica se o nível de consentimento do usuário no Windows Defender deve enviar dados.</span><span class="sxs-lookup"><span data-stu-id="333df-982">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="333df-983">Os valores possíveis são: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span><span class="sxs-lookup"><span data-stu-id="333df-983">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="333df-984">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="333df-984">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="333df-985">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="333df-985">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="333df-986">Permite que um administrador especifique quaisquer níveis de severidade de ameaças válidos e a ID de ação padrão correspondente a ser executada.</span><span class="sxs-lookup"><span data-stu-id="333df-986">Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.</span></span>|



## <a name="response"></a><span data-ttu-id="333df-987">Resposta</span><span class="sxs-lookup"><span data-stu-id="333df-987">Response</span></span>
<span data-ttu-id="333df-988">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="333df-988">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="333df-989">Exemplo</span><span class="sxs-lookup"><span data-stu-id="333df-989">Example</span></span>

### <a name="request"></a><span data-ttu-id="333df-990">Solicitação</span><span class="sxs-lookup"><span data-stu-id="333df-990">Request</span></span>
<span data-ttu-id="333df-991">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="333df-991">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="333df-992">Resposta</span><span class="sxs-lookup"><span data-stu-id="333df-992">Response</span></span>
<span data-ttu-id="333df-p225">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="333df-p225">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




