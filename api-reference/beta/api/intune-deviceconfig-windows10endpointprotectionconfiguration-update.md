---
title: Atualizar windows10EndpointProtectionConfiguration
description: Atualizar as propriedades de um objeto windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa50597f724be41707b0f015d89d9fb051bc9969
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571694"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="9e78a-103">Atualizar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e78a-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="9e78a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9e78a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e78a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e78a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e78a-106">Atualizar as propriedades de um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e78a-106">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e78a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e78a-107">Prerequisites</span></span>
<span data-ttu-id="9e78a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9e78a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9e78a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e78a-110">Permission type</span></span>|<span data-ttu-id="9e78a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9e78a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e78a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e78a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e78a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e78a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e78a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e78a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e78a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e78a-115">Not supported.</span></span>|
|<span data-ttu-id="9e78a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e78a-116">Application</span></span>|<span data-ttu-id="9e78a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e78a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e78a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e78a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9e78a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e78a-119">Request headers</span></span>
|<span data-ttu-id="9e78a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9e78a-120">Header</span></span>|<span data-ttu-id="9e78a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9e78a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e78a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e78a-122">Authorization</span></span>|<span data-ttu-id="9e78a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e78a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e78a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9e78a-124">Accept</span></span>|<span data-ttu-id="9e78a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e78a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e78a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e78a-126">Request body</span></span>
<span data-ttu-id="9e78a-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e78a-127">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="9e78a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e78a-128">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="9e78a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e78a-129">Property</span></span>|<span data-ttu-id="9e78a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e78a-130">Type</span></span>|<span data-ttu-id="9e78a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e78a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e78a-132">id</span><span class="sxs-lookup"><span data-stu-id="9e78a-132">id</span></span>|<span data-ttu-id="9e78a-133">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-133">String</span></span>|<span data-ttu-id="9e78a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9e78a-134">Key of the entity.</span></span> <span data-ttu-id="9e78a-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e78a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e78a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e78a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9e78a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e78a-137">DateTimeOffset</span></span>|<span data-ttu-id="9e78a-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9e78a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9e78a-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e78a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e78a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e78a-140">roleScopeTagIds</span></span>|<span data-ttu-id="9e78a-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e78a-141">String collection</span></span>|<span data-ttu-id="9e78a-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9e78a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9e78a-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e78a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e78a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9e78a-144">supportsScopeTags</span></span>|<span data-ttu-id="9e78a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-145">Boolean</span></span>|<span data-ttu-id="9e78a-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9e78a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9e78a-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9e78a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9e78a-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9e78a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9e78a-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e78a-149">This property is read-only.</span></span> <span data-ttu-id="9e78a-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e78a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e78a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e78a-151">createdDateTime</span></span>|<span data-ttu-id="9e78a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e78a-152">DateTimeOffset</span></span>|<span data-ttu-id="9e78a-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9e78a-153">DateTime the object was created.</span></span> <span data-ttu-id="9e78a-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e78a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e78a-155">descrição</span><span class="sxs-lookup"><span data-stu-id="9e78a-155">description</span></span>|<span data-ttu-id="9e78a-156">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-156">String</span></span>|<span data-ttu-id="9e78a-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e78a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9e78a-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e78a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e78a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9e78a-159">displayName</span></span>|<span data-ttu-id="9e78a-160">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-160">String</span></span>|<span data-ttu-id="9e78a-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e78a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9e78a-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e78a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e78a-163">versão</span><span class="sxs-lookup"><span data-stu-id="9e78a-163">version</span></span>|<span data-ttu-id="9e78a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9e78a-164">Int32</span></span>|<span data-ttu-id="9e78a-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e78a-165">Version of the device configuration.</span></span> <span data-ttu-id="9e78a-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e78a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e78a-167">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="9e78a-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="9e78a-168">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="9e78a-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="9e78a-169">Essa política destina-se a fornecer segurança adicional contra dispositivos compatíveis com DMA externo.</span><span class="sxs-lookup"><span data-stu-id="9e78a-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="9e78a-170">Permite mais controle sobre a enumeração de dispositivos compatíveis com DMA externo incompatíveis com o remapeamento de DMA/isolamento de memória do dispositivo e área restrita.</span><span class="sxs-lookup"><span data-stu-id="9e78a-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="9e78a-171">Essa política só entra em vigor quando a proteção DMA de kernel é suportada e habilitada pelo firmware do sistema.</span><span class="sxs-lookup"><span data-stu-id="9e78a-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="9e78a-172">A proteção DMA de kernel é um recurso de plataforma que não pode ser controlado via política ou pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="9e78a-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="9e78a-173">É preciso ter suporte do sistema no momento da fabricação.</span><span class="sxs-lookup"><span data-stu-id="9e78a-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="9e78a-174">Para verificar se o sistema suporta a proteção DMA de kernel, verifique o campo proteção DMA de kernel na página Resumo de MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="9e78a-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="9e78a-175">Os valores possíveis são: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="9e78a-176">firewallRules</span><span class="sxs-lookup"><span data-stu-id="9e78a-176">firewallRules</span></span>|<span data-ttu-id="9e78a-177">coleção [windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="9e78a-177">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="9e78a-178">Define as configurações da regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="9e78a-178">Configures the firewall rule settings.</span></span> <span data-ttu-id="9e78a-179">Essa coleção pode conter um máximo de 150 elementos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-179">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="9e78a-180">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="9e78a-180">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="9e78a-181">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-181">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-182">Esse direito de usuário é usado pelo Gerenciador de credenciais durante o backup/restauração.</span><span class="sxs-lookup"><span data-stu-id="9e78a-182">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="9e78a-183">As credenciais salvas dos usuários podem ser comprometidas se esse privilégio for dado a outras entidades.</span><span class="sxs-lookup"><span data-stu-id="9e78a-183">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="9e78a-184">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9e78a-184">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9e78a-185">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="9e78a-185">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="9e78a-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-187">Esse direito de usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="9e78a-187">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="9e78a-188">O estado permitido é suportado.</span><span class="sxs-lookup"><span data-stu-id="9e78a-188">State Allowed is supported.</span></span>|
|<span data-ttu-id="9e78a-189">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="9e78a-189">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="9e78a-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-191">Esse direito de usuário determina quais usuários e grupos são bloqueados para se conectarem ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="9e78a-191">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="9e78a-192">Há suporte para o bloco de estado.</span><span class="sxs-lookup"><span data-stu-id="9e78a-192">State Block is supported.</span></span>|
|<span data-ttu-id="9e78a-193">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9e78a-193">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="9e78a-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-195">Esse direito de usuário permite que um processo represente qualquer usuário sem autenticação.</span><span class="sxs-lookup"><span data-stu-id="9e78a-195">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="9e78a-196">Portanto, o processo pode ter acesso aos mesmos recursos locais que esse usuário.</span><span class="sxs-lookup"><span data-stu-id="9e78a-196">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="9e78a-197">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9e78a-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9e78a-198">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="9e78a-198">userRightsLocalLogOn</span></span>|[<span data-ttu-id="9e78a-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-200">Esse direito de usuário determina quais usuários podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="9e78a-200">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="9e78a-201">Estados não conFigurados, permitidos e bloqueados são todos suportados</span><span class="sxs-lookup"><span data-stu-id="9e78a-201">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="9e78a-202">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="9e78a-202">userRightsBackupData</span></span>|[<span data-ttu-id="9e78a-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-204">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao fazer backup de arquivos e diretórios.</span><span class="sxs-lookup"><span data-stu-id="9e78a-204">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="9e78a-205">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9e78a-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9e78a-206">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="9e78a-206">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="9e78a-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-208">Este direito de usuário determina quais usuários e grupos podem alterar a hora e a data no relógio interno do computador.</span><span class="sxs-lookup"><span data-stu-id="9e78a-208">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="9e78a-209">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9e78a-209">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9e78a-210">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="9e78a-210">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="9e78a-211">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-211">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-212">Configuração de segurança que determina se os usuários podem criar objetos globais que estão disponíveis para todas as sessões.</span><span class="sxs-lookup"><span data-stu-id="9e78a-212">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="9e78a-213">Os usuários que podem criar objetos globais podem afetar processos executados em sessões de outros usuários, o que pode levar a falhas de aplicativos ou corrupção de dados.</span><span class="sxs-lookup"><span data-stu-id="9e78a-213">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="9e78a-214">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9e78a-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9e78a-215">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="9e78a-215">userRightsCreatePageFile</span></span>|[<span data-ttu-id="9e78a-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-217">Esse direito de usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de paginação.</span><span class="sxs-lookup"><span data-stu-id="9e78a-217">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="9e78a-218">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9e78a-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9e78a-219">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="9e78a-219">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="9e78a-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-221">Este direito de usuário determina quais contas podem ser usadas por processos para criar um objeto de diretório usando o Gerenciador de objetos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-221">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="9e78a-222">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9e78a-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9e78a-223">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="9e78a-223">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="9e78a-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-225">Esse direito de usuário determina se o usuário pode criar um link simbólico do computador no qual está conectado.</span><span class="sxs-lookup"><span data-stu-id="9e78a-225">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="9e78a-226">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9e78a-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9e78a-227">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="9e78a-227">userRightsCreateToken</span></span>|[<span data-ttu-id="9e78a-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-229">Esse direito de usuário determina quais usuários/grupos podem ser usados por processos para criar um token que pode ser usado para obter acesso a qualquer recurso local quando o processo usa uma API interna para criar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="9e78a-229">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="9e78a-230">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9e78a-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9e78a-231">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="9e78a-231">userRightsDebugPrograms</span></span>|[<span data-ttu-id="9e78a-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-233">Esse direito de usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel.</span><span class="sxs-lookup"><span data-stu-id="9e78a-233">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="9e78a-234">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="9e78a-234">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="9e78a-235">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="9e78a-235">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="9e78a-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-237">Este direito de usuário determina quais usuários e grupos estão proibidos de fazer logon como um cliente de serviços de área de trabalho remota.</span><span class="sxs-lookup"><span data-stu-id="9e78a-237">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="9e78a-238">Há suporte apenas para os Estados não conFigurados e bloqueados</span><span class="sxs-lookup"><span data-stu-id="9e78a-238">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="9e78a-239">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="9e78a-239">userRightsDelegation</span></span>|[<span data-ttu-id="9e78a-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-241">Este direito de usuário determina quais usuários podem definir a configuração confiável para delegação em um objeto de usuário ou computador.</span><span class="sxs-lookup"><span data-stu-id="9e78a-241">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="9e78a-242">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-242">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-243">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="9e78a-243">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="9e78a-244">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-244">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-245">Este direito de usuário determina quais contas podem ser usadas por um processo para adicionar entradas ao log de segurança.</span><span class="sxs-lookup"><span data-stu-id="9e78a-245">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="9e78a-246">O log de segurança é usado para rastrear o acesso de sistema não autorizado.</span><span class="sxs-lookup"><span data-stu-id="9e78a-246">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="9e78a-247">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-247">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-248">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="9e78a-248">userRightsImpersonateClient</span></span>|[<span data-ttu-id="9e78a-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-250">A atribuição desse direito de usuário a um usuário permite que programas executados em nome desse usuário representem um cliente.</span><span class="sxs-lookup"><span data-stu-id="9e78a-250">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="9e78a-251">A exigência desse direito de usuário para esse tipo de representação impede que um usuário não autorizado convença um cliente a se conectar a um serviço que ele criou e, em seguida, representando esse cliente, o que pode elevar as permissões do usuário não autorizado para níveis administrativos ou de sistema.</span><span class="sxs-lookup"><span data-stu-id="9e78a-251">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="9e78a-252">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-253">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="9e78a-253">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="9e78a-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-255">Este direito de usuário determina quais contas podem usar um processo com acesso de propriedade de gravação a outro processo para aumentar a prioridade de execução atribuída ao outro processo.</span><span class="sxs-lookup"><span data-stu-id="9e78a-255">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="9e78a-256">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-257">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="9e78a-257">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="9e78a-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-259">Esse direito de usuário determina quais usuários podem carregar e descarregar dinamicamente drivers de dispositivo ou outro código no modo kernel.</span><span class="sxs-lookup"><span data-stu-id="9e78a-259">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="9e78a-260">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-261">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="9e78a-261">userRightsLockMemory</span></span>|[<span data-ttu-id="9e78a-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-263">Esse direito de usuário determina quais contas podem usar um processo para manter os dados na memória física, o que impede que o sistema pagine os dados para a memória virtual em disco.</span><span class="sxs-lookup"><span data-stu-id="9e78a-263">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="9e78a-264">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-265">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="9e78a-265">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="9e78a-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-267">Esse direito de usuário determina quais usuários podem especificar opções de auditoria de acesso a objetos para recursos individuais, como arquivos, objetos do Active Directory e chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="9e78a-267">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="9e78a-268">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-269">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="9e78a-269">userRightsManageVolumes</span></span>|[<span data-ttu-id="9e78a-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-271">Esse direito de usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como a desfragmentação remota.</span><span class="sxs-lookup"><span data-stu-id="9e78a-271">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="9e78a-272">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-273">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="9e78a-273">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="9e78a-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-275">Esse direito de usuário determina quem pode modificar os valores de ambiente de firmware.</span><span class="sxs-lookup"><span data-stu-id="9e78a-275">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="9e78a-276">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-277">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="9e78a-277">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="9e78a-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-279">Este direito de usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves de registro ou processos pertencentes a outros usuários.</span><span class="sxs-lookup"><span data-stu-id="9e78a-279">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="9e78a-280">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-281">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="9e78a-281">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="9e78a-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-283">Esse direito de usuário determina quais usuários podem usar ferramentas de monitoramento de desempenho para monitorar o desempenho de processos do sistema.</span><span class="sxs-lookup"><span data-stu-id="9e78a-283">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="9e78a-284">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-284">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-285">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="9e78a-285">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="9e78a-286">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-286">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-287">Esse direito de usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede.</span><span class="sxs-lookup"><span data-stu-id="9e78a-287">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="9e78a-288">O mau uso desse direito de usuário pode resultar em uma negação de serviço.</span><span class="sxs-lookup"><span data-stu-id="9e78a-288">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="9e78a-289">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-290">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="9e78a-290">userRightsRestoreData</span></span>|[<span data-ttu-id="9e78a-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-292">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao restaurar backups de arquivos e diretórios e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto.</span><span class="sxs-lookup"><span data-stu-id="9e78a-292">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="9e78a-293">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-294">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="9e78a-294">userRightsTakeOwnership</span></span>|[<span data-ttu-id="9e78a-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-296">Esse direito de usuário determina quais usuários podem assumir a propriedade de qualquer objeto protegível no sistema, incluindo objetos do Active Directory, arquivos e pastas, impressoras, chaves do registro, processos e threads.</span><span class="sxs-lookup"><span data-stu-id="9e78a-296">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="9e78a-297">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="9e78a-298">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="9e78a-298">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="9e78a-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="9e78a-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="9e78a-300">Essa configuração de segurança determina quais contas de serviço são impedidas de registrar um processo como um serviço.</span><span class="sxs-lookup"><span data-stu-id="9e78a-300">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="9e78a-301">Observação: esta configuração de segurança não se aplica às contas de sistema, serviço local ou serviço de rede.</span><span class="sxs-lookup"><span data-stu-id="9e78a-301">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="9e78a-302">Só há suporte para o estado bloqueado.</span><span class="sxs-lookup"><span data-stu-id="9e78a-302">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="9e78a-303">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="9e78a-303">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="9e78a-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-304">Boolean</span></span>|<span data-ttu-id="9e78a-305">Essa configuração determina se o salvamento de jogos do Xbox está habilitado (1) ou desabilitado (0).</span><span class="sxs-lookup"><span data-stu-id="9e78a-305">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="9e78a-306">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="9e78a-306">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="9e78a-307">inStarttype</span><span class="sxs-lookup"><span data-stu-id="9e78a-307">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="9e78a-308">Esta configuração determina se o tipo de início do serviço de gerenciamento de acessórios é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="9e78a-308">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="9e78a-309">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="9e78a-309">Default: Manual.</span></span> <span data-ttu-id="9e78a-310">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-310">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="9e78a-311">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="9e78a-311">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="9e78a-312">inStarttype</span><span class="sxs-lookup"><span data-stu-id="9e78a-312">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="9e78a-313">Essa configuração determina se o tipo de início do serviço do Live Authentication Manager é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="9e78a-313">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="9e78a-314">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="9e78a-314">Default: Manual.</span></span> <span data-ttu-id="9e78a-315">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-315">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="9e78a-316">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="9e78a-316">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="9e78a-317">inStarttype</span><span class="sxs-lookup"><span data-stu-id="9e78a-317">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="9e78a-318">Essa configuração determina se o tipo de início do serviço de salvamento do Live Game é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="9e78a-318">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="9e78a-319">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="9e78a-319">Default: Manual.</span></span> <span data-ttu-id="9e78a-320">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-320">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="9e78a-321">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="9e78a-321">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="9e78a-322">inStarttype</span><span class="sxs-lookup"><span data-stu-id="9e78a-322">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="9e78a-323">Esta configuração determina se o tipo de início do serviço de rede é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="9e78a-323">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="9e78a-324">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="9e78a-324">Default: Manual.</span></span> <span data-ttu-id="9e78a-325">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-325">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="9e78a-326">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="9e78a-326">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="9e78a-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-327">Boolean</span></span>|<span data-ttu-id="9e78a-328">Impedir que os usuários adicionem novas contas da Microsoft a este computador.</span><span class="sxs-lookup"><span data-stu-id="9e78a-328">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="9e78a-329">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="9e78a-329">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="9e78a-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-330">Boolean</span></span>|<span data-ttu-id="9e78a-331">Habilitar contas locais que não estão protegidas por senha para fazer logon de locais diferentes do dispositivo físico. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="9e78a-331">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="9e78a-332">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="9e78a-332">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="9e78a-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-333">Boolean</span></span>|<span data-ttu-id="9e78a-334">Determina se a conta de administrador local está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="9e78a-334">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="9e78a-335">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="9e78a-335">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="9e78a-336">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-336">String</span></span>|<span data-ttu-id="9e78a-337">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "administrador".</span><span class="sxs-lookup"><span data-stu-id="9e78a-337">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="9e78a-338">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="9e78a-338">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="9e78a-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-339">Boolean</span></span>|<span data-ttu-id="9e78a-340">Determina se a conta de convidado está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="9e78a-340">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="9e78a-341">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="9e78a-341">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="9e78a-342">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-342">String</span></span>|<span data-ttu-id="9e78a-343">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "convidado".</span><span class="sxs-lookup"><span data-stu-id="9e78a-343">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="9e78a-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="9e78a-344">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="9e78a-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-345">Boolean</span></span>|<span data-ttu-id="9e78a-346">Impedir que um computador portátil seja desencaixado sem ter que fazer logon.</span><span class="sxs-lookup"><span data-stu-id="9e78a-346">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="9e78a-347">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="9e78a-347">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="9e78a-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-348">Boolean</span></span>|<span data-ttu-id="9e78a-349">Restringir a instalação dos drivers de impressora como parte da conexão a uma impressora compartilhada somente para administradores.</span><span class="sxs-lookup"><span data-stu-id="9e78a-349">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="9e78a-350">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="9e78a-350">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="9e78a-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-351">Boolean</span></span>|<span data-ttu-id="9e78a-352">Habilitar essa configuração permite que somente o usuário conectado interativamente acesse a mídia de CD-ROM.</span><span class="sxs-lookup"><span data-stu-id="9e78a-352">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="9e78a-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="9e78a-353">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="9e78a-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="9e78a-354">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="9e78a-355">Defina quem tem permissão para formatar e ejetar a mídia NTFS removível.</span><span class="sxs-lookup"><span data-stu-id="9e78a-355">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="9e78a-356">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-356">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="9e78a-357">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="9e78a-357">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="9e78a-358">Int32</span><span class="sxs-lookup"><span data-stu-id="9e78a-358">Int32</span></span>|<span data-ttu-id="9e78a-359">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="9e78a-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="9e78a-360">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="9e78a-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="9e78a-361">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="9e78a-361">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="9e78a-362">Int32</span><span class="sxs-lookup"><span data-stu-id="9e78a-362">Int32</span></span>|<span data-ttu-id="9e78a-363">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="9e78a-363">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="9e78a-364">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="9e78a-364">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="9e78a-365">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="9e78a-365">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="9e78a-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-366">Boolean</span></span>|<span data-ttu-id="9e78a-367">Exigir CTRL + ALT + DEL para ser pressionada para que um usuário possa fazer logon.</span><span class="sxs-lookup"><span data-stu-id="9e78a-367">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="9e78a-368">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="9e78a-368">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="9e78a-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-369">Boolean</span></span>|<span data-ttu-id="9e78a-370">Não exibe o nome de usuário da última pessoa que entrou neste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e78a-370">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="9e78a-371">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="9e78a-371">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="9e78a-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-372">Boolean</span></span>|<span data-ttu-id="9e78a-373">Não exibe o nome de usuário da pessoa que está entrando neste dispositivo depois que as credenciais são inseridas e antes da área de trabalho do dispositivo ser exibida.</span><span class="sxs-lookup"><span data-stu-id="9e78a-373">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="9e78a-374">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="9e78a-374">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="9e78a-375">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-375">String</span></span>|<span data-ttu-id="9e78a-376">Defina o título da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="9e78a-376">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="9e78a-377">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="9e78a-377">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="9e78a-378">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-378">String</span></span>|<span data-ttu-id="9e78a-379">Definir o texto da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="9e78a-379">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="9e78a-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="9e78a-380">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="9e78a-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-381">Boolean</span></span>|<span data-ttu-id="9e78a-382">Bloquear solicitações de autenticação PKU2U para este dispositivo para usar identidades online.</span><span class="sxs-lookup"><span data-stu-id="9e78a-382">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="9e78a-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="9e78a-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="9e78a-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-384">Boolean</span></span>|<span data-ttu-id="9e78a-385">Boolean do auxiliar da interface do usuário para entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="9e78a-385">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="9e78a-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="9e78a-386">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="9e78a-387">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-387">String</span></span>|<span data-ttu-id="9e78a-388">Edite a cadeia de caracteres de definição de descritor de segurança padrão para permitir ou impedir que usuários e grupos façam chamadas remotas para o SAM.</span><span class="sxs-lookup"><span data-stu-id="9e78a-388">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="9e78a-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="9e78a-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="9e78a-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="9e78a-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="9e78a-391">Essa configuração de segurança permite que um cliente exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="9e78a-391">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="9e78a-392">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="9e78a-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="9e78a-393">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="9e78a-394">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="9e78a-394">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="9e78a-395">Essa configuração de segurança permite que um servidor exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="9e78a-395">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="9e78a-396">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-396">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="9e78a-397">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="9e78a-397">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="9e78a-398">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="9e78a-398">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="9e78a-399">Essa configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede.</span><span class="sxs-lookup"><span data-stu-id="9e78a-399">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="9e78a-400">Os valores possíveis são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-400">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="9e78a-401">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="9e78a-401">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="9e78a-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-402">Boolean</span></span>|<span data-ttu-id="9e78a-403">Se for habilitada, o cliente SMB permitirá logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="9e78a-403">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="9e78a-404">Se não configurada, o cliente SMB rejeitará logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="9e78a-404">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="9e78a-405">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="9e78a-405">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="9e78a-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-406">Boolean</span></span>|<span data-ttu-id="9e78a-407">Configuração de segurança que determina se o arquivo de paginação de memória virtual será limpo quando o sistema for desligado.</span><span class="sxs-lookup"><span data-stu-id="9e78a-407">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="9e78a-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="9e78a-408">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="9e78a-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-409">Boolean</span></span>|<span data-ttu-id="9e78a-410">Configuração de segurança que determina se um computador pode ser desligado sem a necessidade de fazer logon no Windows.</span><span class="sxs-lookup"><span data-stu-id="9e78a-410">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="9e78a-411">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="9e78a-411">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="9e78a-412">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-412">Boolean</span></span>|<span data-ttu-id="9e78a-413">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="9e78a-413">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="9e78a-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="9e78a-414">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="9e78a-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-415">Boolean</span></span>|<span data-ttu-id="9e78a-416">Virtualizar falhas de gravação de arquivo e registro para locais por usuário</span><span class="sxs-lookup"><span data-stu-id="9e78a-416">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="9e78a-417">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="9e78a-417">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="9e78a-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-418">Boolean</span></span>|<span data-ttu-id="9e78a-419">Impor a validação de caminho de certificação PKI para um determinado arquivo executável antes que seja permitido executar.</span><span class="sxs-lookup"><span data-stu-id="9e78a-419">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="9e78a-420">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="9e78a-420">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="9e78a-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="9e78a-421">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="9e78a-422">Definir o comportamento do prompt de elevação para administradores no modo de aprovação de administrador.</span><span class="sxs-lookup"><span data-stu-id="9e78a-422">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="9e78a-423">Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-423">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="9e78a-424">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="9e78a-424">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="9e78a-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="9e78a-425">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="9e78a-426">Definir o comportamento do prompt de elevação para usuários padrão.</span><span class="sxs-lookup"><span data-stu-id="9e78a-426">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="9e78a-427">Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-427">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="9e78a-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="9e78a-428">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="9e78a-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-429">Boolean</span></span>|<span data-ttu-id="9e78a-430">Habilite todas as solicitações de elevação para ir para a área de trabalho do usuário interativo, e não para a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="9e78a-430">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="9e78a-431">As configurações de política de comportamento de prompt para administradores e usuários padrão são usadas.</span><span class="sxs-lookup"><span data-stu-id="9e78a-431">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="9e78a-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="9e78a-432">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="9e78a-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-433">Boolean</span></span>|<span data-ttu-id="9e78a-434">Instalações de aplicativos que exigem privilégios elevados solicitarão credenciais de administrador. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="9e78a-434">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="9e78a-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="9e78a-435">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="9e78a-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-436">Boolean</span></span>|<span data-ttu-id="9e78a-437">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="9e78a-437">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="9e78a-438">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="9e78a-438">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="9e78a-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-439">Boolean</span></span>|<span data-ttu-id="9e78a-440">Define se a conta de administrador interna usa o modo de aprovação de administrador ou executa todos os aplicativos com privilégios de administrador completo. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="9e78a-440">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="9e78a-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="9e78a-441">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="9e78a-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-442">Boolean</span></span>|<span data-ttu-id="9e78a-443">Definir se o modo de aprovação de administrador e todas as configurações de política de UAC estão habilitados, o padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="9e78a-443">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="9e78a-444">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="9e78a-444">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="9e78a-445">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="9e78a-445">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="9e78a-446">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="9e78a-446">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="9e78a-447">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-447">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="9e78a-448">Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-448">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="9e78a-449">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="9e78a-449">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="9e78a-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="9e78a-450">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="9e78a-451">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="9e78a-451">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="9e78a-452">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-452">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="9e78a-453">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-453">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="9e78a-454">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="9e78a-454">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="9e78a-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-455">Boolean</span></span>|<span data-ttu-id="9e78a-456">Configuração de segurança que determina se o cliente SMB tentará negociar assinatura de pacote SMB.</span><span class="sxs-lookup"><span data-stu-id="9e78a-456">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="9e78a-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="9e78a-457">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="9e78a-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-458">Boolean</span></span>|<span data-ttu-id="9e78a-459">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do cliente SMB.</span><span class="sxs-lookup"><span data-stu-id="9e78a-459">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="9e78a-460">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="9e78a-460">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="9e78a-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-461">Boolean</span></span>|<span data-ttu-id="9e78a-462">Se essa configuração de segurança estiver habilitada, o redirecionador de bloco de mensagens de servidor (SMB) terá permissão para enviar senhas de texto não criptografado para servidores SMB não Microsoft que não ofereçam suporte à criptografia de senha durante a autenticação.</span><span class="sxs-lookup"><span data-stu-id="9e78a-462">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="9e78a-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="9e78a-463">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="9e78a-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-464">Boolean</span></span>|<span data-ttu-id="9e78a-465">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do servidor SMB.</span><span class="sxs-lookup"><span data-stu-id="9e78a-465">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="9e78a-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="9e78a-466">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="9e78a-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-467">Boolean</span></span>|<span data-ttu-id="9e78a-468">Configuração de segurança que determina se o servidor SMB negociará assinatura de pacote SMB com clientes que solicitarem.</span><span class="sxs-lookup"><span data-stu-id="9e78a-468">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="9e78a-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="9e78a-469">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="9e78a-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-470">Boolean</span></span>|<span data-ttu-id="9e78a-471">Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e pipes para as configurações de pipes nomeados que podem ser acessados anonimamente e comPartilhamentos que podem ser acessados anonimamente</span><span class="sxs-lookup"><span data-stu-id="9e78a-471">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="9e78a-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="9e78a-472">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="9e78a-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-473">Boolean</span></span>|<span data-ttu-id="9e78a-474">Essa configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas com o computador.</span><span class="sxs-lookup"><span data-stu-id="9e78a-474">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="9e78a-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="9e78a-475">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="9e78a-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-476">Boolean</span></span>|<span data-ttu-id="9e78a-477">Configuração de segurança que determina se os usuários anônimos devem executar determinadas atividades, como enumeração de nomes de contas de domínio e compartilhamentos de rede.</span><span class="sxs-lookup"><span data-stu-id="9e78a-477">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="9e78a-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="9e78a-478">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="9e78a-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-479">Boolean</span></span>|<span data-ttu-id="9e78a-480">Essa configuração de segurança determina se, na próxima alteração de senha, o valor de hash do LM (LAN Manager) para a nova senha é armazenado.</span><span class="sxs-lookup"><span data-stu-id="9e78a-480">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="9e78a-481">Ele não é armazenado por padrão.</span><span class="sxs-lookup"><span data-stu-id="9e78a-481">It’s not stored by default.</span></span>|
|<span data-ttu-id="9e78a-482">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="9e78a-482">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="9e78a-483">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="9e78a-483">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="9e78a-484">Essa configuração de segurança determina o que acontece quando o cartão inteligente de um usuário conectado é removido do leitor de cartão inteligente.</span><span class="sxs-lookup"><span data-stu-id="9e78a-484">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="9e78a-485">Os valores possíveis são: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-485">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="9e78a-486">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-486">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="9e78a-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-487">Boolean</span></span>|<span data-ttu-id="9e78a-488">Usado para desabilitar a exibição da área de proteção de aplicativo e navegador.</span><span class="sxs-lookup"><span data-stu-id="9e78a-488">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="9e78a-489">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-489">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="9e78a-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-490">Boolean</span></span>|<span data-ttu-id="9e78a-491">Usado para desabilitar a exibição da área de opções da família.</span><span class="sxs-lookup"><span data-stu-id="9e78a-491">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="9e78a-492">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-492">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="9e78a-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-493">Boolean</span></span>|<span data-ttu-id="9e78a-494">Usado para desabilitar a exibição da área de desempenho e integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e78a-494">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="9e78a-495">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-495">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="9e78a-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-496">Boolean</span></span>|<span data-ttu-id="9e78a-497">Usado para desabilitar a exibição da área de firewall e proteção de rede.</span><span class="sxs-lookup"><span data-stu-id="9e78a-497">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="9e78a-498">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-498">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="9e78a-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-499">Boolean</span></span>|<span data-ttu-id="9e78a-500">Usado para desabilitar a exibição da área de proteção contra vírus e ameaças.</span><span class="sxs-lookup"><span data-stu-id="9e78a-500">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="9e78a-501">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-501">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="9e78a-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-502">Boolean</span></span>|<span data-ttu-id="9e78a-503">Usado para desabilitar a exibição da área de proteção da conta.</span><span class="sxs-lookup"><span data-stu-id="9e78a-503">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="9e78a-504">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-504">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="9e78a-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-505">Boolean</span></span>|<span data-ttu-id="9e78a-506">Usado para desabilitar a exibição do botão limpar TPM.</span><span class="sxs-lookup"><span data-stu-id="9e78a-506">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="9e78a-507">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-507">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="9e78a-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-508">Boolean</span></span>|<span data-ttu-id="9e78a-509">Usado para desabilitar a exibição da área de proteção de hardware.</span><span class="sxs-lookup"><span data-stu-id="9e78a-509">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="9e78a-510">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-510">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="9e78a-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-511">Boolean</span></span>|<span data-ttu-id="9e78a-512">Usado para desabilitar a exibição do controle da área de notificação.</span><span class="sxs-lookup"><span data-stu-id="9e78a-512">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="9e78a-513">O usuário precisa sair e entrar ou reiniciar o computador para que essa configuração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="9e78a-513">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="9e78a-514">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-514">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="9e78a-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-515">Boolean</span></span>|<span data-ttu-id="9e78a-516">Usado para desabilitar a exibição da área de proteção contra ransomware.</span><span class="sxs-lookup"><span data-stu-id="9e78a-516">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="9e78a-517">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-517">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="9e78a-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-518">Boolean</span></span>|<span data-ttu-id="9e78a-519">Usado para desabilitar a exibição da área de inicialização segura sob segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e78a-519">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="9e78a-520">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-520">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="9e78a-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-521">Boolean</span></span>|<span data-ttu-id="9e78a-522">Usado para desabilitar a exibição do processo de segurança Solucionando problemas de segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9e78a-522">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="9e78a-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="9e78a-523">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="9e78a-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-524">Boolean</span></span>|<span data-ttu-id="9e78a-525">Usado para desabilitar a exibição de atualizar o firmware do TPM quando um firmware vulnerável é detectado.</span><span class="sxs-lookup"><span data-stu-id="9e78a-525">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="9e78a-526">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="9e78a-526">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="9e78a-527">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-527">String</span></span>|<span data-ttu-id="9e78a-528">O nome da empresa que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="9e78a-528">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="9e78a-529">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="9e78a-529">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="9e78a-530">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-530">String</span></span>|<span data-ttu-id="9e78a-531">O endereço de email que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="9e78a-531">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="9e78a-532">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="9e78a-532">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="9e78a-533">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-533">String</span></span>|<span data-ttu-id="9e78a-534">O número de telefone ou Skype ID que é exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="9e78a-534">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="9e78a-535">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="9e78a-535">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="9e78a-536">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-536">String</span></span>|<span data-ttu-id="9e78a-537">A URL do portal da ajuda que é exibida para os usuários.</span><span class="sxs-lookup"><span data-stu-id="9e78a-537">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="9e78a-538">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="9e78a-538">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="9e78a-539">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="9e78a-539">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="9e78a-540">Notificações para mostrar das áreas de aplicativo exibidas.</span><span class="sxs-lookup"><span data-stu-id="9e78a-540">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="9e78a-541">Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-541">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="9e78a-542">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="9e78a-542">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="9e78a-543">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="9e78a-543">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="9e78a-544">Configurar onde exibir informações de contato de ti para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="9e78a-544">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="9e78a-545">Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-545">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="9e78a-546">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="9e78a-546">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="9e78a-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-547">Boolean</span></span>|<span data-ttu-id="9e78a-548">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="9e78a-548">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="9e78a-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="9e78a-549">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="9e78a-550">Int32</span><span class="sxs-lookup"><span data-stu-id="9e78a-550">Int32</span></span>|<span data-ttu-id="9e78a-551">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="9e78a-551">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="9e78a-552">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="9e78a-552">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="9e78a-553">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="9e78a-553">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="9e78a-554">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="9e78a-554">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="9e78a-555">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="9e78a-555">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="9e78a-556">Selecione a codificação de chave pré-compartilhada a ser usada.</span><span class="sxs-lookup"><span data-stu-id="9e78a-556">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="9e78a-557">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-557">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="9e78a-558">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="9e78a-558">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="9e78a-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-559">Boolean</span></span>|<span data-ttu-id="9e78a-560">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="9e78a-560">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="9e78a-561">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="9e78a-561">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="9e78a-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-562">Boolean</span></span>|<span data-ttu-id="9e78a-563">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="9e78a-563">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="9e78a-564">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="9e78a-564">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="9e78a-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-565">Boolean</span></span>|<span data-ttu-id="9e78a-566">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="9e78a-566">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="9e78a-567">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="9e78a-567">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="9e78a-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-568">Boolean</span></span>|<span data-ttu-id="9e78a-569">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="9e78a-569">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="9e78a-570">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="9e78a-570">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="9e78a-571">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="9e78a-571">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="9e78a-572">Especifique como a lista de certificados revogados será imposta.</span><span class="sxs-lookup"><span data-stu-id="9e78a-572">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="9e78a-573">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-573">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="9e78a-574">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="9e78a-574">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="9e78a-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-575">Boolean</span></span>|<span data-ttu-id="9e78a-576">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="9e78a-576">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="9e78a-577">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="9e78a-577">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="9e78a-578">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="9e78a-578">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="9e78a-579">Configura como o enfileiramento de pacotes deve ser aplicado no cenário de gateway de túnel.</span><span class="sxs-lookup"><span data-stu-id="9e78a-579">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="9e78a-580">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-580">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="9e78a-581">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="9e78a-581">firewallProfileDomain</span></span>|[<span data-ttu-id="9e78a-582">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9e78a-582">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="9e78a-583">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="9e78a-583">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="9e78a-584">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="9e78a-584">firewallProfilePublic</span></span>|[<span data-ttu-id="9e78a-585">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9e78a-585">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="9e78a-586">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="9e78a-586">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="9e78a-587">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="9e78a-587">firewallProfilePrivate</span></span>|[<span data-ttu-id="9e78a-588">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9e78a-588">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="9e78a-589">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="9e78a-589">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="9e78a-590">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="9e78a-590">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="9e78a-591">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-591">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-592">O valor que indica o comportamento do Adobe Reader de criar processos filhos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-592">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="9e78a-593">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-593">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-594">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="9e78a-594">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="9e78a-595">String collection</span><span class="sxs-lookup"><span data-stu-id="9e78a-595">String collection</span></span>|<span data-ttu-id="9e78a-596">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="9e78a-596">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="9e78a-597">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-597">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="9e78a-598">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9e78a-598">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9e78a-599">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-599">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="9e78a-600">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-600">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-601">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="9e78a-601">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="9e78a-602">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-602">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-603">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-603">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="9e78a-604">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-604">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-605">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="9e78a-605">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="9e78a-606">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-606">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-607">O valor que indica o comportamento dos aplicativos de comunicação do Office, incluindo o Microsoft Outlook, da criação de processos filhos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-607">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="9e78a-608">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-608">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="9e78a-609">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="9e78a-610">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9e78a-610">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9e78a-611">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="9e78a-611">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="9e78a-612">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-612">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-613">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="9e78a-613">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="9e78a-614">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-614">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-615">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="9e78a-615">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="9e78a-616">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-616">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-617">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="9e78a-617">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="9e78a-618">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9e78a-618">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9e78a-619">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-619">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="9e78a-620">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-620">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-621">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="9e78a-621">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="9e78a-622">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-622">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-623">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-623">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="9e78a-624">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-624">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-625">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="9e78a-625">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="9e78a-626">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9e78a-626">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9e78a-627">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="9e78a-627">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="9e78a-628">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-628">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-629">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="9e78a-629">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="9e78a-630">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-630">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-631">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="9e78a-631">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="9e78a-632">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-632">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-633">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="9e78a-633">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="9e78a-634">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9e78a-634">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9e78a-635">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="9e78a-635">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="9e78a-636">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-636">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-637">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="9e78a-637">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="9e78a-638">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-638">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-639">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="9e78a-639">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="9e78a-640">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-640">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-641">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-641">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="9e78a-642">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9e78a-642">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9e78a-643">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="9e78a-643">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="9e78a-644">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-644">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-645">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="9e78a-645">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="9e78a-646">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-647">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="9e78a-647">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="9e78a-648">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-649">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="9e78a-649">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="9e78a-650">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-650">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-651">Valor que indica se a credencial que está sendo roubada do subsistema de autoridade de segurança local do Windows é permitida.</span><span class="sxs-lookup"><span data-stu-id="9e78a-651">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="9e78a-652">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-652">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-653">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="9e78a-653">defenderProcessCreationType</span></span>|[<span data-ttu-id="9e78a-654">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9e78a-654">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9e78a-655">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="9e78a-655">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="9e78a-656">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-656">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-657">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="9e78a-657">defenderProcessCreation</span></span>|[<span data-ttu-id="9e78a-658">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-658">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-659">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="9e78a-659">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="9e78a-660">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-660">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-661">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="9e78a-661">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="9e78a-662">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9e78a-662">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9e78a-663">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="9e78a-663">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="9e78a-664">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-664">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-665">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="9e78a-665">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="9e78a-666">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-666">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-667">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="9e78a-667">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="9e78a-668">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-668">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-669">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="9e78a-669">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="9e78a-670">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9e78a-670">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9e78a-671">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="9e78a-671">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="9e78a-672">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-672">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-673">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="9e78a-673">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="9e78a-674">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-674">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-675">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="9e78a-675">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="9e78a-676">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-676">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-677">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-677">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="9e78a-678">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="9e78a-678">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="9e78a-679">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="9e78a-679">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="9e78a-680">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-680">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-681">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="9e78a-681">defenderEmailContentExecution</span></span>|[<span data-ttu-id="9e78a-682">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-683">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="9e78a-683">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="9e78a-684">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-685">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-685">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="9e78a-686">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-686">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-687">O valor que indica o uso da proteção avançada contra o Ransomeware.</span><span class="sxs-lookup"><span data-stu-id="9e78a-687">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="9e78a-688">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-688">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-689">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="9e78a-689">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="9e78a-690">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-690">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="9e78a-691">Valor que indica o comportamento das pastas protegidas.</span><span class="sxs-lookup"><span data-stu-id="9e78a-691">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="9e78a-692">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-692">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="9e78a-693">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="9e78a-693">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="9e78a-694">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e78a-694">String collection</span></span>|<span data-ttu-id="9e78a-695">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="9e78a-695">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="9e78a-696">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="9e78a-696">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="9e78a-697">String collection</span><span class="sxs-lookup"><span data-stu-id="9e78a-697">String collection</span></span>|<span data-ttu-id="9e78a-698">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="9e78a-698">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="9e78a-699">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-699">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="9e78a-700">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="9e78a-700">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="9e78a-701">Valor que indica o comportamento de NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="9e78a-701">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="9e78a-702">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-702">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="9e78a-703">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="9e78a-703">defenderExploitProtectionXml</span></span>|<span data-ttu-id="9e78a-704">Binária</span><span class="sxs-lookup"><span data-stu-id="9e78a-704">Binary</span></span>|<span data-ttu-id="9e78a-705">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="9e78a-705">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="9e78a-706">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="9e78a-706">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="9e78a-707">String</span><span class="sxs-lookup"><span data-stu-id="9e78a-707">String</span></span>|<span data-ttu-id="9e78a-708">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="9e78a-708">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="9e78a-709">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="9e78a-709">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="9e78a-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-710">Boolean</span></span>|<span data-ttu-id="9e78a-711">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="9e78a-711">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="9e78a-712">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="9e78a-712">appLockerApplicationControl</span></span>|[<span data-ttu-id="9e78a-713">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="9e78a-713">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="9e78a-714">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-714">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="9e78a-715">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-715">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="9e78a-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="9e78a-716">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="9e78a-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="9e78a-717">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="9e78a-718">Ative o Credential Guard quando o nível de segurança da plataforma com segurança baseada em inicialização e virtualização segura estiverem habilitados.</span><span class="sxs-lookup"><span data-stu-id="9e78a-718">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="9e78a-719">Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-719">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="9e78a-720">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="9e78a-720">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="9e78a-721">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-721">Boolean</span></span>|<span data-ttu-id="9e78a-722">Ativa a segurança baseada em virtualização (VBS).</span><span class="sxs-lookup"><span data-stu-id="9e78a-722">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="9e78a-723">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="9e78a-723">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="9e78a-724">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-724">Boolean</span></span>|<span data-ttu-id="9e78a-725">Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="9e78a-725">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="9e78a-726">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="9e78a-726">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="9e78a-727">habilitação</span><span class="sxs-lookup"><span data-stu-id="9e78a-727">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="9e78a-728">Permite que o administrador de ti configure o lançamento do System Guard.</span><span class="sxs-lookup"><span data-stu-id="9e78a-728">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="9e78a-729">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-729">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="9e78a-730">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="9e78a-730">smartScreenEnableInShell</span></span>|<span data-ttu-id="9e78a-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-731">Boolean</span></span>|<span data-ttu-id="9e78a-732">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="9e78a-732">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="9e78a-733">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="9e78a-733">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="9e78a-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-734">Boolean</span></span>|<span data-ttu-id="9e78a-735">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="9e78a-735">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="9e78a-736">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="9e78a-736">applicationGuardEnabled</span></span>|<span data-ttu-id="9e78a-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-737">Boolean</span></span>|<span data-ttu-id="9e78a-738">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="9e78a-738">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="9e78a-739">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="9e78a-739">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="9e78a-740">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="9e78a-740">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="9e78a-741">Habilitar o Windows Defender Application Guard para novas versões do Windows.</span><span class="sxs-lookup"><span data-stu-id="9e78a-741">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="9e78a-742">Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-742">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="9e78a-743">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="9e78a-743">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="9e78a-744">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="9e78a-744">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="9e78a-745">Bloquear a área de transferência para transferir o arquivo de imagem, o arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="9e78a-745">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="9e78a-746">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-746">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="9e78a-747">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="9e78a-747">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="9e78a-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-748">Boolean</span></span>|<span data-ttu-id="9e78a-749">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="9e78a-749">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="9e78a-750">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="9e78a-750">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="9e78a-751">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-751">Boolean</span></span>|<span data-ttu-id="9e78a-752">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="9e78a-752">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="9e78a-753">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="9e78a-753">applicationGuardForceAuditing</span></span>|<span data-ttu-id="9e78a-754">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-754">Boolean</span></span>|<span data-ttu-id="9e78a-755">A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)</span><span class="sxs-lookup"><span data-stu-id="9e78a-755">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="9e78a-756">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="9e78a-756">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="9e78a-757">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="9e78a-757">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="9e78a-758">Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="9e78a-758">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="9e78a-759">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="9e78a-759">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="9e78a-760">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="9e78a-760">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="9e78a-761">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-761">Boolean</span></span>|<span data-ttu-id="9e78a-762">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="9e78a-762">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="9e78a-763">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="9e78a-763">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="9e78a-764">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-764">Boolean</span></span>|<span data-ttu-id="9e78a-765">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="9e78a-765">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="9e78a-766">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="9e78a-766">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="9e78a-767">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-767">Boolean</span></span>|<span data-ttu-id="9e78a-768">Permitir a impressão em impressoras locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="9e78a-768">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="9e78a-769">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="9e78a-769">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="9e78a-770">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-770">Boolean</span></span>|<span data-ttu-id="9e78a-771">Permitir a impressão em impressoras da rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="9e78a-771">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="9e78a-772">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="9e78a-772">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="9e78a-773">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-773">Boolean</span></span>|<span data-ttu-id="9e78a-774">Permitir que o Application Guard use virtual GPU</span><span class="sxs-lookup"><span data-stu-id="9e78a-774">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="9e78a-775">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="9e78a-775">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="9e78a-776">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-776">Boolean</span></span>|<span data-ttu-id="9e78a-777">Permitir que os usuários baixem arquivos da borda no contêiner do Application Guard e salve-os no sistema de arquivos host</span><span class="sxs-lookup"><span data-stu-id="9e78a-777">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="9e78a-778">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="9e78a-778">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="9e78a-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-779">Boolean</span></span>|<span data-ttu-id="9e78a-780">Permite que o administrador permita que os usuários padrão habilitem o encrpytion durante o ingresso no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9e78a-780">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="9e78a-781">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="9e78a-781">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="9e78a-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-782">Boolean</span></span>|<span data-ttu-id="9e78a-783">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="9e78a-783">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="9e78a-784">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="9e78a-784">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="9e78a-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-785">Boolean</span></span>|<span data-ttu-id="9e78a-786">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="9e78a-786">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="9e78a-787">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="9e78a-787">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="9e78a-788">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="9e78a-788">bitLockerEncryptDevice</span></span>|<span data-ttu-id="9e78a-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e78a-789">Boolean</span></span>|<span data-ttu-id="9e78a-790">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="9e78a-790">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="9e78a-791">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9e78a-791">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="9e78a-792">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9e78a-792">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="9e78a-793">Política de unidade de sistema BitLocker.</span><span class="sxs-lookup"><span data-stu-id="9e78a-793">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="9e78a-794">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9e78a-794">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="9e78a-795">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9e78a-795">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="9e78a-796">Política de unidade fixa do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="9e78a-796">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="9e78a-797">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9e78a-797">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="9e78a-798">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="9e78a-798">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="9e78a-799">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="9e78a-799">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="9e78a-800">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e78a-800">Response</span></span>
<span data-ttu-id="9e78a-801">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e78a-801">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e78a-802">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e78a-802">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e78a-803">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e78a-803">Request</span></span>
<span data-ttu-id="9e78a-804">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e78a-804">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 27641

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="9e78a-805">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e78a-805">Response</span></span>
<span data-ttu-id="9e78a-p199">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e78a-p199">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 27813

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




