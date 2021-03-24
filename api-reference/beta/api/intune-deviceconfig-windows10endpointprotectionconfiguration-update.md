---
title: Atualizar windows10EndpointProtectionConfiguration
description: Atualizar as propriedades de um objeto windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a46dd9dfa046ad638f6c0518442324809324828
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147487"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="75563-103">Atualizar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="75563-103">Update windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="75563-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75563-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75563-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75563-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75563-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75563-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75563-107">Atualizar as propriedades de um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="75563-107">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75563-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75563-108">Prerequisites</span></span>
<span data-ttu-id="75563-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75563-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75563-111">Permission type</span></span>|<span data-ttu-id="75563-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75563-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75563-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75563-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75563-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75563-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="75563-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75563-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75563-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75563-116">Not supported.</span></span>|
|<span data-ttu-id="75563-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75563-117">Application</span></span>|<span data-ttu-id="75563-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75563-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75563-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75563-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="75563-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75563-120">Request headers</span></span>
|<span data-ttu-id="75563-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75563-121">Header</span></span>|<span data-ttu-id="75563-122">Valor</span><span class="sxs-lookup"><span data-stu-id="75563-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75563-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="75563-123">Authorization</span></span>|<span data-ttu-id="75563-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75563-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75563-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75563-125">Accept</span></span>|<span data-ttu-id="75563-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75563-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75563-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75563-127">Request body</span></span>
<span data-ttu-id="75563-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="75563-128">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="75563-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="75563-129">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="75563-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75563-130">Property</span></span>|<span data-ttu-id="75563-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="75563-131">Type</span></span>|<span data-ttu-id="75563-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="75563-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75563-133">id</span><span class="sxs-lookup"><span data-stu-id="75563-133">id</span></span>|<span data-ttu-id="75563-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-134">String</span></span>|<span data-ttu-id="75563-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="75563-135">Key of the entity.</span></span> <span data-ttu-id="75563-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75563-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75563-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75563-137">lastModifiedDateTime</span></span>|<span data-ttu-id="75563-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75563-138">DateTimeOffset</span></span>|<span data-ttu-id="75563-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="75563-139">DateTime the object was last modified.</span></span> <span data-ttu-id="75563-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75563-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75563-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="75563-141">roleScopeTagIds</span></span>|<span data-ttu-id="75563-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-142">String collection</span></span>|<span data-ttu-id="75563-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="75563-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="75563-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75563-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75563-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="75563-145">supportsScopeTags</span></span>|<span data-ttu-id="75563-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-146">Boolean</span></span>|<span data-ttu-id="75563-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="75563-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="75563-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="75563-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="75563-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="75563-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="75563-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="75563-150">This property is read-only.</span></span> <span data-ttu-id="75563-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75563-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75563-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="75563-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="75563-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="75563-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="75563-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="75563-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="75563-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75563-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75563-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="75563-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="75563-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="75563-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="75563-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="75563-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="75563-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75563-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75563-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="75563-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="75563-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="75563-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="75563-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="75563-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="75563-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75563-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75563-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75563-164">createdDateTime</span></span>|<span data-ttu-id="75563-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75563-165">DateTimeOffset</span></span>|<span data-ttu-id="75563-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="75563-166">DateTime the object was created.</span></span> <span data-ttu-id="75563-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75563-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75563-168">descrição</span><span class="sxs-lookup"><span data-stu-id="75563-168">description</span></span>|<span data-ttu-id="75563-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-169">String</span></span>|<span data-ttu-id="75563-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75563-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="75563-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75563-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75563-172">displayName</span><span class="sxs-lookup"><span data-stu-id="75563-172">displayName</span></span>|<span data-ttu-id="75563-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-173">String</span></span>|<span data-ttu-id="75563-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75563-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="75563-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75563-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75563-176">versão</span><span class="sxs-lookup"><span data-stu-id="75563-176">version</span></span>|<span data-ttu-id="75563-177">Int32</span><span class="sxs-lookup"><span data-stu-id="75563-177">Int32</span></span>|<span data-ttu-id="75563-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75563-178">Version of the device configuration.</span></span> <span data-ttu-id="75563-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="75563-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75563-180">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="75563-180">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="75563-181">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="75563-181">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="75563-182">Esta política destina-se a fornecer segurança adicional contra dispositivos externos com capacidade de DMA.</span><span class="sxs-lookup"><span data-stu-id="75563-182">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="75563-183">Ele permite mais controle sobre a enumeração de dispositivos externos capazes de DMA incompatíveis com o remapping/isolamento de memória do dispositivo e área de segurança.</span><span class="sxs-lookup"><span data-stu-id="75563-183">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="75563-184">Essa política só entra em vigor quando a Proteção DMA do Kernel é suportada e habilitada pelo firmware do sistema.</span><span class="sxs-lookup"><span data-stu-id="75563-184">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="75563-185">O Kernel DMA Protection é um recurso de plataforma que não pode ser controlado por meio de política ou por usuário final.</span><span class="sxs-lookup"><span data-stu-id="75563-185">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="75563-186">Ele precisa ser suportado pelo sistema no momento da fabricação.</span><span class="sxs-lookup"><span data-stu-id="75563-186">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="75563-187">Para verificar se o sistema dá suporte à Proteção DMA kernel, verifique o campo Proteção DMA kernel na página Resumo de MSINFO32.exe.</span><span class="sxs-lookup"><span data-stu-id="75563-187">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="75563-188">Os valores possíveis são: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="75563-188">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="75563-189">firewallRules</span><span class="sxs-lookup"><span data-stu-id="75563-189">firewallRules</span></span>|<span data-ttu-id="75563-190">[Coleção windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="75563-190">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="75563-191">Configura as configurações de regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="75563-191">Configures the firewall rule settings.</span></span> <span data-ttu-id="75563-192">Essa coleção pode conter no máximo 150 elementos.</span><span class="sxs-lookup"><span data-stu-id="75563-192">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="75563-193">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="75563-193">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="75563-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-195">Esse direito de usuário é usado pelo Gerenciador de Credenciais durante Backup/Restauração.</span><span class="sxs-lookup"><span data-stu-id="75563-195">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="75563-196">As credenciais salvas dos usuários podem ser comprometidas se esse privilégio for dado a outras entidades.</span><span class="sxs-lookup"><span data-stu-id="75563-196">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="75563-197">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="75563-198">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="75563-198">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="75563-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-200">Esse direito do usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="75563-200">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="75563-201">Há suporte para State Allowed.</span><span class="sxs-lookup"><span data-stu-id="75563-201">State Allowed is supported.</span></span>|
|<span data-ttu-id="75563-202">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="75563-202">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="75563-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-204">Esse direito do usuário determina quais usuários e grupos estão bloqueados para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="75563-204">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="75563-205">Há suporte para o Bloqueio de Estado.</span><span class="sxs-lookup"><span data-stu-id="75563-205">State Block is supported.</span></span>|
|<span data-ttu-id="75563-206">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="75563-206">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="75563-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-208">Esse direito de usuário permite que um processo represente qualquer usuário sem autenticação.</span><span class="sxs-lookup"><span data-stu-id="75563-208">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="75563-209">O processo pode, portanto, obter acesso aos mesmos recursos locais desse usuário.</span><span class="sxs-lookup"><span data-stu-id="75563-209">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="75563-210">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="75563-211">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="75563-211">userRightsLocalLogOn</span></span>|[<span data-ttu-id="75563-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-213">Esse direito do usuário determina quais usuários podem fazer logoff no computador.</span><span class="sxs-lookup"><span data-stu-id="75563-213">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="75563-214">Estados NotConfigured, Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-214">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="75563-215">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="75563-215">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="75563-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-217">Esse direito do usuário determina quais usuários não podem fazer logoff no computador.</span><span class="sxs-lookup"><span data-stu-id="75563-217">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="75563-218">Estados NotConfigured, Blocked são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-218">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="75563-219">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="75563-219">userRightsBackupData</span></span>|[<span data-ttu-id="75563-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-221">Esse direito do usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao fazer o back-up de arquivos e diretórios.</span><span class="sxs-lookup"><span data-stu-id="75563-221">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="75563-222">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="75563-223">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="75563-223">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="75563-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-225">Esse direito do usuário determina quais usuários e grupos podem alterar a hora e a data no relógio interno do computador.</span><span class="sxs-lookup"><span data-stu-id="75563-225">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="75563-226">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="75563-227">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="75563-227">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="75563-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-229">Essa configuração de segurança determina se os usuários podem criar objetos globais disponíveis para todas as sessões.</span><span class="sxs-lookup"><span data-stu-id="75563-229">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="75563-230">Os usuários que podem criar objetos globais podem afetar processos que são executados em sessões de outros usuários, o que pode levar à falha do aplicativo ou à corrupção de dados.</span><span class="sxs-lookup"><span data-stu-id="75563-230">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="75563-231">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="75563-232">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="75563-232">userRightsCreatePageFile</span></span>|[<span data-ttu-id="75563-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-234">Esse direito do usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de página.</span><span class="sxs-lookup"><span data-stu-id="75563-234">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="75563-235">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-235">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="75563-236">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="75563-236">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="75563-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-238">Esse direito do usuário determina quais contas podem ser usadas pelos processos para criar um objeto de diretório usando o gerenciador de objetos.</span><span class="sxs-lookup"><span data-stu-id="75563-238">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="75563-239">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-239">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="75563-240">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="75563-240">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="75563-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-242">Esse direito do usuário determina se o usuário pode criar um link simbólico do computador no qual ele está conectado.</span><span class="sxs-lookup"><span data-stu-id="75563-242">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="75563-243">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-243">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="75563-244">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="75563-244">userRightsCreateToken</span></span>|[<span data-ttu-id="75563-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-246">Esse direito do usuário determina quais usuários/grupos podem ser usados pelos processos para criar um token que pode ser usado para obter acesso a todos os recursos locais quando o processo usa uma API interna para criar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="75563-246">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="75563-247">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-247">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="75563-248">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="75563-248">userRightsDebugPrograms</span></span>|[<span data-ttu-id="75563-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-250">Esse direito do usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel.</span><span class="sxs-lookup"><span data-stu-id="75563-250">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="75563-251">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-251">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="75563-252">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="75563-252">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="75563-253">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-253">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-254">Esse direito do usuário determina quais usuários e grupos são proibidos de fazer logons como um cliente de Serviços de Área de Trabalho Remota.</span><span class="sxs-lookup"><span data-stu-id="75563-254">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="75563-255">Somente estados NotConfigured e Blocked são suportados</span><span class="sxs-lookup"><span data-stu-id="75563-255">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="75563-256">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="75563-256">userRightsDelegation</span></span>|[<span data-ttu-id="75563-257">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-257">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-258">Esse direito do usuário determina quais usuários podem definir a configuração Confiável para Delegação em um objeto de usuário ou computador.</span><span class="sxs-lookup"><span data-stu-id="75563-258">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="75563-259">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-260">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="75563-260">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="75563-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-262">Esse direito do usuário determina quais contas podem ser usadas por um processo para adicionar entradas ao log de segurança.</span><span class="sxs-lookup"><span data-stu-id="75563-262">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="75563-263">O log de segurança é usado para rastrear o acesso não autorizado ao sistema.</span><span class="sxs-lookup"><span data-stu-id="75563-263">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="75563-264">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-265">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="75563-265">userRightsImpersonateClient</span></span>|[<span data-ttu-id="75563-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-267">Atribuir esse direito de usuário a um usuário permite que programas em execução em nome desse usuário representem um cliente.</span><span class="sxs-lookup"><span data-stu-id="75563-267">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="75563-268">Exigir esse direito de usuário para esse tipo de representação impede que um usuário não autorizado possa convencer um cliente a se conectar a um serviço que ele criou e, em seguida, representar esse cliente, o que pode elevar as permissões do usuário não autorizado para níveis administrativos ou de sistema.</span><span class="sxs-lookup"><span data-stu-id="75563-268">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="75563-269">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-270">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="75563-270">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="75563-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-272">Esse direito do usuário determina quais contas podem usar um processo com acesso à Propriedade Write para outro processo para aumentar a prioridade de execução atribuída ao outro processo.</span><span class="sxs-lookup"><span data-stu-id="75563-272">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="75563-273">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-274">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="75563-274">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="75563-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-276">Esse direito do usuário determina quais usuários podem carregar e descarregar dinamicamente drivers de dispositivo ou outro código no modo kernel.</span><span class="sxs-lookup"><span data-stu-id="75563-276">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="75563-277">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-278">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="75563-278">userRightsLockMemory</span></span>|[<span data-ttu-id="75563-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-280">Esse direito do usuário determina quais contas podem usar um processo para manter dados na memória física, o que impede que o sistema paja os dados para a memória virtual no disco.</span><span class="sxs-lookup"><span data-stu-id="75563-280">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="75563-281">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-282">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="75563-282">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="75563-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-284">Esse direito do usuário determina quais usuários podem especificar opções de auditoria de acesso a objetos para recursos individuais, como arquivos, objetos do Active Directory e chaves do Registro.</span><span class="sxs-lookup"><span data-stu-id="75563-284">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="75563-285">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-286">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="75563-286">userRightsManageVolumes</span></span>|[<span data-ttu-id="75563-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-288">Esse direito do usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como desfragmentação remota.</span><span class="sxs-lookup"><span data-stu-id="75563-288">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="75563-289">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-290">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="75563-290">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="75563-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-292">Esse direito do usuário determina quem pode modificar valores de ambiente de firmware.</span><span class="sxs-lookup"><span data-stu-id="75563-292">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="75563-293">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-294">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="75563-294">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="75563-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-296">Esse direito do usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves do Registro ou processos pertencentes a outros usuários.</span><span class="sxs-lookup"><span data-stu-id="75563-296">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="75563-297">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-298">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="75563-298">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="75563-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-300">Esse direito do usuário determina quais usuários podem usar ferramentas de monitoramento de desempenho para monitorar o desempenho dos processos do sistema.</span><span class="sxs-lookup"><span data-stu-id="75563-300">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="75563-301">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-301">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-302">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="75563-302">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="75563-303">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-303">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-304">Esse direito do usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede.</span><span class="sxs-lookup"><span data-stu-id="75563-304">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="75563-305">O uso indevido desse direito de usuário pode resultar em negação de serviço.</span><span class="sxs-lookup"><span data-stu-id="75563-305">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="75563-306">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-306">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-307">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="75563-307">userRightsRestoreData</span></span>|[<span data-ttu-id="75563-308">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-308">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-309">Esse direito do usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao restaurar arquivos e diretórios de backup e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto.</span><span class="sxs-lookup"><span data-stu-id="75563-309">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="75563-310">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-310">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-311">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="75563-311">userRightsTakeOwnership</span></span>|[<span data-ttu-id="75563-312">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="75563-312">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="75563-313">Esse direito do usuário determina quais usuários podem assumir a propriedade de qualquer objeto segura no sistema, incluindo objetos, arquivos e pastas do Active Directory, impressoras, chaves de registro, processos e threads.</span><span class="sxs-lookup"><span data-stu-id="75563-313">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="75563-314">Somente os estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="75563-314">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="75563-315">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="75563-315">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="75563-316">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-316">Boolean</span></span>|<span data-ttu-id="75563-317">Essa configuração determina se o jogo do xbox está habilitado (1) ou desabilitado (0).</span><span class="sxs-lookup"><span data-stu-id="75563-317">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="75563-318">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="75563-318">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="75563-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="75563-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="75563-320">Essa configuração determina se o tipo de início do serviço de gerenciamento de acessórios é Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="75563-320">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="75563-321">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="75563-321">Default: Manual.</span></span> <span data-ttu-id="75563-322">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="75563-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="75563-323">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="75563-323">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="75563-324">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="75563-324">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="75563-325">Essa configuração determina se o tipo de início do serviço Live Auth Manager é Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="75563-325">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="75563-326">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="75563-326">Default: Manual.</span></span> <span data-ttu-id="75563-327">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="75563-327">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="75563-328">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="75563-328">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="75563-329">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="75563-329">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="75563-330">Essa configuração determina se o tipo de início do serviço de salvar jogo ao vivo é Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="75563-330">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="75563-331">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="75563-331">Default: Manual.</span></span> <span data-ttu-id="75563-332">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="75563-332">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="75563-333">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="75563-333">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="75563-334">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="75563-334">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="75563-335">Essa configuração determina se o tipo de início do serviço de rede é Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="75563-335">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="75563-336">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="75563-336">Default: Manual.</span></span> <span data-ttu-id="75563-337">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="75563-337">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="75563-338">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="75563-338">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="75563-339">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-339">Boolean</span></span>|<span data-ttu-id="75563-340">Impedir que os usuários adicionem novas contas da Microsoft a este computador.</span><span class="sxs-lookup"><span data-stu-id="75563-340">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="75563-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="75563-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="75563-342">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-342">Boolean</span></span>|<span data-ttu-id="75563-343">Habilitar contas locais que não estão protegidas por senha para fazer logoff de locais diferentes do dispositivo físico. O padrão está habilitado</span><span class="sxs-lookup"><span data-stu-id="75563-343">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="75563-344">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="75563-344">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="75563-345">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-345">Boolean</span></span>|<span data-ttu-id="75563-346">Determina se a conta de Administrador Local está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="75563-346">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="75563-347">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="75563-347">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="75563-348">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-348">String</span></span>|<span data-ttu-id="75563-349">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "Administrador".</span><span class="sxs-lookup"><span data-stu-id="75563-349">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="75563-350">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="75563-350">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="75563-351">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-351">Boolean</span></span>|<span data-ttu-id="75563-352">Determina se a conta de convidado está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="75563-352">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="75563-353">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="75563-353">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="75563-354">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-354">String</span></span>|<span data-ttu-id="75563-355">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "Guest".</span><span class="sxs-lookup"><span data-stu-id="75563-355">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="75563-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="75563-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="75563-357">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-357">Boolean</span></span>|<span data-ttu-id="75563-358">Impedir que um computador portátil seja desfeito sem precisar fazer logon.</span><span class="sxs-lookup"><span data-stu-id="75563-358">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="75563-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="75563-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="75563-360">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-360">Boolean</span></span>|<span data-ttu-id="75563-361">Restringir a instalação de drivers de impressora como parte da conexão com uma impressora compartilhada somente para administradores.</span><span class="sxs-lookup"><span data-stu-id="75563-361">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="75563-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="75563-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="75563-363">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-363">Boolean</span></span>|<span data-ttu-id="75563-364">Habilitando essas configurações permite que apenas o usuário conectado interativamente acesse a mídia CD-ROM.</span><span class="sxs-lookup"><span data-stu-id="75563-364">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="75563-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="75563-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="75563-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="75563-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="75563-367">Definir quem tem permissão para formatar e ejetar mídia NTFS removível.</span><span class="sxs-lookup"><span data-stu-id="75563-367">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="75563-368">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="75563-368">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="75563-369">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="75563-369">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="75563-370">Int32</span><span class="sxs-lookup"><span data-stu-id="75563-370">Int32</span></span>|<span data-ttu-id="75563-371">Defina minutos máximos de inatividade na tela de logon da área de trabalho interativa até que o protetor de tela seja executado.</span><span class="sxs-lookup"><span data-stu-id="75563-371">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="75563-372">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="75563-372">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="75563-373">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="75563-373">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="75563-374">Int32</span><span class="sxs-lookup"><span data-stu-id="75563-374">Int32</span></span>|<span data-ttu-id="75563-375">Defina minutos máximos de inatividade na tela de logon da área de trabalho interativa até que o protetor de tela seja executado.</span><span class="sxs-lookup"><span data-stu-id="75563-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="75563-376">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="75563-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="75563-377">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="75563-377">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="75563-378">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-378">Boolean</span></span>|<span data-ttu-id="75563-379">Exigir que CTRL+ALT+DEL seja pressionado antes que um usuário possa fazer logoff.</span><span class="sxs-lookup"><span data-stu-id="75563-379">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="75563-380">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="75563-380">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="75563-381">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-381">Boolean</span></span>|<span data-ttu-id="75563-382">Não exibe o nome de usuário da última pessoa que se inscreveu neste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75563-382">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="75563-383">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="75563-383">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="75563-384">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-384">Boolean</span></span>|<span data-ttu-id="75563-385">Não exibe o nome de usuário da pessoa que está entrando nesse dispositivo depois que as credenciais são inseridas e antes que a área de trabalho do dispositivo seja mostrada.</span><span class="sxs-lookup"><span data-stu-id="75563-385">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="75563-386">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="75563-386">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="75563-387">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-387">String</span></span>|<span data-ttu-id="75563-388">De definir o título da mensagem para os usuários que tentam fazer logoff.</span><span class="sxs-lookup"><span data-stu-id="75563-388">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="75563-389">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="75563-389">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="75563-390">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-390">String</span></span>|<span data-ttu-id="75563-391">Definir texto de mensagem para usuários que tentam fazer logoff.</span><span class="sxs-lookup"><span data-stu-id="75563-391">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="75563-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="75563-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="75563-393">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-393">Boolean</span></span>|<span data-ttu-id="75563-394">Bloquear solicitações de autenticação PKU2U para esse dispositivo para usar identidades online.</span><span class="sxs-lookup"><span data-stu-id="75563-394">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="75563-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="75563-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="75563-396">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-396">Boolean</span></span>|<span data-ttu-id="75563-397">Boolean auxiliar da interface do usuário para a entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="75563-397">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="75563-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="75563-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="75563-399">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-399">String</span></span>|<span data-ttu-id="75563-400">Edite a cadeia de caracteres padrão do Idioma de Definição do Descritor de Segurança para permitir ou negar que usuários e grupos façam chamadas remotas para o SAM.</span><span class="sxs-lookup"><span data-stu-id="75563-400">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="75563-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="75563-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="75563-402">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="75563-402">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="75563-403">Essa configuração de segurança permite que um cliente exigir a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="75563-403">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="75563-404">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="75563-404">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="75563-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="75563-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="75563-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="75563-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="75563-407">Essa configuração de segurança permite que um servidor exigir a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="75563-407">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="75563-408">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="75563-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="75563-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="75563-409">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="75563-410">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="75563-410">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="75563-411">Essa configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede.</span><span class="sxs-lookup"><span data-stu-id="75563-411">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="75563-412">Os possíveis valores são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="75563-412">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="75563-413">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="75563-413">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="75563-414">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-414">Boolean</span></span>|<span data-ttu-id="75563-415">Se habilitado, o cliente SMB permitirá logons de convidados inseguros.</span><span class="sxs-lookup"><span data-stu-id="75563-415">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="75563-416">Se não estiver configurado, o cliente SMB rejeitará logons de convidados inseguros.</span><span class="sxs-lookup"><span data-stu-id="75563-416">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="75563-417">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="75563-417">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="75563-418">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-418">Boolean</span></span>|<span data-ttu-id="75563-419">Essa configuração de segurança determina se o arquivo de página de memória virtual é limpo quando o sistema é desligado.</span><span class="sxs-lookup"><span data-stu-id="75563-419">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="75563-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="75563-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="75563-421">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-421">Boolean</span></span>|<span data-ttu-id="75563-422">Essa configuração de segurança determina se um computador pode ser desligado sem precisar fazer logoff no Windows.</span><span class="sxs-lookup"><span data-stu-id="75563-422">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="75563-423">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="75563-423">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="75563-424">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-424">Boolean</span></span>|<span data-ttu-id="75563-425">Permitir que aplicativos UIAccess solicitarem elevação sem usar a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="75563-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="75563-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="75563-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="75563-427">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-427">Boolean</span></span>|<span data-ttu-id="75563-428">Virtualizar falhas de gravação de arquivo e registro em locais de usuário</span><span class="sxs-lookup"><span data-stu-id="75563-428">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="75563-429">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="75563-429">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="75563-430">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-430">Boolean</span></span>|<span data-ttu-id="75563-431">Impor a validação do caminho de certificação PKI para um determinado arquivo executável antes que ele seja autorizado a ser executado.</span><span class="sxs-lookup"><span data-stu-id="75563-431">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="75563-432">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="75563-432">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="75563-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="75563-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="75563-434">Defina o comportamento do prompt de elevação para administradores no Modo de Aprovação do Administrador.</span><span class="sxs-lookup"><span data-stu-id="75563-434">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="75563-435">Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="75563-435">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="75563-436">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="75563-436">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="75563-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="75563-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="75563-438">Defina o comportamento do prompt de elevação para usuários padrão.</span><span class="sxs-lookup"><span data-stu-id="75563-438">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="75563-439">Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="75563-439">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="75563-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="75563-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="75563-441">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-441">Boolean</span></span>|<span data-ttu-id="75563-442">Habilita todas as solicitações de elevação para ir para a área de trabalho do usuário interativo em vez da área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="75563-442">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="75563-443">Configurações de política de comportamento de prompt para administradores e usuários padrão são usadas.</span><span class="sxs-lookup"><span data-stu-id="75563-443">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="75563-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="75563-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="75563-445">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-445">Boolean</span></span>|<span data-ttu-id="75563-446">Instalações de aplicativos que exigem privilégios elevados solicitarão credenciais de administrador. O padrão está habilitado</span><span class="sxs-lookup"><span data-stu-id="75563-446">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="75563-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="75563-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="75563-448">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-448">Boolean</span></span>|<span data-ttu-id="75563-449">Permitir que aplicativos UIAccess solicitarem elevação sem usar a área de trabalho segura. O padrão está habilitado</span><span class="sxs-lookup"><span data-stu-id="75563-449">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="75563-450">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="75563-450">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="75563-451">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-451">Boolean</span></span>|<span data-ttu-id="75563-452">Define se a conta de administrador integrado usa o Modo de Aprovação do Administrador ou executa todos os aplicativos com privilégios de administrador completos. O padrão está habilitado</span><span class="sxs-lookup"><span data-stu-id="75563-452">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="75563-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="75563-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="75563-454">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-454">Boolean</span></span>|<span data-ttu-id="75563-455">Definir se o Modo de Aprovação de Administrador e todas as configurações de política UAC estão habilitadas, o padrão está habilitado</span><span class="sxs-lookup"><span data-stu-id="75563-455">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="75563-456">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="75563-456">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="75563-457">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="75563-457">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="75563-458">Configure as informações do usuário exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="75563-458">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="75563-459">Se não estiver configurado, o nome de exibição do usuário, o domínio e o nome de usuário serão mostrados.</span><span class="sxs-lookup"><span data-stu-id="75563-459">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="75563-460">Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="75563-460">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="75563-461">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="75563-461">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="75563-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="75563-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="75563-463">Configure as informações do usuário exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="75563-463">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="75563-464">Se não estiver configurado, o nome de exibição do usuário, o domínio e o nome de usuário serão mostrados.</span><span class="sxs-lookup"><span data-stu-id="75563-464">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="75563-465">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="75563-465">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="75563-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="75563-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="75563-467">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-467">Boolean</span></span>|<span data-ttu-id="75563-468">Essa configuração de segurança determina se o cliente SMB tenta negociar a assinatura de pacote SMB.</span><span class="sxs-lookup"><span data-stu-id="75563-468">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="75563-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="75563-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="75563-470">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-470">Boolean</span></span>|<span data-ttu-id="75563-471">Essa configuração de segurança determina se a assinatura de pacote é necessária pelo componente cliente SMB.</span><span class="sxs-lookup"><span data-stu-id="75563-471">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="75563-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="75563-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="75563-473">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-473">Boolean</span></span>|<span data-ttu-id="75563-474">Se essa configuração de segurança estiver habilitada, o redirecionador de bloco de mensagens do servidor (SMB) poderá enviar senhas de texto sem formatação para servidores não Microsoft SMB que não suportam criptografia de senha durante a autenticação.</span><span class="sxs-lookup"><span data-stu-id="75563-474">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="75563-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="75563-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="75563-476">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-476">Boolean</span></span>|<span data-ttu-id="75563-477">Essa configuração de segurança determina se a assinatura de pacote é necessária pelo componente de servidor SMB.</span><span class="sxs-lookup"><span data-stu-id="75563-477">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="75563-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="75563-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="75563-479">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-479">Boolean</span></span>|<span data-ttu-id="75563-480">Essa configuração de segurança determina se o servidor SMB negociará a assinatura de pacotes SMB com clientes que o solicitam.</span><span class="sxs-lookup"><span data-stu-id="75563-480">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="75563-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="75563-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="75563-482">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-482">Boolean</span></span>|<span data-ttu-id="75563-483">Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e canalização às configurações de pipes nomeados que podem ser acessados anonimamente e Compartilhamentos que podem ser acessados anonimamente</span><span class="sxs-lookup"><span data-stu-id="75563-483">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="75563-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="75563-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="75563-485">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-485">Boolean</span></span>|<span data-ttu-id="75563-486">Essa configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas com o computador.</span><span class="sxs-lookup"><span data-stu-id="75563-486">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="75563-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="75563-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="75563-488">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-488">Boolean</span></span>|<span data-ttu-id="75563-489">Essa configuração de segurança determina se os usuários anônimos podem executar determinadas atividades, como enumerar os nomes de contas de domínio e compartilhamentos de rede.</span><span class="sxs-lookup"><span data-stu-id="75563-489">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="75563-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="75563-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="75563-491">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-491">Boolean</span></span>|<span data-ttu-id="75563-492">Essa configuração de segurança determina se, na próxima alteração de senha, o valor de hash do Gerenciador de LAN (LM) da nova senha será armazenado.</span><span class="sxs-lookup"><span data-stu-id="75563-492">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="75563-493">Ele não é armazenado por padrão.</span><span class="sxs-lookup"><span data-stu-id="75563-493">It’s not stored by default.</span></span>|
|<span data-ttu-id="75563-494">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="75563-494">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="75563-495">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="75563-495">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="75563-496">Essa configuração de segurança determina o que acontece quando o cartão inteligente para um usuário conectado é removido do leitor de cartão inteligente.</span><span class="sxs-lookup"><span data-stu-id="75563-496">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="75563-497">Os valores possíveis são: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="75563-497">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="75563-498">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="75563-498">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="75563-499">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-499">Boolean</span></span>|<span data-ttu-id="75563-500">Usado para desabilitar a exibição da área de proteção do aplicativo e do navegador.</span><span class="sxs-lookup"><span data-stu-id="75563-500">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="75563-501">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="75563-501">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="75563-502">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-502">Boolean</span></span>|<span data-ttu-id="75563-503">Usado para desabilitar a exibição da área de opções da família.</span><span class="sxs-lookup"><span data-stu-id="75563-503">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="75563-504">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="75563-504">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="75563-505">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-505">Boolean</span></span>|<span data-ttu-id="75563-506">Usado para desabilitar a exibição da área de desempenho e de saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75563-506">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="75563-507">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="75563-507">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="75563-508">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-508">Boolean</span></span>|<span data-ttu-id="75563-509">Usado para desabilitar a exibição do firewall e da área de proteção de rede.</span><span class="sxs-lookup"><span data-stu-id="75563-509">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="75563-510">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="75563-510">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="75563-511">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-511">Boolean</span></span>|<span data-ttu-id="75563-512">Usado para desabilitar a exibição da área de proteção contra vírus e ameaças.</span><span class="sxs-lookup"><span data-stu-id="75563-512">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="75563-513">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="75563-513">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="75563-514">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-514">Boolean</span></span>|<span data-ttu-id="75563-515">Usado para desabilitar a exibição da área de proteção da conta.</span><span class="sxs-lookup"><span data-stu-id="75563-515">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="75563-516">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="75563-516">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="75563-517">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-517">Boolean</span></span>|<span data-ttu-id="75563-518">Usado para desabilitar a exibição do botão Limpar TPM.</span><span class="sxs-lookup"><span data-stu-id="75563-518">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="75563-519">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="75563-519">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="75563-520">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-520">Boolean</span></span>|<span data-ttu-id="75563-521">Usado para desabilitar a exibição da área de proteção de hardware.</span><span class="sxs-lookup"><span data-stu-id="75563-521">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="75563-522">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="75563-522">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="75563-523">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-523">Boolean</span></span>|<span data-ttu-id="75563-524">Usado para desabilitar a exibição do controle de área de notificação.</span><span class="sxs-lookup"><span data-stu-id="75563-524">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="75563-525">O usuário precisa sair e entrar ou reiniciar o computador para que essa configuração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="75563-525">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="75563-526">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="75563-526">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="75563-527">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-527">Boolean</span></span>|<span data-ttu-id="75563-528">Usado para desabilitar a exibição da área de proteção de ransomware.</span><span class="sxs-lookup"><span data-stu-id="75563-528">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="75563-529">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="75563-529">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="75563-530">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-530">Boolean</span></span>|<span data-ttu-id="75563-531">Usado para desabilitar a exibição da área de inicialização segura em Segurança do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75563-531">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="75563-532">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="75563-532">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="75563-533">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-533">Boolean</span></span>|<span data-ttu-id="75563-534">Usado para desabilitar a exibição da solução de problemas do processo de segurança em Segurança do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75563-534">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="75563-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="75563-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="75563-536">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-536">Boolean</span></span>|<span data-ttu-id="75563-537">Usado para desabilitar a exibição do firmware TPM de atualização quando um firmware vulnerável é detectado.</span><span class="sxs-lookup"><span data-stu-id="75563-537">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="75563-538">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="75563-538">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="75563-539">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-539">String</span></span>|<span data-ttu-id="75563-540">O nome da empresa que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="75563-540">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="75563-541">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="75563-541">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="75563-542">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-542">String</span></span>|<span data-ttu-id="75563-543">O endereço de email que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="75563-543">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="75563-544">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="75563-544">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="75563-545">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-545">String</span></span>|<span data-ttu-id="75563-546">O número de telefone ou a ID do Skype que é exibida para os usuários.</span><span class="sxs-lookup"><span data-stu-id="75563-546">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="75563-547">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="75563-547">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="75563-548">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-548">String</span></span>|<span data-ttu-id="75563-549">A URL do portal de ajuda exibida para os usuários.</span><span class="sxs-lookup"><span data-stu-id="75563-549">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="75563-550">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="75563-550">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="75563-551">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="75563-551">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="75563-552">Notificações a ser exibidas nas áreas exibidas do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="75563-552">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="75563-553">Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="75563-553">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="75563-554">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="75563-554">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="75563-555">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="75563-555">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="75563-556">Configure onde exibir informações de contato de IT para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="75563-556">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="75563-557">Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="75563-557">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="75563-558">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="75563-558">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="75563-559">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="75563-559">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="75563-560">Configure as configurações do Windows Defender TamperProtection.</span><span class="sxs-lookup"><span data-stu-id="75563-560">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="75563-561">Os valores possíveis são: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-561">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="75563-562">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="75563-562">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="75563-563">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-563">Boolean</span></span>|<span data-ttu-id="75563-564">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="75563-564">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="75563-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="75563-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="75563-566">Int32</span><span class="sxs-lookup"><span data-stu-id="75563-566">Int32</span></span>|<span data-ttu-id="75563-567">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="75563-567">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="75563-568">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="75563-568">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="75563-569">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="75563-569">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="75563-570">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="75563-570">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="75563-571">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="75563-571">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="75563-572">Selecione a codificação de tecla pré-compartilhada a ser usada.</span><span class="sxs-lookup"><span data-stu-id="75563-572">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="75563-573">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="75563-573">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="75563-574">firewallIPSecExemptionsNone</span><span class="sxs-lookup"><span data-stu-id="75563-574">firewallIPSecExemptionsNone</span></span>|<span data-ttu-id="75563-575">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-575">Boolean</span></span>|<span data-ttu-id="75563-576">Configura isenções IPSec para nenhuma isenção</span><span class="sxs-lookup"><span data-stu-id="75563-576">Configures IPSec exemptions to no exemptions</span></span>|
|<span data-ttu-id="75563-577">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="75563-577">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="75563-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-578">Boolean</span></span>|<span data-ttu-id="75563-579">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="75563-579">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="75563-580">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="75563-580">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="75563-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-581">Boolean</span></span>|<span data-ttu-id="75563-582">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="75563-582">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="75563-583">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="75563-583">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="75563-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-584">Boolean</span></span>|<span data-ttu-id="75563-585">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="75563-585">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="75563-586">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="75563-586">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="75563-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-587">Boolean</span></span>|<span data-ttu-id="75563-588">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="75563-588">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="75563-589">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="75563-589">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="75563-590">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="75563-590">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="75563-591">Especifique como a lista de revogações de certificados deve ser imposta.</span><span class="sxs-lookup"><span data-stu-id="75563-591">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="75563-592">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="75563-592">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="75563-593">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="75563-593">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="75563-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-594">Boolean</span></span>|<span data-ttu-id="75563-595">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="75563-595">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="75563-596">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="75563-596">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="75563-597">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="75563-597">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="75563-598">Configura como a fila de pacotes deve ser aplicada no cenário de gateway de túnel.</span><span class="sxs-lookup"><span data-stu-id="75563-598">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="75563-599">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="75563-599">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="75563-600">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="75563-600">firewallProfileDomain</span></span>|[<span data-ttu-id="75563-601">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="75563-601">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="75563-602">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="75563-602">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="75563-603">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="75563-603">firewallProfilePublic</span></span>|[<span data-ttu-id="75563-604">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="75563-604">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="75563-605">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="75563-605">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="75563-606">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="75563-606">firewallProfilePrivate</span></span>|[<span data-ttu-id="75563-607">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="75563-607">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="75563-608">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="75563-608">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="75563-609">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="75563-609">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="75563-610">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-610">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-611">Valor que indica o comportamento do Adobe Reader da criação de processos filho.</span><span class="sxs-lookup"><span data-stu-id="75563-611">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="75563-612">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-612">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-613">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="75563-613">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="75563-614">String collection</span><span class="sxs-lookup"><span data-stu-id="75563-614">String collection</span></span>|<span data-ttu-id="75563-615">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="75563-615">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="75563-616">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="75563-616">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="75563-617">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="75563-617">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="75563-618">Valor que indica o comportamento dos aplicativos do Office injetando em outros processos.</span><span class="sxs-lookup"><span data-stu-id="75563-618">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="75563-619">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-619">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="75563-620">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="75563-620">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="75563-621">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-621">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-622">Valor que indica o comportamento dos aplicativos do Office injetando em outros processos.</span><span class="sxs-lookup"><span data-stu-id="75563-622">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="75563-623">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-623">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-624">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="75563-624">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="75563-625">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-626">Valor que indica o comportamento dos aplicativos de comunicação do Office, incluindo o Microsoft Outlook, da criação de processos filho.</span><span class="sxs-lookup"><span data-stu-id="75563-626">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="75563-627">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-627">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-628">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="75563-628">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="75563-629">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="75563-629">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="75563-630">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="75563-630">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="75563-631">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-631">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="75563-632">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="75563-632">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="75563-633">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-633">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-634">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="75563-634">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="75563-635">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-635">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-636">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="75563-636">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="75563-637">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="75563-637">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="75563-638">Valor que indica o comportamento do aplicativo do Office iniciando processos filho.</span><span class="sxs-lookup"><span data-stu-id="75563-638">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="75563-639">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-639">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="75563-640">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="75563-640">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="75563-641">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-641">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-642">Valor que indica o comportamento do aplicativo do Office iniciando processos filho.</span><span class="sxs-lookup"><span data-stu-id="75563-642">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="75563-643">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-643">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-644">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="75563-644">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="75563-645">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="75563-645">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="75563-646">Valor que indica o comportamento das importações win32 do código macro no Office.</span><span class="sxs-lookup"><span data-stu-id="75563-646">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="75563-647">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-647">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="75563-648">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="75563-648">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="75563-649">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-649">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-650">Valor que indica o comportamento das importações win32 do código macro no Office.</span><span class="sxs-lookup"><span data-stu-id="75563-650">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="75563-651">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-651">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-652">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="75563-652">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="75563-653">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="75563-653">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="75563-654">Valor que indica o comportamento do código js/vbs/ps/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="75563-654">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="75563-655">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-655">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="75563-656">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="75563-656">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="75563-657">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-657">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-658">Valor que indica o comportamento do código js/vbs/ps/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="75563-658">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="75563-659">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-659">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-660">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="75563-660">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="75563-661">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="75563-661">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="75563-662">Valor que indica o comportamento dos js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="75563-662">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="75563-663">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-663">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="75563-664">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="75563-664">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="75563-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-666">Valor que indica o comportamento dos js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="75563-666">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="75563-667">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-667">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-668">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="75563-668">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="75563-669">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-669">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-670">Valor que indica se o roubo de credenciais do subsistema da autoridade de segurança local do Windows é permitido.</span><span class="sxs-lookup"><span data-stu-id="75563-670">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="75563-671">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-671">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-672">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="75563-672">defenderProcessCreationType</span></span>|[<span data-ttu-id="75563-673">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="75563-673">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="75563-674">Valor que indica a resposta a criações de processo provenientes de comandos PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="75563-674">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="75563-675">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-675">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="75563-676">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="75563-676">defenderProcessCreation</span></span>|[<span data-ttu-id="75563-677">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-677">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-678">Valor que indica a resposta a criações de processo provenientes de comandos PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="75563-678">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="75563-679">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-679">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-680">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="75563-680">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="75563-681">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="75563-681">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="75563-682">Valor que indica resposta a processos não assinados e não assinados executados a partir do USB.</span><span class="sxs-lookup"><span data-stu-id="75563-682">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="75563-683">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-683">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="75563-684">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="75563-684">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="75563-685">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-685">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-686">Valor que indica resposta a processos não assinados e não assinados executados a partir do USB.</span><span class="sxs-lookup"><span data-stu-id="75563-686">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="75563-687">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-687">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-688">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="75563-688">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="75563-689">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="75563-689">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="75563-690">Valor que indica a resposta a executáveis que não atendem a uma prevalência, idade ou critérios de lista confiáveis.</span><span class="sxs-lookup"><span data-stu-id="75563-690">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="75563-691">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-691">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="75563-692">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="75563-692">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="75563-693">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-693">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-694">Valor que indica a resposta a executáveis que não atendem a uma prevalência, idade ou critérios de lista confiáveis.</span><span class="sxs-lookup"><span data-stu-id="75563-694">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="75563-695">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-695">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-696">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="75563-696">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="75563-697">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="75563-697">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="75563-698">Valor que indica se a execução de conteúdo executável (exe, dll, ps, js, vbs, etc) deve ser retirada do email (webmail/email-client).</span><span class="sxs-lookup"><span data-stu-id="75563-698">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="75563-699">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-699">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="75563-700">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="75563-700">defenderEmailContentExecution</span></span>|[<span data-ttu-id="75563-701">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-701">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-702">Valor que indica se a execução de conteúdo executável (exe, dll, ps, js, vbs, etc) deve ser retirada do email (webmail/email-client).</span><span class="sxs-lookup"><span data-stu-id="75563-702">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="75563-703">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-703">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-704">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-704">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="75563-705">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-705">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-706">Valor que indica o uso de proteção avançada contra ransomeware.</span><span class="sxs-lookup"><span data-stu-id="75563-706">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="75563-707">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-707">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-708">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="75563-708">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="75563-709">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-709">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="75563-710">Valor que indica o comportamento das pastas protegidas.</span><span class="sxs-lookup"><span data-stu-id="75563-710">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="75563-711">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="75563-711">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="75563-712">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="75563-712">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="75563-713">String collection</span><span class="sxs-lookup"><span data-stu-id="75563-713">String collection</span></span>|<span data-ttu-id="75563-714">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="75563-714">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="75563-715">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="75563-715">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="75563-716">String collection</span><span class="sxs-lookup"><span data-stu-id="75563-716">String collection</span></span>|<span data-ttu-id="75563-717">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="75563-717">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="75563-718">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-718">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="75563-719">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-719">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-720">Valor que indica o comportamento de NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="75563-720">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="75563-721">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-721">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-722">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="75563-722">defenderExploitProtectionXml</span></span>|<span data-ttu-id="75563-723">Binária</span><span class="sxs-lookup"><span data-stu-id="75563-723">Binary</span></span>|<span data-ttu-id="75563-724">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="75563-724">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="75563-725">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="75563-725">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="75563-726">String</span><span class="sxs-lookup"><span data-stu-id="75563-726">String</span></span>|<span data-ttu-id="75563-727">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="75563-727">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="75563-728">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="75563-728">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="75563-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-729">Boolean</span></span>|<span data-ttu-id="75563-730">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="75563-730">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="75563-731">defenderBlockPersistenceThroughWmiType</span><span class="sxs-lookup"><span data-stu-id="75563-731">defenderBlockPersistenceThroughWmiType</span></span>|[<span data-ttu-id="75563-732">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="75563-732">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="75563-733">Valor que indica o comportamento de persistência de bloqueio por meio da assinatura de evento WMI.</span><span class="sxs-lookup"><span data-stu-id="75563-733">Value indicating the behavior of Block persistence through WMI event subscription.</span></span> <span data-ttu-id="75563-734">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-734">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="75563-735">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="75563-735">appLockerApplicationControl</span></span>|[<span data-ttu-id="75563-736">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="75563-736">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="75563-737">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="75563-737">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="75563-738">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="75563-738">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="75563-739">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="75563-739">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="75563-740">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="75563-740">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="75563-741">Ative o Credential Guard quando o nível de segurança da plataforma com Inicialização Segura e Segurança Baseada em Virtualização estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="75563-741">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="75563-742">Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="75563-742">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.</span></span>|
|<span data-ttu-id="75563-743">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="75563-743">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="75563-744">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-744">Boolean</span></span>|<span data-ttu-id="75563-745">A liga o VBS (Virtualization Based Security).</span><span class="sxs-lookup"><span data-stu-id="75563-745">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="75563-746">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="75563-746">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="75563-747">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-747">Boolean</span></span>|<span data-ttu-id="75563-748">Essa propriedade será preterida em maio de 2019 e será substituída pela propriedade DeviceGuardSecureBootWithDMA.</span><span class="sxs-lookup"><span data-stu-id="75563-748">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="75563-749">Especifica se o Nível de Segurança da Plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="75563-749">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="75563-750">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="75563-750">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="75563-751">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="75563-751">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="75563-752">Especifica se o Nível de Segurança da Plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="75563-752">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="75563-753">Os valores possíveis são: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="75563-753">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="75563-754">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="75563-754">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="75563-755">enablement</span><span class="sxs-lookup"><span data-stu-id="75563-755">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="75563-756">Permite que o administrador de IT configure o lançamento do System Guard.</span><span class="sxs-lookup"><span data-stu-id="75563-756">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="75563-757">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="75563-757">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="75563-758">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="75563-758">smartScreenEnableInShell</span></span>|<span data-ttu-id="75563-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-759">Boolean</span></span>|<span data-ttu-id="75563-760">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="75563-760">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="75563-761">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="75563-761">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="75563-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-762">Boolean</span></span>|<span data-ttu-id="75563-763">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="75563-763">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="75563-764">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="75563-764">applicationGuardEnabled</span></span>|<span data-ttu-id="75563-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-765">Boolean</span></span>|<span data-ttu-id="75563-766">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="75563-766">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="75563-767">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="75563-767">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="75563-768">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="75563-768">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="75563-769">Habilita Windows Defender Application Guard para builds mais novas do Windows.</span><span class="sxs-lookup"><span data-stu-id="75563-769">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="75563-770">Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="75563-770">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="75563-771">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="75563-771">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="75563-772">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="75563-772">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="75563-773">Bloqueie a área de transferência de arquivo de imagem, arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="75563-773">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="75563-774">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="75563-774">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="75563-775">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="75563-775">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="75563-776">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-776">Boolean</span></span>|<span data-ttu-id="75563-777">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="75563-777">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="75563-778">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="75563-778">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="75563-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-779">Boolean</span></span>|<span data-ttu-id="75563-780">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="75563-780">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="75563-781">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="75563-781">applicationGuardForceAuditing</span></span>|<span data-ttu-id="75563-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-782">Boolean</span></span>|<span data-ttu-id="75563-783">A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)</span><span class="sxs-lookup"><span data-stu-id="75563-783">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="75563-784">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="75563-784">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="75563-785">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="75563-785">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="75563-786">Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="75563-786">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="75563-787">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="75563-787">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="75563-788">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="75563-788">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="75563-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-789">Boolean</span></span>|<span data-ttu-id="75563-790">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="75563-790">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="75563-791">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="75563-791">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="75563-792">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-792">Boolean</span></span>|<span data-ttu-id="75563-793">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="75563-793">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="75563-794">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="75563-794">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="75563-795">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-795">Boolean</span></span>|<span data-ttu-id="75563-796">Permitir a impressão em impressoras locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="75563-796">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="75563-797">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="75563-797">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="75563-798">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-798">Boolean</span></span>|<span data-ttu-id="75563-799">Permitir a impressão em impressoras da rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="75563-799">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="75563-800">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="75563-800">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="75563-801">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-801">Boolean</span></span>|<span data-ttu-id="75563-802">Permitir que o application guard use GPU virtual</span><span class="sxs-lookup"><span data-stu-id="75563-802">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="75563-803">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="75563-803">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="75563-804">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-804">Boolean</span></span>|<span data-ttu-id="75563-805">Permitir que os usuários baixem arquivos do Edge no contêiner do application guard e salve-os no sistema de arquivos host</span><span class="sxs-lookup"><span data-stu-id="75563-805">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="75563-806">applicationGuardAllowCameraMicrophoneRedirection</span><span class="sxs-lookup"><span data-stu-id="75563-806">applicationGuardAllowCameraMicrophoneRedirection</span></span>|<span data-ttu-id="75563-807">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-807">Boolean</span></span>|<span data-ttu-id="75563-808">Obtém ou define se os aplicativos dentro do Microsoft Defender Application Guard podem acessar a câmera e o microfone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="75563-808">Gets or sets whether applications inside Microsoft Defender Application Guard can access the device’s camera and microphone.</span></span>|
|<span data-ttu-id="75563-809">applicationGuardCertificateThumbprints</span><span class="sxs-lookup"><span data-stu-id="75563-809">applicationGuardCertificateThumbprints</span></span>|<span data-ttu-id="75563-810">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="75563-810">String collection</span></span>|<span data-ttu-id="75563-811">Permite que determinados Certificados Raiz de nível de dispositivo sejam compartilhados com o contêiner do Microsoft Defender Application Guard.</span><span class="sxs-lookup"><span data-stu-id="75563-811">Allows certain device level Root Certificates to be shared with the Microsoft Defender Application Guard container.</span></span>|
|<span data-ttu-id="75563-812">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="75563-812">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="75563-813">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-813">Boolean</span></span>|<span data-ttu-id="75563-814">Permite que o administrador permita que os usuários padrão habilitam a encrpytion durante a entrada do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="75563-814">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="75563-815">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="75563-815">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="75563-816">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-816">Boolean</span></span>|<span data-ttu-id="75563-817">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="75563-817">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="75563-818">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="75563-818">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="75563-819">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-819">Boolean</span></span>|<span data-ttu-id="75563-820">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="75563-820">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="75563-821">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="75563-821">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="75563-822">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="75563-822">bitLockerEncryptDevice</span></span>|<span data-ttu-id="75563-823">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-823">Boolean</span></span>|<span data-ttu-id="75563-824">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="75563-824">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="75563-825">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="75563-825">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="75563-826">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="75563-826">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="75563-827">Política de unidade do sistema BitLocker.</span><span class="sxs-lookup"><span data-stu-id="75563-827">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="75563-828">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="75563-828">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="75563-829">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="75563-829">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="75563-830">Política de Unidade Fixa do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="75563-830">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="75563-831">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="75563-831">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="75563-832">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="75563-832">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="75563-833">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="75563-833">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="75563-834">bitLockerRecoveryPasswordRotation</span><span class="sxs-lookup"><span data-stu-id="75563-834">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="75563-835">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="75563-835">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="75563-836">Essa configuração inicia uma rotação de senha de recuperação orientada pelo cliente após uma recuperação da unidade do sistema operacional (usando bootmgr ou WinRE).</span><span class="sxs-lookup"><span data-stu-id="75563-836">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="75563-837">Os valores possíveis são: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span><span class="sxs-lookup"><span data-stu-id="75563-837">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|
|<span data-ttu-id="75563-838">defenderDisableScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="75563-838">defenderDisableScanArchiveFiles</span></span>|<span data-ttu-id="75563-839">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-839">Boolean</span></span>|<span data-ttu-id="75563-840">Permite ou não a verificação de arquivos.</span><span class="sxs-lookup"><span data-stu-id="75563-840">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="75563-841">defenderAllowScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="75563-841">defenderAllowScanArchiveFiles</span></span>|<span data-ttu-id="75563-842">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-842">Boolean</span></span>|<span data-ttu-id="75563-843">Permite ou não a verificação de arquivos.</span><span class="sxs-lookup"><span data-stu-id="75563-843">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="75563-844">defenderDisableBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="75563-844">defenderDisableBehaviorMonitoring</span></span>|<span data-ttu-id="75563-845">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-845">Boolean</span></span>|<span data-ttu-id="75563-846">Permite ou não permite Windows Defender funcionalidade de Monitoramento de Comportamento.</span><span class="sxs-lookup"><span data-stu-id="75563-846">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="75563-847">defenderAllowBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="75563-847">defenderAllowBehaviorMonitoring</span></span>|<span data-ttu-id="75563-848">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-848">Boolean</span></span>|<span data-ttu-id="75563-849">Permite ou não permite Windows Defender funcionalidade de Monitoramento de Comportamento.</span><span class="sxs-lookup"><span data-stu-id="75563-849">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="75563-850">defenderDisableCloudProtection</span><span class="sxs-lookup"><span data-stu-id="75563-850">defenderDisableCloudProtection</span></span>|<span data-ttu-id="75563-851">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-851">Boolean</span></span>|<span data-ttu-id="75563-852">Para proteger melhor seu computador, Windows Defender enviará informações à Microsoft sobre todos os problemas encontrados.</span><span class="sxs-lookup"><span data-stu-id="75563-852">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="75563-853">A Microsoft analisará essas informações, aprenderá mais sobre problemas que afetam você e outros clientes e oferecerá soluções aprimoradas.</span><span class="sxs-lookup"><span data-stu-id="75563-853">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="75563-854">defenderAllowCloudProtection</span><span class="sxs-lookup"><span data-stu-id="75563-854">defenderAllowCloudProtection</span></span>|<span data-ttu-id="75563-855">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-855">Boolean</span></span>|<span data-ttu-id="75563-856">Para proteger melhor seu computador, Windows Defender enviará informações à Microsoft sobre todos os problemas encontrados.</span><span class="sxs-lookup"><span data-stu-id="75563-856">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="75563-857">A Microsoft analisará essas informações, aprenderá mais sobre problemas que afetam você e outros clientes e oferecerá soluções aprimoradas.</span><span class="sxs-lookup"><span data-stu-id="75563-857">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="75563-858">defenderEnableScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="75563-858">defenderEnableScanIncomingMail</span></span>|<span data-ttu-id="75563-859">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-859">Boolean</span></span>|<span data-ttu-id="75563-860">Permite ou não permite a verificação de email.</span><span class="sxs-lookup"><span data-stu-id="75563-860">Allows or disallows scanning of email.</span></span>|
|<span data-ttu-id="75563-861">defenderEnableScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="75563-861">defenderEnableScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="75563-862">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-862">Boolean</span></span>|<span data-ttu-id="75563-863">Permite ou não permite uma verificação completa de unidades de rede mapeadas.</span><span class="sxs-lookup"><span data-stu-id="75563-863">Allows or disallows a full scan of mapped network drives.</span></span>|
|<span data-ttu-id="75563-864">defenderDisableScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="75563-864">defenderDisableScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="75563-865">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-865">Boolean</span></span>|<span data-ttu-id="75563-866">Permite ou não permite uma verificação completa de unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="75563-866">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="75563-867">Durante uma verificação rápida, as unidades removíveis ainda podem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="75563-867">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="75563-868">defenderAllowScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="75563-868">defenderAllowScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="75563-869">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-869">Boolean</span></span>|<span data-ttu-id="75563-870">Permite ou não permite uma verificação completa de unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="75563-870">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="75563-871">Durante uma verificação rápida, as unidades removíveis ainda podem ser verificados.</span><span class="sxs-lookup"><span data-stu-id="75563-871">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="75563-872">defenderDisableScanDownloads</span><span class="sxs-lookup"><span data-stu-id="75563-872">defenderDisableScanDownloads</span></span>|<span data-ttu-id="75563-873">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-873">Boolean</span></span>|<span data-ttu-id="75563-874">Permite ou não permite Windows Defender de Proteção do IOAVP.</span><span class="sxs-lookup"><span data-stu-id="75563-874">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="75563-875">defenderAllowScanDownloads</span><span class="sxs-lookup"><span data-stu-id="75563-875">defenderAllowScanDownloads</span></span>|<span data-ttu-id="75563-876">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-876">Boolean</span></span>|<span data-ttu-id="75563-877">Permite ou não permite Windows Defender de Proteção do IOAVP.</span><span class="sxs-lookup"><span data-stu-id="75563-877">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="75563-878">defenderDisableIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="75563-878">defenderDisableIntrusionPreventionSystem</span></span>|<span data-ttu-id="75563-879">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-879">Boolean</span></span>|<span data-ttu-id="75563-880">Permite ou não a funcionalidade Windows Defender Prevenção contra Intrusões.</span><span class="sxs-lookup"><span data-stu-id="75563-880">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="75563-881">defenderAllowIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="75563-881">defenderAllowIntrusionPreventionSystem</span></span>|<span data-ttu-id="75563-882">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-882">Boolean</span></span>|<span data-ttu-id="75563-883">Permite ou não a funcionalidade Windows Defender Prevenção contra Intrusões.</span><span class="sxs-lookup"><span data-stu-id="75563-883">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="75563-884">defenderDisableOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="75563-884">defenderDisableOnAccessProtection</span></span>|<span data-ttu-id="75563-885">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-885">Boolean</span></span>|<span data-ttu-id="75563-886">Permite ou não permite Windows Defender funcionalidade na Proteção do Access.</span><span class="sxs-lookup"><span data-stu-id="75563-886">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="75563-887">defenderAllowOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="75563-887">defenderAllowOnAccessProtection</span></span>|<span data-ttu-id="75563-888">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-888">Boolean</span></span>|<span data-ttu-id="75563-889">Permite ou não permite Windows Defender funcionalidade na Proteção do Access.</span><span class="sxs-lookup"><span data-stu-id="75563-889">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="75563-890">defenderDisableRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="75563-890">defenderDisableRealTimeMonitoring</span></span>|<span data-ttu-id="75563-891">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-891">Boolean</span></span>|<span data-ttu-id="75563-892">Permite ou não permite Windows Defender funcionalidade de Monitoramento em Tempo Real.</span><span class="sxs-lookup"><span data-stu-id="75563-892">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="75563-893">defenderAllowRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="75563-893">defenderAllowRealTimeMonitoring</span></span>|<span data-ttu-id="75563-894">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-894">Boolean</span></span>|<span data-ttu-id="75563-895">Permite ou não permite Windows Defender funcionalidade de Monitoramento em Tempo Real.</span><span class="sxs-lookup"><span data-stu-id="75563-895">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="75563-896">defenderDisableScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="75563-896">defenderDisableScanNetworkFiles</span></span>|<span data-ttu-id="75563-897">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-897">Boolean</span></span>|<span data-ttu-id="75563-898">Permite ou não permite uma verificação de arquivos de rede.</span><span class="sxs-lookup"><span data-stu-id="75563-898">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="75563-899">defenderAllowScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="75563-899">defenderAllowScanNetworkFiles</span></span>|<span data-ttu-id="75563-900">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-900">Boolean</span></span>|<span data-ttu-id="75563-901">Permite ou não permite uma verificação de arquivos de rede.</span><span class="sxs-lookup"><span data-stu-id="75563-901">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="75563-902">defenderDisableScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="75563-902">defenderDisableScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="75563-903">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-903">Boolean</span></span>|<span data-ttu-id="75563-904">Permite ou não Windows Defender funcionalidade de Verificação de Script.</span><span class="sxs-lookup"><span data-stu-id="75563-904">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="75563-905">defenderAllowScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="75563-905">defenderAllowScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="75563-906">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-906">Boolean</span></span>|<span data-ttu-id="75563-907">Permite ou não Windows Defender funcionalidade de Verificação de Script.</span><span class="sxs-lookup"><span data-stu-id="75563-907">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="75563-908">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="75563-908">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="75563-909">Boolean</span><span class="sxs-lookup"><span data-stu-id="75563-909">Boolean</span></span>|<span data-ttu-id="75563-910">Permite ou não permite o acesso do usuário à interface do usuário Windows Defender usuário.</span><span class="sxs-lookup"><span data-stu-id="75563-910">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="75563-911">Se não for permitido, todas as Windows Defender também serão suprimidas.</span><span class="sxs-lookup"><span data-stu-id="75563-911">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="75563-912">defenderAllowEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="75563-912">defenderAllowEndUserAccess</span></span>|<span data-ttu-id="75563-913">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-913">Boolean</span></span>|<span data-ttu-id="75563-914">Permite ou não permite o acesso do usuário à interface do usuário Windows Defender usuário.</span><span class="sxs-lookup"><span data-stu-id="75563-914">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="75563-915">Se não for permitido, todas as Windows Defender também serão suprimidas.</span><span class="sxs-lookup"><span data-stu-id="75563-915">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="75563-916">defenderScanMaxCpuPercentage</span><span class="sxs-lookup"><span data-stu-id="75563-916">defenderScanMaxCpuPercentage</span></span>|<span data-ttu-id="75563-917">Int32</span><span class="sxs-lookup"><span data-stu-id="75563-917">Int32</span></span>|<span data-ttu-id="75563-918">Representa o fator de carga média da CPU para Windows Defender verificação (em porcentagem).</span><span class="sxs-lookup"><span data-stu-id="75563-918">Represents the average CPU load factor for the Windows Defender scan (in percent).</span></span> <span data-ttu-id="75563-919">O valor padrão é 50.</span><span class="sxs-lookup"><span data-stu-id="75563-919">The default value is 50.</span></span> <span data-ttu-id="75563-920">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="75563-920">Valid values 0 to 100</span></span>|
|<span data-ttu-id="75563-921">defenderCheckForSignaturesBeforeRunningScan</span><span class="sxs-lookup"><span data-stu-id="75563-921">defenderCheckForSignaturesBeforeRunningScan</span></span>|<span data-ttu-id="75563-922">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-922">Boolean</span></span>|<span data-ttu-id="75563-923">Essa configuração de política permite que você gerencie se uma verificação de novas definições de vírus e spyware ocorrerá antes de executar uma verificação.</span><span class="sxs-lookup"><span data-stu-id="75563-923">This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.</span></span>|
|<span data-ttu-id="75563-924">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="75563-924">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="75563-925">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="75563-925">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="75563-926">Adicionado ao Windows 10, versão 1709.</span><span class="sxs-lookup"><span data-stu-id="75563-926">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="75563-927">Esta configuração de política determina o quão Windows Defender antivírus será agressivo no bloqueio e verificação de arquivos suspeitos.</span><span class="sxs-lookup"><span data-stu-id="75563-927">This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files.</span></span> <span data-ttu-id="75563-928">O tipo de valor é inteiro.</span><span class="sxs-lookup"><span data-stu-id="75563-928">Value type is integer.</span></span> <span data-ttu-id="75563-929">Esse recurso requer a configuração "Ingressar no Microsoft MAPS" habilitada para funcionar.</span><span class="sxs-lookup"><span data-stu-id="75563-929">This feature requires the "Join Microsoft MAPS" setting enabled in order to function.</span></span> <span data-ttu-id="75563-930">Os valores possíveis são: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span><span class="sxs-lookup"><span data-stu-id="75563-930">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="75563-931">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="75563-931">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="75563-932">Int32</span><span class="sxs-lookup"><span data-stu-id="75563-932">Int32</span></span>|<span data-ttu-id="75563-933">Adicionado ao Windows 10, versão 1709.</span><span class="sxs-lookup"><span data-stu-id="75563-933">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="75563-934">Esse recurso permite que Windows Defender Antivírus bloqueie um arquivo suspeito por até 60 segundos e o digitalizar na nuvem para garantir que ele seja seguro.</span><span class="sxs-lookup"><span data-stu-id="75563-934">This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe.</span></span> <span data-ttu-id="75563-935">O tipo de valor é inteiro, o intervalo é de 0 a 50.</span><span class="sxs-lookup"><span data-stu-id="75563-935">Value type is integer, range is 0 - 50.</span></span> <span data-ttu-id="75563-936">Esse recurso depende de três outras configurações DE MAPAs que devem ser habilitadas: "Configurar o recurso "Bloquear à Primeira Vista"; " Ingressar no Microsoft MAPS"; "Enviar amostras de arquivo quando uma análise posterior for necessária".</span><span class="sxs-lookup"><span data-stu-id="75563-936">This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required".</span></span> <span data-ttu-id="75563-937">Valores válidos de 0 a 50</span><span class="sxs-lookup"><span data-stu-id="75563-937">Valid values 0 to 50</span></span>|
|<span data-ttu-id="75563-938">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="75563-938">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="75563-939">Int32</span><span class="sxs-lookup"><span data-stu-id="75563-939">Int32</span></span>|<span data-ttu-id="75563-940">Período de tempo (em dias) que os itens de quarentena serão armazenados no sistema.</span><span class="sxs-lookup"><span data-stu-id="75563-940">Time period (in days) that quarantine items will be stored on the system.</span></span> <span data-ttu-id="75563-941">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="75563-941">Valid values 0 to 90</span></span>|
|<span data-ttu-id="75563-942">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="75563-942">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="75563-943">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-943">Boolean</span></span>|<span data-ttu-id="75563-944">Essa configuração de política permite configurar verificações de captura para verificações completas agendadas.</span><span class="sxs-lookup"><span data-stu-id="75563-944">This policy setting allows you to configure catch-up scans for scheduled full scans.</span></span> <span data-ttu-id="75563-945">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span><span class="sxs-lookup"><span data-stu-id="75563-945">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="75563-946">Normalmente, essas verificações agendadas são perdidas porque o computador foi desligado no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="75563-946">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="75563-947">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="75563-947">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="75563-948">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-948">Boolean</span></span>|<span data-ttu-id="75563-949">Essa configuração de política permite configurar verificações de recuperação para verificações rápidas agendadas.</span><span class="sxs-lookup"><span data-stu-id="75563-949">This policy setting allows you to configure catch-up scans for scheduled quick scans.</span></span> <span data-ttu-id="75563-950">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span><span class="sxs-lookup"><span data-stu-id="75563-950">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="75563-951">Normalmente, essas verificações agendadas são perdidas porque o computador foi desligado no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="75563-951">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="75563-952">defenderEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="75563-952">defenderEnableLowCpuPriority</span></span>|<span data-ttu-id="75563-953">Booleano</span><span class="sxs-lookup"><span data-stu-id="75563-953">Boolean</span></span>|<span data-ttu-id="75563-954">Essa configuração de política permite habilitar ou desabilitar a baixa prioridade da CPU para verificações agendadas.</span><span class="sxs-lookup"><span data-stu-id="75563-954">This policy setting allows you to enable or disable low CPU priority for scheduled scans.</span></span>|
|<span data-ttu-id="75563-955">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="75563-955">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="75563-956">String collection</span><span class="sxs-lookup"><span data-stu-id="75563-956">String collection</span></span>|<span data-ttu-id="75563-957">Extensões de arquivo a serem excluídas das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="75563-957">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="75563-958">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="75563-958">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="75563-959">String collection</span><span class="sxs-lookup"><span data-stu-id="75563-959">String collection</span></span>|<span data-ttu-id="75563-960">Arquivos e pastas a serem excluídos das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="75563-960">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="75563-961">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="75563-961">defenderProcessesToExclude</span></span>|<span data-ttu-id="75563-962">String collection</span><span class="sxs-lookup"><span data-stu-id="75563-962">String collection</span></span>|<span data-ttu-id="75563-963">Processos a serem excluídos das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="75563-963">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="75563-964">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="75563-964">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="75563-965">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="75563-965">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="75563-966">Adicionado no Windows 10, versão 1607.</span><span class="sxs-lookup"><span data-stu-id="75563-966">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="75563-967">Especifica o nível de detecção de aplicativos potencialmente indesejados (PUAs).</span><span class="sxs-lookup"><span data-stu-id="75563-967">Specifies the level of detection for potentially unwanted applications (PUAs).</span></span> <span data-ttu-id="75563-968">Windows Defender alerta quando um software potencialmente indesejado está sendo baixado ou tenta instalar-se em seu computador.</span><span class="sxs-lookup"><span data-stu-id="75563-968">Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer.</span></span> <span data-ttu-id="75563-969">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="75563-969">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="75563-970">defenderScanDirection</span><span class="sxs-lookup"><span data-stu-id="75563-970">defenderScanDirection</span></span>|[<span data-ttu-id="75563-971">defenderRealtimeScanDirection</span><span class="sxs-lookup"><span data-stu-id="75563-971">defenderRealtimeScanDirection</span></span>](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|<span data-ttu-id="75563-972">Controles que conjuntos de arquivos devem ser monitorados.</span><span class="sxs-lookup"><span data-stu-id="75563-972">Controls which sets of files should be monitored.</span></span> <span data-ttu-id="75563-973">Os valores possíveis são: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span><span class="sxs-lookup"><span data-stu-id="75563-973">Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="75563-974">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="75563-974">defenderScanType</span></span>|[<span data-ttu-id="75563-975">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="75563-975">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="75563-976">Seleciona se será feita uma verificação rápida ou uma verificação completa.</span><span class="sxs-lookup"><span data-stu-id="75563-976">Selects whether to perform a quick scan or full scan.</span></span> <span data-ttu-id="75563-977">Os valores possíveis são: `userDefined`, `disabled`, `quick`, `full`.</span><span class="sxs-lookup"><span data-stu-id="75563-977">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="75563-978">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="75563-978">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="75563-979">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="75563-979">TimeOfDay</span></span>|<span data-ttu-id="75563-980">Seleciona a hora do dia em que a Windows Defender rápida deve ser executado.</span><span class="sxs-lookup"><span data-stu-id="75563-980">Selects the time of day that the Windows Defender quick scan should run.</span></span> <span data-ttu-id="75563-981">Por exemplo, um valor de 0=12:00AM, um valor de 60=1:00AM, um valor de 120=2:00 e assim por diante, até um valor de 1380=11:00PM.</span><span class="sxs-lookup"><span data-stu-id="75563-981">For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM.</span></span> <span data-ttu-id="75563-982">O valor padrão é 120</span><span class="sxs-lookup"><span data-stu-id="75563-982">The default value is 120</span></span>|
|<span data-ttu-id="75563-983">defenderScheduledScanDay</span><span class="sxs-lookup"><span data-stu-id="75563-983">defenderScheduledScanDay</span></span>|[<span data-ttu-id="75563-984">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="75563-984">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="75563-985">Seleciona o dia em que a verificação Windows Defender deve ser executado.</span><span class="sxs-lookup"><span data-stu-id="75563-985">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="75563-986">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="75563-986">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="75563-987">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="75563-987">defenderScheduledScanTime</span></span>|<span data-ttu-id="75563-988">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="75563-988">TimeOfDay</span></span>|<span data-ttu-id="75563-989">Seleciona a hora do dia em que a verificação Windows Defender deve ser executado.</span><span class="sxs-lookup"><span data-stu-id="75563-989">Selects the time of day that the Windows Defender scan should run.</span></span>|
|<span data-ttu-id="75563-990">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="75563-990">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="75563-991">Int32</span><span class="sxs-lookup"><span data-stu-id="75563-991">Int32</span></span>|<span data-ttu-id="75563-992">Especifica o intervalo (em horas) que será usado para verificar assinaturas, portanto, em vez de usar ScheduleDay e ScheduleTime, a verificação de novas assinaturas será definida de acordo com o intervalo.</span><span class="sxs-lookup"><span data-stu-id="75563-992">Specifies the interval (in hours) that will be used to check for signatures, so instead of using the ScheduleDay and ScheduleTime the check for new signatures will be set according to the interval.</span></span> <span data-ttu-id="75563-993">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="75563-993">Valid values 0 to 24</span></span>|
|<span data-ttu-id="75563-994">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="75563-994">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="75563-995">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="75563-995">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="75563-996">Verifica se o nível de consentimento do usuário Windows Defender enviar dados.</span><span class="sxs-lookup"><span data-stu-id="75563-996">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="75563-997">Os valores possíveis são: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span><span class="sxs-lookup"><span data-stu-id="75563-997">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="75563-998">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="75563-998">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="75563-999">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="75563-999">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="75563-1000">Permite que um administrador especifique quaisquer níveis de gravidade de ameaça válidos e a ID de ação padrão correspondente a ser tomada.</span><span class="sxs-lookup"><span data-stu-id="75563-1000">Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.</span></span>|



## <a name="response"></a><span data-ttu-id="75563-1001">Resposta</span><span class="sxs-lookup"><span data-stu-id="75563-1001">Response</span></span>
<span data-ttu-id="75563-1002">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75563-1002">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75563-1003">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75563-1003">Example</span></span>

### <a name="request"></a><span data-ttu-id="75563-1004">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75563-1004">Request</span></span>
<span data-ttu-id="75563-1005">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75563-1005">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 31268

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
  "firewallIPSecExemptionsNone": true,
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
  "defenderBlockPersistenceThroughWmiType": "block",
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
  "applicationGuardAllowCameraMicrophoneRedirection": true,
  "applicationGuardCertificateThumbprints": [
    "Application Guard Certificate Thumbprints value"
  ],
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

### <a name="response"></a><span data-ttu-id="75563-1006">Resposta</span><span class="sxs-lookup"><span data-stu-id="75563-1006">Response</span></span>
<span data-ttu-id="75563-p226">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75563-p226">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 31440

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
  "firewallIPSecExemptionsNone": true,
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
  "defenderBlockPersistenceThroughWmiType": "block",
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
  "applicationGuardAllowCameraMicrophoneRedirection": true,
  "applicationGuardCertificateThumbprints": [
    "Application Guard Certificate Thumbprints value"
  ],
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




