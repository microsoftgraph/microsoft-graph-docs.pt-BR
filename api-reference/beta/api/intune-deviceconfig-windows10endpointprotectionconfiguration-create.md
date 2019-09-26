---
title: Criar windows10EndpointProtectionConfiguration
description: Criar um novo objeto windows10EndpointProtectionConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 360895177308aca3b3780b6ebd5c7f15f557e7bb
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37182810"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="567f4-103">Criar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="567f4-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="567f4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="567f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="567f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="567f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="567f4-106">Criar um novo objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="567f4-106">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="567f4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="567f4-107">Prerequisites</span></span>
<span data-ttu-id="567f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="567f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="567f4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="567f4-110">Permission type</span></span>|<span data-ttu-id="567f4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="567f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="567f4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="567f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="567f4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="567f4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="567f4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="567f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="567f4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="567f4-115">Not supported.</span></span>|
|<span data-ttu-id="567f4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="567f4-116">Application</span></span>|<span data-ttu-id="567f4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="567f4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="567f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="567f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="567f4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="567f4-119">Request headers</span></span>
|<span data-ttu-id="567f4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="567f4-120">Header</span></span>|<span data-ttu-id="567f4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="567f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="567f4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="567f4-122">Authorization</span></span>|<span data-ttu-id="567f4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="567f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="567f4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="567f4-124">Accept</span></span>|<span data-ttu-id="567f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="567f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="567f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="567f4-126">Request body</span></span>
<span data-ttu-id="567f4-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="567f4-127">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="567f4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="567f4-128">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="567f4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="567f4-129">Property</span></span>|<span data-ttu-id="567f4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="567f4-130">Type</span></span>|<span data-ttu-id="567f4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="567f4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="567f4-132">id</span><span class="sxs-lookup"><span data-stu-id="567f4-132">id</span></span>|<span data-ttu-id="567f4-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="567f4-133">String</span></span>|<span data-ttu-id="567f4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="567f4-134">Key of the entity.</span></span> <span data-ttu-id="567f4-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567f4-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567f4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="567f4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="567f4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="567f4-137">DateTimeOffset</span></span>|<span data-ttu-id="567f4-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="567f4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="567f4-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567f4-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567f4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="567f4-140">roleScopeTagIds</span></span>|<span data-ttu-id="567f4-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="567f4-141">String collection</span></span>|<span data-ttu-id="567f4-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="567f4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="567f4-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567f4-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567f4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="567f4-144">supportsScopeTags</span></span>|<span data-ttu-id="567f4-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-145">Boolean</span></span>|<span data-ttu-id="567f4-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="567f4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="567f4-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="567f4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="567f4-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="567f4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="567f4-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="567f4-149">This property is read-only.</span></span> <span data-ttu-id="567f4-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567f4-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567f4-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="567f4-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="567f4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="567f4-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="567f4-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="567f4-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="567f4-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567f4-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567f4-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="567f4-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="567f4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="567f4-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="567f4-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="567f4-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="567f4-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567f4-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567f4-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="567f4-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="567f4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="567f4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="567f4-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="567f4-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="567f4-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567f4-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567f4-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="567f4-163">createdDateTime</span></span>|<span data-ttu-id="567f4-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="567f4-164">DateTimeOffset</span></span>|<span data-ttu-id="567f4-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="567f4-165">DateTime the object was created.</span></span> <span data-ttu-id="567f4-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567f4-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567f4-167">descrição</span><span class="sxs-lookup"><span data-stu-id="567f4-167">description</span></span>|<span data-ttu-id="567f4-168">String</span><span class="sxs-lookup"><span data-stu-id="567f4-168">String</span></span>|<span data-ttu-id="567f4-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="567f4-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="567f4-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567f4-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567f4-171">displayName</span><span class="sxs-lookup"><span data-stu-id="567f4-171">displayName</span></span>|<span data-ttu-id="567f4-172">String</span><span class="sxs-lookup"><span data-stu-id="567f4-172">String</span></span>|<span data-ttu-id="567f4-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="567f4-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="567f4-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567f4-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567f4-175">versão</span><span class="sxs-lookup"><span data-stu-id="567f4-175">version</span></span>|<span data-ttu-id="567f4-176">Int32</span><span class="sxs-lookup"><span data-stu-id="567f4-176">Int32</span></span>|<span data-ttu-id="567f4-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="567f4-177">Version of the device configuration.</span></span> <span data-ttu-id="567f4-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="567f4-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="567f4-179">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="567f4-179">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="567f4-180">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="567f4-180">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="567f4-181">Essa política destina-se a fornecer segurança adicional contra dispositivos compatíveis com DMA externo.</span><span class="sxs-lookup"><span data-stu-id="567f4-181">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="567f4-182">Permite mais controle sobre a enumeração de dispositivos compatíveis com DMA externo incompatíveis com o remapeamento de DMA/isolamento de memória do dispositivo e área restrita.</span><span class="sxs-lookup"><span data-stu-id="567f4-182">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="567f4-183">Essa política só entra em vigor quando a proteção DMA de kernel é suportada e habilitada pelo firmware do sistema.</span><span class="sxs-lookup"><span data-stu-id="567f4-183">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="567f4-184">A proteção DMA de kernel é um recurso de plataforma que não pode ser controlado via política ou pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="567f4-184">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="567f4-185">É preciso ter suporte do sistema no momento da fabricação.</span><span class="sxs-lookup"><span data-stu-id="567f4-185">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="567f4-186">Para verificar se o sistema suporta a proteção DMA de kernel, verifique o campo proteção DMA de kernel na página Resumo de MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="567f4-186">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="567f4-187">Os valores possíveis são: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="567f4-187">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="567f4-188">firewallRules</span><span class="sxs-lookup"><span data-stu-id="567f4-188">firewallRules</span></span>|<span data-ttu-id="567f4-189">coleção [windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="567f4-189">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="567f4-190">Define as configurações da regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="567f4-190">Configures the firewall rule settings.</span></span> <span data-ttu-id="567f4-191">Essa coleção pode conter um máximo de 150 elementos.</span><span class="sxs-lookup"><span data-stu-id="567f4-191">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="567f4-192">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="567f4-192">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="567f4-193">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-193">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-194">Esse direito de usuário é usado pelo Gerenciador de credenciais durante o backup/restauração.</span><span class="sxs-lookup"><span data-stu-id="567f4-194">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="567f4-195">As credenciais salvas dos usuários podem ser comprometidas se esse privilégio for dado a outras entidades.</span><span class="sxs-lookup"><span data-stu-id="567f4-195">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="567f4-196">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="567f4-196">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="567f4-197">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="567f4-197">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="567f4-198">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-198">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-199">Esse direito de usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="567f4-199">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="567f4-200">O estado permitido é suportado.</span><span class="sxs-lookup"><span data-stu-id="567f4-200">State Allowed is supported.</span></span>|
|<span data-ttu-id="567f4-201">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="567f4-201">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="567f4-202">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-202">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-203">Esse direito de usuário determina quais usuários e grupos são bloqueados para se conectarem ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="567f4-203">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="567f4-204">Há suporte para o bloco de estado.</span><span class="sxs-lookup"><span data-stu-id="567f4-204">State Block is supported.</span></span>|
|<span data-ttu-id="567f4-205">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="567f4-205">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="567f4-206">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-206">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-207">Esse direito de usuário permite que um processo represente qualquer usuário sem autenticação.</span><span class="sxs-lookup"><span data-stu-id="567f4-207">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="567f4-208">Portanto, o processo pode ter acesso aos mesmos recursos locais que esse usuário.</span><span class="sxs-lookup"><span data-stu-id="567f4-208">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="567f4-209">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="567f4-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="567f4-210">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="567f4-210">userRightsLocalLogOn</span></span>|[<span data-ttu-id="567f4-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-212">Esse direito de usuário determina quais usuários podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="567f4-212">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="567f4-213">Estados não configurados, permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="567f4-213">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="567f4-214">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="567f4-214">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="567f4-215">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-215">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-216">Esse direito de usuário determina quais usuários não podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="567f4-216">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="567f4-217">Estados não configurados, bloqueados são suportados</span><span class="sxs-lookup"><span data-stu-id="567f4-217">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="567f4-218">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="567f4-218">userRightsBackupData</span></span>|[<span data-ttu-id="567f4-219">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-219">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-220">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao fazer backup de arquivos e diretórios.</span><span class="sxs-lookup"><span data-stu-id="567f4-220">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="567f4-221">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="567f4-221">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="567f4-222">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="567f4-222">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="567f4-223">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-223">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-224">Este direito de usuário determina quais usuários e grupos podem alterar a hora e a data no relógio interno do computador.</span><span class="sxs-lookup"><span data-stu-id="567f4-224">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="567f4-225">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="567f4-225">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="567f4-226">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="567f4-226">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="567f4-227">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-227">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-228">Configuração de segurança que determina se os usuários podem criar objetos globais que estão disponíveis para todas as sessões.</span><span class="sxs-lookup"><span data-stu-id="567f4-228">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="567f4-229">Os usuários que podem criar objetos globais podem afetar processos executados em sessões de outros usuários, o que pode levar a falhas de aplicativos ou corrupção de dados.</span><span class="sxs-lookup"><span data-stu-id="567f4-229">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="567f4-230">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="567f4-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="567f4-231">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="567f4-231">userRightsCreatePageFile</span></span>|[<span data-ttu-id="567f4-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-233">Esse direito de usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de paginação.</span><span class="sxs-lookup"><span data-stu-id="567f4-233">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="567f4-234">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="567f4-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="567f4-235">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="567f4-235">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="567f4-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-237">Este direito de usuário determina quais contas podem ser usadas por processos para criar um objeto de diretório usando o Gerenciador de objetos.</span><span class="sxs-lookup"><span data-stu-id="567f4-237">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="567f4-238">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="567f4-238">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="567f4-239">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="567f4-239">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="567f4-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-241">Esse direito de usuário determina se o usuário pode criar um link simbólico do computador no qual está conectado.</span><span class="sxs-lookup"><span data-stu-id="567f4-241">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="567f4-242">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="567f4-242">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="567f4-243">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="567f4-243">userRightsCreateToken</span></span>|[<span data-ttu-id="567f4-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-245">Esse direito de usuário determina quais usuários/grupos podem ser usados por processos para criar um token que pode ser usado para obter acesso a qualquer recurso local quando o processo usa uma API interna para criar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="567f4-245">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="567f4-246">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="567f4-246">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="567f4-247">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="567f4-247">userRightsDebugPrograms</span></span>|[<span data-ttu-id="567f4-248">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-248">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-249">Esse direito de usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel.</span><span class="sxs-lookup"><span data-stu-id="567f4-249">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="567f4-250">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="567f4-250">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="567f4-251">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="567f4-251">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="567f4-252">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-252">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-253">Este direito de usuário determina quais usuários e grupos estão proibidos de fazer logon como um cliente de serviços de área de trabalho remota.</span><span class="sxs-lookup"><span data-stu-id="567f4-253">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="567f4-254">Há suporte apenas para os Estados não configurados e bloqueados</span><span class="sxs-lookup"><span data-stu-id="567f4-254">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="567f4-255">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="567f4-255">userRightsDelegation</span></span>|[<span data-ttu-id="567f4-256">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-256">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-257">Este direito de usuário determina quais usuários podem definir a configuração confiável para delegação em um objeto de usuário ou computador.</span><span class="sxs-lookup"><span data-stu-id="567f4-257">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="567f4-258">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-258">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-259">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="567f4-259">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="567f4-260">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-260">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-261">Este direito de usuário determina quais contas podem ser usadas por um processo para adicionar entradas ao log de segurança.</span><span class="sxs-lookup"><span data-stu-id="567f4-261">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="567f4-262">O log de segurança é usado para rastrear o acesso de sistema não autorizado.</span><span class="sxs-lookup"><span data-stu-id="567f4-262">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="567f4-263">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-263">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-264">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="567f4-264">userRightsImpersonateClient</span></span>|[<span data-ttu-id="567f4-265">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-265">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-266">A atribuição desse direito de usuário a um usuário permite que programas executados em nome desse usuário representem um cliente.</span><span class="sxs-lookup"><span data-stu-id="567f4-266">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="567f4-267">A exigência desse direito de usuário para esse tipo de representação impede que um usuário não autorizado convença um cliente a se conectar a um serviço que ele criou e, em seguida, representando esse cliente, o que pode elevar as permissões do usuário não autorizado para níveis administrativos ou de sistema.</span><span class="sxs-lookup"><span data-stu-id="567f4-267">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="567f4-268">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-269">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="567f4-269">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="567f4-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-271">Este direito de usuário determina quais contas podem usar um processo com acesso de propriedade de gravação a outro processo para aumentar a prioridade de execução atribuída ao outro processo.</span><span class="sxs-lookup"><span data-stu-id="567f4-271">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="567f4-272">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-273">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="567f4-273">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="567f4-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-275">Esse direito de usuário determina quais usuários podem carregar e descarregar dinamicamente drivers de dispositivo ou outro código no modo kernel.</span><span class="sxs-lookup"><span data-stu-id="567f4-275">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="567f4-276">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-277">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="567f4-277">userRightsLockMemory</span></span>|[<span data-ttu-id="567f4-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-279">Esse direito de usuário determina quais contas podem usar um processo para manter os dados na memória física, o que impede que o sistema pagine os dados para a memória virtual em disco.</span><span class="sxs-lookup"><span data-stu-id="567f4-279">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="567f4-280">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-281">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="567f4-281">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="567f4-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-283">Esse direito de usuário determina quais usuários podem especificar opções de auditoria de acesso a objetos para recursos individuais, como arquivos, objetos do Active Directory e chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="567f4-283">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="567f4-284">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-285">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="567f4-285">userRightsManageVolumes</span></span>|[<span data-ttu-id="567f4-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-287">Esse direito de usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como a desfragmentação remota.</span><span class="sxs-lookup"><span data-stu-id="567f4-287">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="567f4-288">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-288">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-289">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="567f4-289">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="567f4-290">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-290">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-291">Esse direito de usuário determina quem pode modificar os valores de ambiente de firmware.</span><span class="sxs-lookup"><span data-stu-id="567f4-291">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="567f4-292">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-292">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-293">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="567f4-293">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="567f4-294">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-294">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-295">Este direito de usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves de registro ou processos pertencentes a outros usuários.</span><span class="sxs-lookup"><span data-stu-id="567f4-295">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="567f4-296">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-296">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-297">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="567f4-297">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="567f4-298">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-298">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-299">Esse direito de usuário determina quais usuários podem usar ferramentas de monitoramento de desempenho para monitorar o desempenho de processos do sistema.</span><span class="sxs-lookup"><span data-stu-id="567f4-299">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="567f4-300">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-300">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-301">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="567f4-301">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="567f4-302">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-302">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-303">Esse direito de usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede.</span><span class="sxs-lookup"><span data-stu-id="567f4-303">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="567f4-304">O mau uso desse direito de usuário pode resultar em uma negação de serviço.</span><span class="sxs-lookup"><span data-stu-id="567f4-304">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="567f4-305">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-305">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-306">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="567f4-306">userRightsRestoreData</span></span>|[<span data-ttu-id="567f4-307">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-307">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-308">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao restaurar backups de arquivos e diretórios e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto.</span><span class="sxs-lookup"><span data-stu-id="567f4-308">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="567f4-309">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-309">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-310">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="567f4-310">userRightsTakeOwnership</span></span>|[<span data-ttu-id="567f4-311">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="567f4-311">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="567f4-312">Esse direito de usuário determina quais usuários podem assumir a propriedade de qualquer objeto protegível no sistema, incluindo objetos do Active Directory, arquivos e pastas, impressoras, chaves do registro, processos e threads.</span><span class="sxs-lookup"><span data-stu-id="567f4-312">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="567f4-313">Há suporte apenas para os Estados não configurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-313">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="567f4-314">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="567f4-314">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="567f4-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-315">Boolean</span></span>|<span data-ttu-id="567f4-316">Essa configuração determina se o salvamento de jogos do Xbox está habilitado (1) ou desabilitado (0).</span><span class="sxs-lookup"><span data-stu-id="567f4-316">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="567f4-317">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="567f4-317">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="567f4-318">instarttype</span><span class="sxs-lookup"><span data-stu-id="567f4-318">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="567f4-319">Esta configuração determina se o tipo de início do serviço de gerenciamento de acessórios é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="567f4-319">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="567f4-320">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="567f4-320">Default: Manual.</span></span> <span data-ttu-id="567f4-321">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="567f4-321">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="567f4-322">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="567f4-322">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="567f4-323">instarttype</span><span class="sxs-lookup"><span data-stu-id="567f4-323">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="567f4-324">Essa configuração determina se o tipo de início do serviço do Live Authentication Manager é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="567f4-324">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="567f4-325">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="567f4-325">Default: Manual.</span></span> <span data-ttu-id="567f4-326">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="567f4-326">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="567f4-327">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="567f4-327">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="567f4-328">instarttype</span><span class="sxs-lookup"><span data-stu-id="567f4-328">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="567f4-329">Essa configuração determina se o tipo de início do serviço de salvamento do Live Game é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="567f4-329">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="567f4-330">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="567f4-330">Default: Manual.</span></span> <span data-ttu-id="567f4-331">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="567f4-331">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="567f4-332">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="567f4-332">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="567f4-333">instarttype</span><span class="sxs-lookup"><span data-stu-id="567f4-333">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="567f4-334">Esta configuração determina se o tipo de início do serviço de rede é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="567f4-334">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="567f4-335">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="567f4-335">Default: Manual.</span></span> <span data-ttu-id="567f4-336">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="567f4-336">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="567f4-337">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="567f4-337">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="567f4-338">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-338">Boolean</span></span>|<span data-ttu-id="567f4-339">Impedir que os usuários adicionem novas contas da Microsoft a este computador.</span><span class="sxs-lookup"><span data-stu-id="567f4-339">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="567f4-340">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="567f4-340">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="567f4-341">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-341">Boolean</span></span>|<span data-ttu-id="567f4-342">Habilitar contas locais que não estão protegidas por senha para fazer logon de locais diferentes do dispositivo físico. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="567f4-342">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="567f4-343">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="567f4-343">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="567f4-344">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-344">Boolean</span></span>|<span data-ttu-id="567f4-345">Determina se a conta de administrador local está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="567f4-345">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="567f4-346">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="567f4-346">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="567f4-347">String</span><span class="sxs-lookup"><span data-stu-id="567f4-347">String</span></span>|<span data-ttu-id="567f4-348">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "administrador".</span><span class="sxs-lookup"><span data-stu-id="567f4-348">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="567f4-349">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="567f4-349">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="567f4-350">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-350">Boolean</span></span>|<span data-ttu-id="567f4-351">Determina se a conta de convidado está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="567f4-351">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="567f4-352">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="567f4-352">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="567f4-353">String</span><span class="sxs-lookup"><span data-stu-id="567f4-353">String</span></span>|<span data-ttu-id="567f4-354">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "convidado".</span><span class="sxs-lookup"><span data-stu-id="567f4-354">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="567f4-355">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="567f4-355">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="567f4-356">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-356">Boolean</span></span>|<span data-ttu-id="567f4-357">Impedir que um computador portátil seja desencaixado sem ter que fazer logon.</span><span class="sxs-lookup"><span data-stu-id="567f4-357">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="567f4-358">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="567f4-358">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="567f4-359">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-359">Boolean</span></span>|<span data-ttu-id="567f4-360">Restringir a instalação dos drivers de impressora como parte da conexão a uma impressora compartilhada somente para administradores.</span><span class="sxs-lookup"><span data-stu-id="567f4-360">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="567f4-361">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="567f4-361">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="567f4-362">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-362">Boolean</span></span>|<span data-ttu-id="567f4-363">Habilitar essa configuração permite que somente o usuário conectado interativamente acesse a mídia de CD-ROM.</span><span class="sxs-lookup"><span data-stu-id="567f4-363">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="567f4-364">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="567f4-364">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="567f4-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="567f4-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="567f4-366">Defina quem tem permissão para formatar e ejetar a mídia NTFS removível.</span><span class="sxs-lookup"><span data-stu-id="567f4-366">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="567f4-367">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="567f4-367">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="567f4-368">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="567f4-368">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="567f4-369">Int32</span><span class="sxs-lookup"><span data-stu-id="567f4-369">Int32</span></span>|<span data-ttu-id="567f4-370">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="567f4-370">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="567f4-371">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="567f4-371">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="567f4-372">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="567f4-372">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="567f4-373">Int32</span><span class="sxs-lookup"><span data-stu-id="567f4-373">Int32</span></span>|<span data-ttu-id="567f4-374">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="567f4-374">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="567f4-375">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="567f4-375">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="567f4-376">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="567f4-376">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="567f4-377">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-377">Boolean</span></span>|<span data-ttu-id="567f4-378">Exigir CTRL + ALT + DEL para ser pressionada para que um usuário possa fazer logon.</span><span class="sxs-lookup"><span data-stu-id="567f4-378">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="567f4-379">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="567f4-379">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="567f4-380">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-380">Boolean</span></span>|<span data-ttu-id="567f4-381">Não exibe o nome de usuário da última pessoa que entrou neste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="567f4-381">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="567f4-382">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="567f4-382">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="567f4-383">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-383">Boolean</span></span>|<span data-ttu-id="567f4-384">Não exibe o nome de usuário da pessoa que está entrando neste dispositivo depois que as credenciais são inseridas e antes da área de trabalho do dispositivo ser exibida.</span><span class="sxs-lookup"><span data-stu-id="567f4-384">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="567f4-385">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="567f4-385">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="567f4-386">String</span><span class="sxs-lookup"><span data-stu-id="567f4-386">String</span></span>|<span data-ttu-id="567f4-387">Defina o título da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="567f4-387">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="567f4-388">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="567f4-388">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="567f4-389">String</span><span class="sxs-lookup"><span data-stu-id="567f4-389">String</span></span>|<span data-ttu-id="567f4-390">Definir o texto da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="567f4-390">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="567f4-391">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="567f4-391">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="567f4-392">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-392">Boolean</span></span>|<span data-ttu-id="567f4-393">Bloquear solicitações de autenticação PKU2U para este dispositivo para usar identidades online.</span><span class="sxs-lookup"><span data-stu-id="567f4-393">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="567f4-394">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="567f4-394">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="567f4-395">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-395">Boolean</span></span>|<span data-ttu-id="567f4-396">Boolean do auxiliar da interface do usuário para entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="567f4-396">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="567f4-397">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="567f4-397">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="567f4-398">String</span><span class="sxs-lookup"><span data-stu-id="567f4-398">String</span></span>|<span data-ttu-id="567f4-399">Edite a cadeia de caracteres de definição de descritor de segurança padrão para permitir ou impedir que usuários e grupos façam chamadas remotas para o SAM.</span><span class="sxs-lookup"><span data-stu-id="567f4-399">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="567f4-400">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="567f4-400">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="567f4-401">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="567f4-401">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="567f4-402">Essa configuração de segurança permite que um cliente exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="567f4-402">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="567f4-403">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="567f4-403">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="567f4-404">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="567f4-404">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="567f4-405">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="567f4-405">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="567f4-406">Essa configuração de segurança permite que um servidor exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="567f4-406">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="567f4-407">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="567f4-407">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="567f4-408">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="567f4-408">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="567f4-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="567f4-409">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="567f4-410">Essa configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede.</span><span class="sxs-lookup"><span data-stu-id="567f4-410">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="567f4-411">Os possíveis valores são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="567f4-411">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="567f4-412">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="567f4-412">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="567f4-413">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-413">Boolean</span></span>|<span data-ttu-id="567f4-414">Se for habilitada, o cliente SMB permitirá logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="567f4-414">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="567f4-415">Se não configurada, o cliente SMB rejeitará logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="567f4-415">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="567f4-416">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="567f4-416">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="567f4-417">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-417">Boolean</span></span>|<span data-ttu-id="567f4-418">Configuração de segurança que determina se o arquivo de paginação de memória virtual será limpo quando o sistema for desligado.</span><span class="sxs-lookup"><span data-stu-id="567f4-418">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="567f4-419">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="567f4-419">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="567f4-420">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-420">Boolean</span></span>|<span data-ttu-id="567f4-421">Configuração de segurança que determina se um computador pode ser desligado sem a necessidade de fazer logon no Windows.</span><span class="sxs-lookup"><span data-stu-id="567f4-421">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="567f4-422">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="567f4-422">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="567f4-423">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-423">Boolean</span></span>|<span data-ttu-id="567f4-424">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="567f4-424">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="567f4-425">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="567f4-425">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="567f4-426">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-426">Boolean</span></span>|<span data-ttu-id="567f4-427">Virtualizar falhas de gravação de arquivo e registro para locais por usuário</span><span class="sxs-lookup"><span data-stu-id="567f4-427">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="567f4-428">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="567f4-428">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="567f4-429">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-429">Boolean</span></span>|<span data-ttu-id="567f4-430">Impor a validação de caminho de certificação PKI para um determinado arquivo executável antes que seja permitido executar.</span><span class="sxs-lookup"><span data-stu-id="567f4-430">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="567f4-431">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="567f4-431">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="567f4-432">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="567f4-432">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="567f4-433">Definir o comportamento do prompt de elevação para administradores no modo de aprovação de administrador.</span><span class="sxs-lookup"><span data-stu-id="567f4-433">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="567f4-434">Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="567f4-434">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="567f4-435">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="567f4-435">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="567f4-436">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="567f4-436">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="567f4-437">Definir o comportamento do prompt de elevação para usuários padrão.</span><span class="sxs-lookup"><span data-stu-id="567f4-437">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="567f4-438">Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="567f4-438">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="567f4-439">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="567f4-439">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="567f4-440">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-440">Boolean</span></span>|<span data-ttu-id="567f4-441">Habilite todas as solicitações de elevação para ir para a área de trabalho do usuário interativo, e não para a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="567f4-441">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="567f4-442">As configurações de política de comportamento de prompt para administradores e usuários padrão são usadas.</span><span class="sxs-lookup"><span data-stu-id="567f4-442">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="567f4-443">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="567f4-443">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="567f4-444">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-444">Boolean</span></span>|<span data-ttu-id="567f4-445">Instalações de aplicativos que exigem privilégios elevados solicitarão credenciais de administrador. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="567f4-445">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="567f4-446">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="567f4-446">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="567f4-447">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-447">Boolean</span></span>|<span data-ttu-id="567f4-448">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="567f4-448">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="567f4-449">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="567f4-449">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="567f4-450">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-450">Boolean</span></span>|<span data-ttu-id="567f4-451">Define se a conta de administrador interna usa o modo de aprovação de administrador ou executa todos os aplicativos com privilégios de administrador completo. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="567f4-451">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="567f4-452">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="567f4-452">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="567f4-453">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-453">Boolean</span></span>|<span data-ttu-id="567f4-454">Definir se o modo de aprovação de administrador e todas as configurações de política de UAC estão habilitados, o padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="567f4-454">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="567f4-455">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="567f4-455">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="567f4-456">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="567f4-456">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="567f4-457">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="567f4-457">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="567f4-458">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-458">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="567f4-459">Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="567f4-459">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="567f4-460">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="567f4-460">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="567f4-461">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="567f4-461">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="567f4-462">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="567f4-462">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="567f4-463">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="567f4-463">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="567f4-464">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="567f4-464">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="567f4-465">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="567f4-465">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="567f4-466">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-466">Boolean</span></span>|<span data-ttu-id="567f4-467">Configuração de segurança que determina se o cliente SMB tentará negociar assinatura de pacote SMB.</span><span class="sxs-lookup"><span data-stu-id="567f4-467">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="567f4-468">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="567f4-468">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="567f4-469">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-469">Boolean</span></span>|<span data-ttu-id="567f4-470">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do cliente SMB.</span><span class="sxs-lookup"><span data-stu-id="567f4-470">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="567f4-471">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="567f4-471">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="567f4-472">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-472">Boolean</span></span>|<span data-ttu-id="567f4-473">Se essa configuração de segurança estiver habilitada, o redirecionador de bloco de mensagens de servidor (SMB) terá permissão para enviar senhas de texto não criptografado para servidores SMB não Microsoft que não ofereçam suporte à criptografia de senha durante a autenticação.</span><span class="sxs-lookup"><span data-stu-id="567f4-473">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="567f4-474">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="567f4-474">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="567f4-475">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-475">Boolean</span></span>|<span data-ttu-id="567f4-476">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do servidor SMB.</span><span class="sxs-lookup"><span data-stu-id="567f4-476">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="567f4-477">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="567f4-477">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="567f4-478">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-478">Boolean</span></span>|<span data-ttu-id="567f4-479">Configuração de segurança que determina se o servidor SMB negociará assinatura de pacote SMB com clientes que solicitarem.</span><span class="sxs-lookup"><span data-stu-id="567f4-479">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="567f4-480">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="567f4-480">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="567f4-481">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-481">Boolean</span></span>|<span data-ttu-id="567f4-482">Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e pipes para as configurações de pipes nomeados que podem ser acessados anonimamente e compartilhamentos que podem ser acessados anonimamente</span><span class="sxs-lookup"><span data-stu-id="567f4-482">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="567f4-483">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="567f4-483">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="567f4-484">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-484">Boolean</span></span>|<span data-ttu-id="567f4-485">Essa configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas com o computador.</span><span class="sxs-lookup"><span data-stu-id="567f4-485">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="567f4-486">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="567f4-486">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="567f4-487">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-487">Boolean</span></span>|<span data-ttu-id="567f4-488">Configuração de segurança que determina se os usuários anônimos devem executar determinadas atividades, como enumeração de nomes de contas de domínio e compartilhamentos de rede.</span><span class="sxs-lookup"><span data-stu-id="567f4-488">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="567f4-489">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="567f4-489">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="567f4-490">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-490">Boolean</span></span>|<span data-ttu-id="567f4-491">Essa configuração de segurança determina se, na próxima alteração de senha, o valor de hash do LM (LAN Manager) para a nova senha é armazenado.</span><span class="sxs-lookup"><span data-stu-id="567f4-491">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="567f4-492">Ele não é armazenado por padrão.</span><span class="sxs-lookup"><span data-stu-id="567f4-492">It’s not stored by default.</span></span>|
|<span data-ttu-id="567f4-493">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="567f4-493">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="567f4-494">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="567f4-494">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="567f4-495">Essa configuração de segurança determina o que acontece quando o cartão inteligente de um usuário conectado é removido do leitor de cartão inteligente.</span><span class="sxs-lookup"><span data-stu-id="567f4-495">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="567f4-496">Os valores possíveis são: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="567f4-496">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="567f4-497">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="567f4-497">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="567f4-498">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-498">Boolean</span></span>|<span data-ttu-id="567f4-499">Usado para desabilitar a exibição da área de proteção de aplicativo e navegador.</span><span class="sxs-lookup"><span data-stu-id="567f4-499">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="567f4-500">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="567f4-500">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="567f4-501">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-501">Boolean</span></span>|<span data-ttu-id="567f4-502">Usado para desabilitar a exibição da área de opções da família.</span><span class="sxs-lookup"><span data-stu-id="567f4-502">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="567f4-503">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="567f4-503">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="567f4-504">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-504">Boolean</span></span>|<span data-ttu-id="567f4-505">Usado para desabilitar a exibição da área de desempenho e integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="567f4-505">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="567f4-506">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="567f4-506">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="567f4-507">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-507">Boolean</span></span>|<span data-ttu-id="567f4-508">Usado para desabilitar a exibição da área de firewall e proteção de rede.</span><span class="sxs-lookup"><span data-stu-id="567f4-508">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="567f4-509">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="567f4-509">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="567f4-510">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-510">Boolean</span></span>|<span data-ttu-id="567f4-511">Usado para desabilitar a exibição da área de proteção contra vírus e ameaças.</span><span class="sxs-lookup"><span data-stu-id="567f4-511">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="567f4-512">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="567f4-512">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="567f4-513">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-513">Boolean</span></span>|<span data-ttu-id="567f4-514">Usado para desabilitar a exibição da área de proteção da conta.</span><span class="sxs-lookup"><span data-stu-id="567f4-514">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="567f4-515">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="567f4-515">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="567f4-516">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-516">Boolean</span></span>|<span data-ttu-id="567f4-517">Usado para desabilitar a exibição do botão limpar TPM.</span><span class="sxs-lookup"><span data-stu-id="567f4-517">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="567f4-518">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="567f4-518">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="567f4-519">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-519">Boolean</span></span>|<span data-ttu-id="567f4-520">Usado para desabilitar a exibição da área de proteção de hardware.</span><span class="sxs-lookup"><span data-stu-id="567f4-520">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="567f4-521">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="567f4-521">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="567f4-522">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-522">Boolean</span></span>|<span data-ttu-id="567f4-523">Usado para desabilitar a exibição do controle da área de notificação.</span><span class="sxs-lookup"><span data-stu-id="567f4-523">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="567f4-524">O usuário precisa sair e entrar ou reiniciar o computador para que essa configuração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="567f4-524">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="567f4-525">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="567f4-525">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="567f4-526">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-526">Boolean</span></span>|<span data-ttu-id="567f4-527">Usado para desabilitar a exibição da área de proteção contra ransomware.</span><span class="sxs-lookup"><span data-stu-id="567f4-527">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="567f4-528">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="567f4-528">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="567f4-529">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-529">Boolean</span></span>|<span data-ttu-id="567f4-530">Usado para desabilitar a exibição da área de inicialização segura sob segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="567f4-530">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="567f4-531">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="567f4-531">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="567f4-532">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-532">Boolean</span></span>|<span data-ttu-id="567f4-533">Usado para desabilitar a exibição do processo de segurança Solucionando problemas de segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="567f4-533">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="567f4-534">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="567f4-534">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="567f4-535">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-535">Boolean</span></span>|<span data-ttu-id="567f4-536">Usado para desabilitar a exibição de atualizar o firmware do TPM quando um firmware vulnerável é detectado.</span><span class="sxs-lookup"><span data-stu-id="567f4-536">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="567f4-537">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="567f4-537">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="567f4-538">String</span><span class="sxs-lookup"><span data-stu-id="567f4-538">String</span></span>|<span data-ttu-id="567f4-539">O nome da empresa que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="567f4-539">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="567f4-540">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="567f4-540">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="567f4-541">String</span><span class="sxs-lookup"><span data-stu-id="567f4-541">String</span></span>|<span data-ttu-id="567f4-542">O endereço de email que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="567f4-542">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="567f4-543">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="567f4-543">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="567f4-544">String</span><span class="sxs-lookup"><span data-stu-id="567f4-544">String</span></span>|<span data-ttu-id="567f4-545">O número de telefone ou Skype ID que é exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="567f4-545">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="567f4-546">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="567f4-546">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="567f4-547">String</span><span class="sxs-lookup"><span data-stu-id="567f4-547">String</span></span>|<span data-ttu-id="567f4-548">A URL do portal da ajuda que é exibida para os usuários.</span><span class="sxs-lookup"><span data-stu-id="567f4-548">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="567f4-549">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="567f4-549">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="567f4-550">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="567f4-550">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="567f4-551">Notificações para mostrar das áreas de aplicativo exibidas.</span><span class="sxs-lookup"><span data-stu-id="567f4-551">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="567f4-552">Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="567f4-552">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="567f4-553">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="567f4-553">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="567f4-554">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="567f4-554">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="567f4-555">Configurar onde exibir informações de contato de ti para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="567f4-555">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="567f4-556">Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="567f4-556">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="567f4-557">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="567f4-557">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="567f4-558">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="567f4-558">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="567f4-559">Defina as configurações do Windows Defender TamperProtection.</span><span class="sxs-lookup"><span data-stu-id="567f4-559">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="567f4-560">Os valores possíveis são: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="567f4-560">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="567f4-561">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="567f4-561">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="567f4-562">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-562">Boolean</span></span>|<span data-ttu-id="567f4-563">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="567f4-563">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="567f4-564">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="567f4-564">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="567f4-565">Int32</span><span class="sxs-lookup"><span data-stu-id="567f4-565">Int32</span></span>|<span data-ttu-id="567f4-566">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="567f4-566">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="567f4-567">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="567f4-567">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="567f4-568">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="567f4-568">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="567f4-569">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="567f4-569">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="567f4-570">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="567f4-570">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="567f4-571">Selecione a codificação de chave pré-compartilhada a ser usada.</span><span class="sxs-lookup"><span data-stu-id="567f4-571">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="567f4-572">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="567f4-572">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="567f4-573">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="567f4-573">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="567f4-574">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-574">Boolean</span></span>|<span data-ttu-id="567f4-575">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="567f4-575">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="567f4-576">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="567f4-576">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="567f4-577">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-577">Boolean</span></span>|<span data-ttu-id="567f4-578">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="567f4-578">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="567f4-579">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="567f4-579">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="567f4-580">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-580">Boolean</span></span>|<span data-ttu-id="567f4-581">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="567f4-581">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="567f4-582">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="567f4-582">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="567f4-583">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-583">Boolean</span></span>|<span data-ttu-id="567f4-584">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="567f4-584">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="567f4-585">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="567f4-585">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="567f4-586">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="567f4-586">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="567f4-587">Especifique como a lista de certificados revogados será imposta.</span><span class="sxs-lookup"><span data-stu-id="567f4-587">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="567f4-588">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="567f4-588">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="567f4-589">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="567f4-589">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="567f4-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="567f4-590">Boolean</span></span>|<span data-ttu-id="567f4-591">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="567f4-591">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="567f4-592">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="567f4-592">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="567f4-593">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="567f4-593">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="567f4-594">Configura como o enfileiramento de pacotes deve ser aplicado no cenário de gateway de túnel.</span><span class="sxs-lookup"><span data-stu-id="567f4-594">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="567f4-595">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="567f4-595">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="567f4-596">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="567f4-596">firewallProfileDomain</span></span>|[<span data-ttu-id="567f4-597">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="567f4-597">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="567f4-598">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="567f4-598">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="567f4-599">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="567f4-599">firewallProfilePublic</span></span>|[<span data-ttu-id="567f4-600">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="567f4-600">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="567f4-601">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="567f4-601">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="567f4-602">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="567f4-602">firewallProfilePrivate</span></span>|[<span data-ttu-id="567f4-603">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="567f4-603">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="567f4-604">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="567f4-604">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="567f4-605">attackSurfaceReductionRules</span><span class="sxs-lookup"><span data-stu-id="567f4-605">attackSurfaceReductionRules</span></span>|<span data-ttu-id="567f4-606">String</span><span class="sxs-lookup"><span data-stu-id="567f4-606">String</span></span>|<span data-ttu-id="567f4-607">Regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="567f4-607">Attack surface reduction rules</span></span>|
|<span data-ttu-id="567f4-608">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="567f4-608">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="567f4-609">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-609">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-610">O valor que indica o comportamento do Adobe Reader de criar processos filhos.</span><span class="sxs-lookup"><span data-stu-id="567f4-610">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="567f4-611">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-611">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-612">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="567f4-612">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="567f4-613">String collection</span><span class="sxs-lookup"><span data-stu-id="567f4-613">String collection</span></span>|<span data-ttu-id="567f4-614">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="567f4-614">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="567f4-615">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-615">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="567f4-616">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="567f4-616">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="567f4-617">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="567f4-617">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="567f4-618">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-618">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-619">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="567f4-619">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="567f4-620">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-620">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-621">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="567f4-621">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="567f4-622">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-622">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-623">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="567f4-623">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="567f4-624">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-624">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-625">O valor que indica o comportamento dos aplicativos de comunicação do Office, incluindo o Microsoft Outlook, da criação de processos filhos.</span><span class="sxs-lookup"><span data-stu-id="567f4-625">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="567f4-626">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-626">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-627">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="567f4-627">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="567f4-628">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="567f4-628">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="567f4-629">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="567f4-629">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="567f4-630">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-630">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-631">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="567f4-631">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="567f4-632">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-632">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-633">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="567f4-633">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="567f4-634">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-634">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-635">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="567f4-635">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="567f4-636">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="567f4-636">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="567f4-637">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="567f4-637">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="567f4-638">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-638">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-639">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="567f4-639">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="567f4-640">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-640">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-641">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="567f4-641">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="567f4-642">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-642">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-643">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="567f4-643">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="567f4-644">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="567f4-644">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="567f4-645">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="567f4-645">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="567f4-646">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-646">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-647">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="567f4-647">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="567f4-648">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-648">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-649">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="567f4-649">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="567f4-650">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-650">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-651">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="567f4-651">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="567f4-652">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="567f4-652">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="567f4-653">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="567f4-653">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="567f4-654">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-654">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-655">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="567f4-655">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="567f4-656">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-656">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-657">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="567f4-657">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="567f4-658">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-658">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-659">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="567f4-659">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="567f4-660">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="567f4-660">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="567f4-661">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="567f4-661">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="567f4-662">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-662">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-663">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="567f4-663">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="567f4-664">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-664">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-665">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="567f4-665">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="567f4-666">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-666">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-667">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="567f4-667">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="567f4-668">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-668">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-669">Valor que indica se a credencial que está sendo roubada do subsistema de autoridade de segurança local do Windows é permitida.</span><span class="sxs-lookup"><span data-stu-id="567f4-669">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="567f4-670">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-670">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-671">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="567f4-671">defenderProcessCreationType</span></span>|[<span data-ttu-id="567f4-672">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="567f4-672">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="567f4-673">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="567f4-673">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="567f4-674">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-674">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-675">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="567f4-675">defenderProcessCreation</span></span>|[<span data-ttu-id="567f4-676">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-676">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-677">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="567f4-677">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="567f4-678">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-678">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-679">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="567f4-679">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="567f4-680">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="567f4-680">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="567f4-681">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="567f4-681">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="567f4-682">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-682">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-683">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="567f4-683">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="567f4-684">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-684">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-685">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="567f4-685">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="567f4-686">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-686">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-687">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="567f4-687">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="567f4-688">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="567f4-688">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="567f4-689">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="567f4-689">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="567f4-690">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-690">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-691">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="567f4-691">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="567f4-692">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-692">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-693">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="567f4-693">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="567f4-694">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-694">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-695">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="567f4-695">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="567f4-696">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="567f4-696">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="567f4-697">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="567f4-697">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="567f4-698">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-698">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-699">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="567f4-699">defenderEmailContentExecution</span></span>|[<span data-ttu-id="567f4-700">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-700">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-701">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="567f4-701">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="567f4-702">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-702">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-703">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-703">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="567f4-704">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-704">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-705">O valor que indica o uso da proteção avançada contra o Ransomeware.</span><span class="sxs-lookup"><span data-stu-id="567f4-705">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="567f4-706">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-706">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-707">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="567f4-707">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="567f4-708">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-708">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="567f4-709">Valor que indica o comportamento das pastas protegidas.</span><span class="sxs-lookup"><span data-stu-id="567f4-709">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="567f4-710">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="567f4-710">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="567f4-711">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="567f4-711">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="567f4-712">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="567f4-712">String collection</span></span>|<span data-ttu-id="567f4-713">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="567f4-713">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="567f4-714">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="567f4-714">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="567f4-715">String collection</span><span class="sxs-lookup"><span data-stu-id="567f4-715">String collection</span></span>|<span data-ttu-id="567f4-716">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="567f4-716">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="567f4-717">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-717">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="567f4-718">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="567f4-718">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="567f4-719">Valor que indica o comportamento de NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="567f4-719">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="567f4-720">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="567f4-720">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="567f4-721">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="567f4-721">defenderExploitProtectionXml</span></span>|<span data-ttu-id="567f4-722">Binária</span><span class="sxs-lookup"><span data-stu-id="567f4-722">Binary</span></span>|<span data-ttu-id="567f4-723">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="567f4-723">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="567f4-724">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="567f4-724">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="567f4-725">String</span><span class="sxs-lookup"><span data-stu-id="567f4-725">String</span></span>|<span data-ttu-id="567f4-726">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="567f4-726">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="567f4-727">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="567f4-727">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="567f4-728">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-728">Boolean</span></span>|<span data-ttu-id="567f4-729">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="567f4-729">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="567f4-730">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="567f4-730">appLockerApplicationControl</span></span>|[<span data-ttu-id="567f4-731">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="567f4-731">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="567f4-732">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="567f4-732">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="567f4-733">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="567f4-733">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="567f4-734">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="567f4-734">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="567f4-735">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="567f4-735">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="567f4-736">Ative o Credential Guard quando o nível de segurança da plataforma com segurança baseada em inicialização e virtualização segura estiverem habilitados.</span><span class="sxs-lookup"><span data-stu-id="567f4-736">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="567f4-737">Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="567f4-737">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="567f4-738">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="567f4-738">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="567f4-739">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-739">Boolean</span></span>|<span data-ttu-id="567f4-740">Ativa a segurança baseada em virtualização (VBS).</span><span class="sxs-lookup"><span data-stu-id="567f4-740">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="567f4-741">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="567f4-741">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="567f4-742">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-742">Boolean</span></span>|<span data-ttu-id="567f4-743">Essa propriedade será substituída em maio de 2019 e será substituída pela propriedade DeviceGuardSecureBootWithDMA.</span><span class="sxs-lookup"><span data-stu-id="567f4-743">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="567f4-744">Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="567f4-744">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="567f4-745">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="567f4-745">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="567f4-746">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="567f4-746">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="567f4-747">Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="567f4-747">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="567f4-748">Os valores possíveis são: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="567f4-748">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="567f4-749">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="567f4-749">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="567f4-750">habilitação</span><span class="sxs-lookup"><span data-stu-id="567f4-750">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="567f4-751">Permite que o administrador de ti configure o lançamento do System Guard.</span><span class="sxs-lookup"><span data-stu-id="567f4-751">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="567f4-752">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="567f4-752">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="567f4-753">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="567f4-753">smartScreenEnableInShell</span></span>|<span data-ttu-id="567f4-754">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-754">Boolean</span></span>|<span data-ttu-id="567f4-755">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="567f4-755">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="567f4-756">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="567f4-756">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="567f4-757">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-757">Boolean</span></span>|<span data-ttu-id="567f4-758">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="567f4-758">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="567f4-759">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="567f4-759">applicationGuardEnabled</span></span>|<span data-ttu-id="567f4-760">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-760">Boolean</span></span>|<span data-ttu-id="567f4-761">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="567f4-761">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="567f4-762">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="567f4-762">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="567f4-763">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="567f4-763">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="567f4-764">Habilitar o Windows Defender Application Guard para novas versões do Windows.</span><span class="sxs-lookup"><span data-stu-id="567f4-764">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="567f4-765">Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="567f4-765">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="567f4-766">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="567f4-766">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="567f4-767">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="567f4-767">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="567f4-768">Bloquear a área de transferência para transferir o arquivo de imagem, o arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="567f4-768">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="567f4-769">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="567f4-769">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="567f4-770">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="567f4-770">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="567f4-771">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-771">Boolean</span></span>|<span data-ttu-id="567f4-772">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="567f4-772">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="567f4-773">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="567f4-773">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="567f4-774">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-774">Boolean</span></span>|<span data-ttu-id="567f4-775">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="567f4-775">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="567f4-776">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="567f4-776">applicationGuardForceAuditing</span></span>|<span data-ttu-id="567f4-777">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-777">Boolean</span></span>|<span data-ttu-id="567f4-778">A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)</span><span class="sxs-lookup"><span data-stu-id="567f4-778">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="567f4-779">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="567f4-779">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="567f4-780">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="567f4-780">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="567f4-781">Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="567f4-781">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="567f4-782">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="567f4-782">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="567f4-783">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="567f4-783">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="567f4-784">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-784">Boolean</span></span>|<span data-ttu-id="567f4-785">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="567f4-785">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="567f4-786">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="567f4-786">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="567f4-787">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-787">Boolean</span></span>|<span data-ttu-id="567f4-788">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="567f4-788">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="567f4-789">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="567f4-789">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="567f4-790">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-790">Boolean</span></span>|<span data-ttu-id="567f4-791">Permitir a impressão em impressoras locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="567f4-791">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="567f4-792">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="567f4-792">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="567f4-793">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-793">Boolean</span></span>|<span data-ttu-id="567f4-794">Permitir a impressão em impressoras da rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="567f4-794">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="567f4-795">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="567f4-795">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="567f4-796">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-796">Boolean</span></span>|<span data-ttu-id="567f4-797">Permitir que o Application Guard use virtual GPU</span><span class="sxs-lookup"><span data-stu-id="567f4-797">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="567f4-798">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="567f4-798">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="567f4-799">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-799">Boolean</span></span>|<span data-ttu-id="567f4-800">Permitir que os usuários baixem arquivos da borda no contêiner do Application Guard e salve-os no sistema de arquivos host</span><span class="sxs-lookup"><span data-stu-id="567f4-800">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="567f4-801">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="567f4-801">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="567f4-802">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-802">Boolean</span></span>|<span data-ttu-id="567f4-803">Permite que o administrador permita que os usuários padrão habilitem o encrpytion durante o ingresso no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="567f4-803">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="567f4-804">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="567f4-804">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="567f4-805">Booliano</span><span class="sxs-lookup"><span data-stu-id="567f4-805">Boolean</span></span>|<span data-ttu-id="567f4-806">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="567f4-806">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="567f4-807">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="567f4-807">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="567f4-808">Boolean</span><span class="sxs-lookup"><span data-stu-id="567f4-808">Boolean</span></span>|<span data-ttu-id="567f4-809">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="567f4-809">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="567f4-810">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="567f4-810">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="567f4-811">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="567f4-811">bitLockerEncryptDevice</span></span>|<span data-ttu-id="567f4-812">Boolean</span><span class="sxs-lookup"><span data-stu-id="567f4-812">Boolean</span></span>|<span data-ttu-id="567f4-813">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="567f4-813">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="567f4-814">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="567f4-814">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="567f4-815">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="567f4-815">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="567f4-816">Política de unidade de sistema BitLocker.</span><span class="sxs-lookup"><span data-stu-id="567f4-816">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="567f4-817">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="567f4-817">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="567f4-818">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="567f4-818">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="567f4-819">Política de unidade fixa do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="567f4-819">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="567f4-820">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="567f4-820">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="567f4-821">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="567f4-821">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="567f4-822">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="567f4-822">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="567f4-823">bitLockerRecoveryPasswordRotation</span><span class="sxs-lookup"><span data-stu-id="567f4-823">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="567f4-824">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="567f4-824">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="567f4-825">Essa configuração inicia uma rotação de senha de recuperação voltada para o cliente após uma recuperação de unidade de sistema operacional (seja usando bootmgr ou WinRE).</span><span class="sxs-lookup"><span data-stu-id="567f4-825">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="567f4-826">Os valores possíveis são: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span><span class="sxs-lookup"><span data-stu-id="567f4-826">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|



## <a name="response"></a><span data-ttu-id="567f4-827">Resposta</span><span class="sxs-lookup"><span data-stu-id="567f4-827">Response</span></span>
<span data-ttu-id="567f4-828">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="567f4-828">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="567f4-829">Exemplo</span><span class="sxs-lookup"><span data-stu-id="567f4-829">Example</span></span>

### <a name="request"></a><span data-ttu-id="567f4-830">Solicitação</span><span class="sxs-lookup"><span data-stu-id="567f4-830">Request</span></span>
<span data-ttu-id="567f4-831">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="567f4-831">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 28662

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
  "attackSurfaceReductionRules": "Attack Surface Reduction Rules value",
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
  "bitLockerRecoveryPasswordRotation": "disabled"
}
```

### <a name="response"></a><span data-ttu-id="567f4-832">Resposta</span><span class="sxs-lookup"><span data-stu-id="567f4-832">Response</span></span>
<span data-ttu-id="567f4-p206">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="567f4-p206">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 28834

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
  "attackSurfaceReductionRules": "Attack Surface Reduction Rules value",
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
  "bitLockerRecoveryPasswordRotation": "disabled"
}
```




