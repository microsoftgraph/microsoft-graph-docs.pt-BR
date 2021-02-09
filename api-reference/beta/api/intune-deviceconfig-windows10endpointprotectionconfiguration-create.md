---
title: Criar windows10EndpointProtectionConfiguration
description: Criar um novo objeto windows10EndpointProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04b1e1a7567d7a2ab63803097c9c84b2046ab411
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154569"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="39d3e-103">Criar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="39d3e-103">Create windows10EndpointProtectionConfiguration</span></span>

<span data-ttu-id="39d3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39d3e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39d3e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39d3e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39d3e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39d3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39d3e-107">Criar um novo objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39d3e-107">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39d3e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="39d3e-108">Prerequisites</span></span>
<span data-ttu-id="39d3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39d3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39d3e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39d3e-111">Permission type</span></span>|<span data-ttu-id="39d3e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="39d3e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39d3e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39d3e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39d3e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39d3e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39d3e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39d3e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39d3e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39d3e-116">Not supported.</span></span>|
|<span data-ttu-id="39d3e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39d3e-117">Application</span></span>|<span data-ttu-id="39d3e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39d3e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39d3e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39d3e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="39d3e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39d3e-120">Request headers</span></span>
|<span data-ttu-id="39d3e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39d3e-121">Header</span></span>|<span data-ttu-id="39d3e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="39d3e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39d3e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="39d3e-123">Authorization</span></span>|<span data-ttu-id="39d3e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39d3e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39d3e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39d3e-125">Accept</span></span>|<span data-ttu-id="39d3e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39d3e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39d3e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39d3e-127">Request body</span></span>
<span data-ttu-id="39d3e-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="39d3e-128">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="39d3e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="39d3e-129">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="39d3e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39d3e-130">Property</span></span>|<span data-ttu-id="39d3e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="39d3e-131">Type</span></span>|<span data-ttu-id="39d3e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="39d3e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39d3e-133">id</span><span class="sxs-lookup"><span data-stu-id="39d3e-133">id</span></span>|<span data-ttu-id="39d3e-134">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-134">String</span></span>|<span data-ttu-id="39d3e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="39d3e-135">Key of the entity.</span></span> <span data-ttu-id="39d3e-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39d3e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39d3e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39d3e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="39d3e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39d3e-138">DateTimeOffset</span></span>|<span data-ttu-id="39d3e-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="39d3e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="39d3e-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39d3e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39d3e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39d3e-141">roleScopeTagIds</span></span>|<span data-ttu-id="39d3e-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="39d3e-142">String collection</span></span>|<span data-ttu-id="39d3e-143">Lista de Marcas de Escopo para esta instância de Entidade.</span><span class="sxs-lookup"><span data-stu-id="39d3e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="39d3e-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39d3e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39d3e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="39d3e-145">supportsScopeTags</span></span>|<span data-ttu-id="39d3e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-146">Boolean</span></span>|<span data-ttu-id="39d3e-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="39d3e-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="39d3e-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvida excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="39d3e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="39d3e-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="39d3e-150">This property is read-only.</span></span> <span data-ttu-id="39d3e-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39d3e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39d3e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="39d3e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="39d3e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="39d3e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="39d3e-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="39d3e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="39d3e-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39d3e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39d3e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="39d3e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="39d3e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="39d3e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="39d3e-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="39d3e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="39d3e-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39d3e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39d3e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="39d3e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="39d3e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="39d3e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="39d3e-162">A regra de aplicabilidade do modo de dispositivo para esta política.</span><span class="sxs-lookup"><span data-stu-id="39d3e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="39d3e-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39d3e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39d3e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39d3e-164">createdDateTime</span></span>|<span data-ttu-id="39d3e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39d3e-165">DateTimeOffset</span></span>|<span data-ttu-id="39d3e-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-166">DateTime the object was created.</span></span> <span data-ttu-id="39d3e-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39d3e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39d3e-168">description</span><span class="sxs-lookup"><span data-stu-id="39d3e-168">description</span></span>|<span data-ttu-id="39d3e-169">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-169">String</span></span>|<span data-ttu-id="39d3e-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39d3e-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39d3e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39d3e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="39d3e-172">displayName</span></span>|<span data-ttu-id="39d3e-173">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-173">String</span></span>|<span data-ttu-id="39d3e-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39d3e-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39d3e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39d3e-176">versão</span><span class="sxs-lookup"><span data-stu-id="39d3e-176">version</span></span>|<span data-ttu-id="39d3e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="39d3e-177">Int32</span></span>|<span data-ttu-id="39d3e-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-178">Version of the device configuration.</span></span> <span data-ttu-id="39d3e-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="39d3e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39d3e-180">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="39d3e-180">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="39d3e-181">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="39d3e-181">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="39d3e-182">Essa política se destina a fornecer segurança adicional contra dispositivos compatíveis com DMA externos.</span><span class="sxs-lookup"><span data-stu-id="39d3e-182">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="39d3e-183">Ele permite mais controle sobre a enumeração de dispositivos externos compatíveis com DMA incompatíveis com isolamento de memória de dispositivo/remapeamento de DMA e áreas de segurança.</span><span class="sxs-lookup"><span data-stu-id="39d3e-183">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="39d3e-184">Essa política só entra em vigor quando a Proteção DMA de Kernel é suportada e habilitada pelo firmware do sistema.</span><span class="sxs-lookup"><span data-stu-id="39d3e-184">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="39d3e-185">A Proteção DMA de Kernel é um recurso de plataforma que não pode ser controlado por meio de política ou por usuário final.</span><span class="sxs-lookup"><span data-stu-id="39d3e-185">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="39d3e-186">Ele deve ser suportado pelo sistema no momento da fabricação.</span><span class="sxs-lookup"><span data-stu-id="39d3e-186">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="39d3e-187">Para verificar se o sistema dá suporte à Proteção de DMA kernel, verifique o campo Proteção DMA kernel na página Resumo do MSINFO32.exe.</span><span class="sxs-lookup"><span data-stu-id="39d3e-187">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="39d3e-188">Os valores possíveis são: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-188">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="39d3e-189">firewallRules</span><span class="sxs-lookup"><span data-stu-id="39d3e-189">firewallRules</span></span>|<span data-ttu-id="39d3e-190">[Coleção windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md)</span><span class="sxs-lookup"><span data-stu-id="39d3e-190">[windowsFirewallRule](../resources/intune-deviceconfig-windowsfirewallrule.md) collection</span></span>|<span data-ttu-id="39d3e-191">Define as configurações de regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="39d3e-191">Configures the firewall rule settings.</span></span> <span data-ttu-id="39d3e-192">Essa coleção pode conter no máximo 150 elementos.</span><span class="sxs-lookup"><span data-stu-id="39d3e-192">This collection can contain a maximum of 150 elements.</span></span>|
|<span data-ttu-id="39d3e-193">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="39d3e-193">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="39d3e-194">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-194">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-195">Esse direito de usuário é usado pelo Gerenciador de Credenciais durante o Backup/Restauração.</span><span class="sxs-lookup"><span data-stu-id="39d3e-195">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="39d3e-196">As credenciais salvas dos usuários poderão ser comprometidas se esse privilégio for dado a outras entidades.</span><span class="sxs-lookup"><span data-stu-id="39d3e-196">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="39d3e-197">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="39d3e-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="39d3e-198">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="39d3e-198">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="39d3e-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-200">Esse direito de usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="39d3e-200">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="39d3e-201">Há suporte para o estado permitido.</span><span class="sxs-lookup"><span data-stu-id="39d3e-201">State Allowed is supported.</span></span>|
|<span data-ttu-id="39d3e-202">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="39d3e-202">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="39d3e-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-204">Esse direito de usuário determina quais usuários e grupos serão bloqueados para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="39d3e-204">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="39d3e-205">Há suporte para o Bloqueio de Estado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-205">State Block is supported.</span></span>|
|<span data-ttu-id="39d3e-206">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="39d3e-206">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="39d3e-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-208">Esse direito de usuário permite que um processo represente qualquer usuário sem autenticação.</span><span class="sxs-lookup"><span data-stu-id="39d3e-208">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="39d3e-209">Portanto, o processo pode obter acesso aos mesmos recursos locais desse usuário.</span><span class="sxs-lookup"><span data-stu-id="39d3e-209">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="39d3e-210">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="39d3e-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="39d3e-211">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="39d3e-211">userRightsLocalLogOn</span></span>|[<span data-ttu-id="39d3e-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-213">Esse direito de usuário determina quais usuários podem fazer logoff no computador.</span><span class="sxs-lookup"><span data-stu-id="39d3e-213">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="39d3e-214">Estados Não Configurados, Permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="39d3e-214">States NotConfigured, Allowed are supported</span></span> |
|<span data-ttu-id="39d3e-215">userRightsDenyLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="39d3e-215">userRightsDenyLocalLogOn</span></span>|[<span data-ttu-id="39d3e-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-217">Esse direito de usuário determina quais usuários não podem fazer logoff no computador.</span><span class="sxs-lookup"><span data-stu-id="39d3e-217">This user right determines which users cannot log on to the computer.</span></span> <span data-ttu-id="39d3e-218">Há suporte para Estados Não Configurados, Bloqueados</span><span class="sxs-lookup"><span data-stu-id="39d3e-218">States NotConfigured, Blocked are supported</span></span> |
|<span data-ttu-id="39d3e-219">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="39d3e-219">userRightsBackupData</span></span>|[<span data-ttu-id="39d3e-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-221">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao fazer o back up de arquivos e diretórios.</span><span class="sxs-lookup"><span data-stu-id="39d3e-221">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="39d3e-222">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="39d3e-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="39d3e-223">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="39d3e-223">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="39d3e-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-225">Esse direito de usuário determina quais usuários e grupos podem alterar a hora e a data no relógio interno do computador.</span><span class="sxs-lookup"><span data-stu-id="39d3e-225">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="39d3e-226">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="39d3e-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="39d3e-227">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="39d3e-227">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="39d3e-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-229">Esta configuração de segurança determina se os usuários podem criar objetos globais que estão disponíveis para todas as sessões.</span><span class="sxs-lookup"><span data-stu-id="39d3e-229">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="39d3e-230">Os usuários que podem criar objetos globais podem afetar processos executados em sessões de outros usuários, o que pode levar a falhas de aplicativos ou corrupção de dados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-230">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="39d3e-231">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="39d3e-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="39d3e-232">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="39d3e-232">userRightsCreatePageFile</span></span>|[<span data-ttu-id="39d3e-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-234">Esse direito de usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de página.</span><span class="sxs-lookup"><span data-stu-id="39d3e-234">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="39d3e-235">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="39d3e-235">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="39d3e-236">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="39d3e-236">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="39d3e-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-238">Esse direito de usuário determina quais contas podem ser usadas por processos para criar um objeto de diretório usando o gerenciador de objetos.</span><span class="sxs-lookup"><span data-stu-id="39d3e-238">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="39d3e-239">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="39d3e-239">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="39d3e-240">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="39d3e-240">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="39d3e-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-242">Esse direito de usuário determina se o usuário pode criar um link simbólico do computador no qual ele está conectado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-242">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="39d3e-243">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="39d3e-243">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="39d3e-244">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="39d3e-244">userRightsCreateToken</span></span>|[<span data-ttu-id="39d3e-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-246">Esse direito de usuário determina quais usuários/grupos podem ser usados por processos para criar um token que pode ser usado para obter acesso a todos os recursos locais quando o processo usa uma API interna para criar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="39d3e-246">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="39d3e-247">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="39d3e-247">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="39d3e-248">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="39d3e-248">userRightsDebugPrograms</span></span>|[<span data-ttu-id="39d3e-249">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-249">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-250">Esse direito de usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel.</span><span class="sxs-lookup"><span data-stu-id="39d3e-250">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="39d3e-251">Somente estados NotConfigured e Allowed são suportados</span><span class="sxs-lookup"><span data-stu-id="39d3e-251">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="39d3e-252">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="39d3e-252">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="39d3e-253">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-253">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-254">Esse direito de usuário determina quais usuários e grupos são proibidos de fazer logons como um cliente de Serviços de Área de Trabalho Remota.</span><span class="sxs-lookup"><span data-stu-id="39d3e-254">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="39d3e-255">Somente estados NotConfigured e Blocked são suportados</span><span class="sxs-lookup"><span data-stu-id="39d3e-255">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="39d3e-256">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="39d3e-256">userRightsDelegation</span></span>|[<span data-ttu-id="39d3e-257">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-257">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-258">Esse direito de usuário determina quais usuários podem definir a configuração Confiável para Delegação em um objeto de usuário ou computador.</span><span class="sxs-lookup"><span data-stu-id="39d3e-258">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="39d3e-259">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-259">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-260">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="39d3e-260">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="39d3e-261">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-261">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-262">Esse direito de usuário determina quais contas podem ser usadas por um processo para adicionar entradas ao log de segurança.</span><span class="sxs-lookup"><span data-stu-id="39d3e-262">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="39d3e-263">O log de segurança é usado para rastrear o acesso não autorizado ao sistema.</span><span class="sxs-lookup"><span data-stu-id="39d3e-263">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="39d3e-264">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-265">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="39d3e-265">userRightsImpersonateClient</span></span>|[<span data-ttu-id="39d3e-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-267">Atribuir esse direito de usuário a um usuário permite que programas executados em nome desse usuário representem um cliente.</span><span class="sxs-lookup"><span data-stu-id="39d3e-267">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="39d3e-268">Exigir esse direito de usuário para esse tipo de representação impede que um usuário não autorizado insuve um cliente para se conectar a um serviço que ele criou e, em seguida, representar esse cliente, o que pode elevar as permissões do usuário não autorizado para níveis administrativos ou do sistema.</span><span class="sxs-lookup"><span data-stu-id="39d3e-268">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="39d3e-269">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-270">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="39d3e-270">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="39d3e-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-272">Esse direito de usuário determina quais contas podem usar um processo com acesso de Propriedade de Gravação a outro processo para aumentar a prioridade de execução atribuída ao outro processo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-272">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="39d3e-273">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-274">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="39d3e-274">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="39d3e-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-276">Esse direito de usuário determina quais usuários podem carregar e descarregar dinamicamente drivers de dispositivo ou outro código no modo kernel.</span><span class="sxs-lookup"><span data-stu-id="39d3e-276">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="39d3e-277">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-278">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="39d3e-278">userRightsLockMemory</span></span>|[<span data-ttu-id="39d3e-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-280">Esse direito de usuário determina quais contas podem usar um processo para manter os dados na memória física, o que impede que o sistema paging os dados para a memória virtual no disco.</span><span class="sxs-lookup"><span data-stu-id="39d3e-280">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="39d3e-281">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-282">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="39d3e-282">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="39d3e-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-284">Esse direito de usuário determina quais usuários podem especificar opções de auditoria de acesso a objetos para recursos individuais, como arquivos, objetos do Active Directory e chaves do Registro.</span><span class="sxs-lookup"><span data-stu-id="39d3e-284">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="39d3e-285">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-286">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="39d3e-286">userRightsManageVolumes</span></span>|[<span data-ttu-id="39d3e-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-288">Esse direito de usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como desfragmentação remota.</span><span class="sxs-lookup"><span data-stu-id="39d3e-288">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="39d3e-289">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-290">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="39d3e-290">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="39d3e-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-292">Esse direito de usuário determina quem pode modificar os valores do ambiente do firmware.</span><span class="sxs-lookup"><span data-stu-id="39d3e-292">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="39d3e-293">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-294">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="39d3e-294">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="39d3e-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-296">Esse direito de usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves do Registro ou processos pertencentes a outros usuários.</span><span class="sxs-lookup"><span data-stu-id="39d3e-296">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="39d3e-297">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-297">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-298">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="39d3e-298">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="39d3e-299">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-299">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-300">Esse direito de usuário determina quais usuários podem usar as ferramentas de monitoramento de desempenho para monitorar o desempenho dos processos do sistema.</span><span class="sxs-lookup"><span data-stu-id="39d3e-300">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="39d3e-301">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-301">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-302">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="39d3e-302">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="39d3e-303">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-303">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-304">Esse direito de usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede.</span><span class="sxs-lookup"><span data-stu-id="39d3e-304">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="39d3e-305">O uso indevido desse direito de usuário pode resultar em negação de serviço.</span><span class="sxs-lookup"><span data-stu-id="39d3e-305">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="39d3e-306">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-306">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-307">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="39d3e-307">userRightsRestoreData</span></span>|[<span data-ttu-id="39d3e-308">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-308">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-309">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao restaurar arquivos e diretórios de backup e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto.</span><span class="sxs-lookup"><span data-stu-id="39d3e-309">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="39d3e-310">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-310">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-311">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="39d3e-311">userRightsTakeOwnership</span></span>|[<span data-ttu-id="39d3e-312">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="39d3e-312">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="39d3e-313">Esse direito de usuário determina quais usuários podem assumir a propriedade de qualquer objeto de segurança no sistema, incluindo objetos, arquivos e pastas do Active Directory, impressoras, chaves do Registro, processos e threads.</span><span class="sxs-lookup"><span data-stu-id="39d3e-313">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="39d3e-314">Somente estados NotConfigured e Allowed são suportados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-314">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="39d3e-315">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="39d3e-315">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="39d3e-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-316">Boolean</span></span>|<span data-ttu-id="39d3e-317">Esta configuração determina se o jogo salvar no xbox está habilitado (1) ou desabilitado (0).</span><span class="sxs-lookup"><span data-stu-id="39d3e-317">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="39d3e-318">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="39d3e-318">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="39d3e-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="39d3e-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="39d3e-320">Esta configuração determina se o tipo de início do serviço de gerenciamento de acessórios é Automático(2), Manual(3), Desabilitado(4).</span><span class="sxs-lookup"><span data-stu-id="39d3e-320">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="39d3e-321">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="39d3e-321">Default: Manual.</span></span> <span data-ttu-id="39d3e-322">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="39d3e-323">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="39d3e-323">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="39d3e-324">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="39d3e-324">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="39d3e-325">Esta configuração determina se o tipo de início do serviço Live Auth Manager é Automático(2), Manual(3), Desabilitado(4).</span><span class="sxs-lookup"><span data-stu-id="39d3e-325">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="39d3e-326">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="39d3e-326">Default: Manual.</span></span> <span data-ttu-id="39d3e-327">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-327">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="39d3e-328">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="39d3e-328">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="39d3e-329">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="39d3e-329">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="39d3e-330">Esta configuração determina se o tipo de início do serviço Live Game Save é Automático(2), Manual(3), Desabilitado(4).</span><span class="sxs-lookup"><span data-stu-id="39d3e-330">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="39d3e-331">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="39d3e-331">Default: Manual.</span></span> <span data-ttu-id="39d3e-332">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-332">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="39d3e-333">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="39d3e-333">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="39d3e-334">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="39d3e-334">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="39d3e-335">Esta configuração determina se o tipo de início do serviço de rede é Automático(2), Manual(3), Desabilitado(4).</span><span class="sxs-lookup"><span data-stu-id="39d3e-335">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="39d3e-336">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="39d3e-336">Default: Manual.</span></span> <span data-ttu-id="39d3e-337">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-337">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="39d3e-338">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="39d3e-338">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="39d3e-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-339">Boolean</span></span>|<span data-ttu-id="39d3e-340">Impedir que os usuários adicionem novas contas da Microsoft a este computador.</span><span class="sxs-lookup"><span data-stu-id="39d3e-340">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="39d3e-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="39d3e-341">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="39d3e-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-342">Boolean</span></span>|<span data-ttu-id="39d3e-343">Habilita contas locais que não estão protegidas por senha para fazer logoff de locais que não sejam o dispositivo físico. O padrão está habilitado</span><span class="sxs-lookup"><span data-stu-id="39d3e-343">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="39d3e-344">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="39d3e-344">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="39d3e-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-345">Boolean</span></span>|<span data-ttu-id="39d3e-346">Determina se a conta administrador local está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="39d3e-346">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="39d3e-347">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="39d3e-347">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="39d3e-348">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-348">String</span></span>|<span data-ttu-id="39d3e-349">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "Administrador".</span><span class="sxs-lookup"><span data-stu-id="39d3e-349">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="39d3e-350">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="39d3e-350">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="39d3e-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-351">Boolean</span></span>|<span data-ttu-id="39d3e-352">Determina se a conta de Convidado está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="39d3e-352">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="39d3e-353">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="39d3e-353">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="39d3e-354">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-354">String</span></span>|<span data-ttu-id="39d3e-355">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "Guest".</span><span class="sxs-lookup"><span data-stu-id="39d3e-355">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="39d3e-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="39d3e-356">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="39d3e-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-357">Boolean</span></span>|<span data-ttu-id="39d3e-358">Impedir que um computador portátil seja desaqueado sem precisar fazer logon.</span><span class="sxs-lookup"><span data-stu-id="39d3e-358">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="39d3e-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="39d3e-359">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="39d3e-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-360">Boolean</span></span>|<span data-ttu-id="39d3e-361">Restrinja a instalação de drivers de impressora como parte da conexão a uma impressora compartilhada somente para administradores.</span><span class="sxs-lookup"><span data-stu-id="39d3e-361">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="39d3e-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="39d3e-362">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="39d3e-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-363">Boolean</span></span>|<span data-ttu-id="39d3e-364">A habilitação dessa configuração permite que apenas o usuário conectado interativamente acesse a mídia de CD-ROM.</span><span class="sxs-lookup"><span data-stu-id="39d3e-364">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="39d3e-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="39d3e-365">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="39d3e-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="39d3e-366">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="39d3e-367">Defina quem tem permissão para formatar e ejetar a mídia NTFS removível.</span><span class="sxs-lookup"><span data-stu-id="39d3e-367">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="39d3e-368">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-368">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="39d3e-369">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="39d3e-369">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="39d3e-370">Int32</span><span class="sxs-lookup"><span data-stu-id="39d3e-370">Int32</span></span>|<span data-ttu-id="39d3e-371">Defina o máximo de minutos de inatividade na tela de logon da área de trabalho interativa até que a economia de tela seja executado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-371">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="39d3e-372">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="39d3e-372">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="39d3e-373">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="39d3e-373">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="39d3e-374">Int32</span><span class="sxs-lookup"><span data-stu-id="39d3e-374">Int32</span></span>|<span data-ttu-id="39d3e-375">Defina o máximo de minutos de inatividade na tela de logon da área de trabalho interativa até que a economia de tela seja executado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-375">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="39d3e-376">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="39d3e-376">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="39d3e-377">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="39d3e-377">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="39d3e-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-378">Boolean</span></span>|<span data-ttu-id="39d3e-379">Exigir que CTRL+ALT+DEL seja pressionado antes que um usuário possa fazer logoff.</span><span class="sxs-lookup"><span data-stu-id="39d3e-379">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="39d3e-380">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="39d3e-380">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="39d3e-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-381">Boolean</span></span>|<span data-ttu-id="39d3e-382">Não exibe o nome de usuário da última pessoa que fez login neste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-382">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="39d3e-383">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="39d3e-383">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="39d3e-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-384">Boolean</span></span>|<span data-ttu-id="39d3e-385">Não exibe o nome de usuário da pessoa que entrou nesse dispositivo depois que as credenciais são inseridas e antes que a área de trabalho do dispositivo seja mostrada.</span><span class="sxs-lookup"><span data-stu-id="39d3e-385">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="39d3e-386">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="39d3e-386">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="39d3e-387">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-387">String</span></span>|<span data-ttu-id="39d3e-388">Definir o título da mensagem para os usuários que tentarem entrar.</span><span class="sxs-lookup"><span data-stu-id="39d3e-388">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="39d3e-389">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="39d3e-389">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="39d3e-390">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-390">String</span></span>|<span data-ttu-id="39d3e-391">Definir o texto da mensagem para os usuários que tentarem entrar.</span><span class="sxs-lookup"><span data-stu-id="39d3e-391">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="39d3e-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="39d3e-392">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="39d3e-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-393">Boolean</span></span>|<span data-ttu-id="39d3e-394">Bloquear solicitações de autenticação PKU2U para este dispositivo para usar identidades online.</span><span class="sxs-lookup"><span data-stu-id="39d3e-394">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="39d3e-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="39d3e-395">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="39d3e-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-396">Boolean</span></span>|<span data-ttu-id="39d3e-397">Boolean auxiliar de interface do usuário para a entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="39d3e-397">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="39d3e-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="39d3e-398">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="39d3e-399">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-399">String</span></span>|<span data-ttu-id="39d3e-400">Edite a cadeia de caracteres padrão do Idioma de Definição do Descritor de Segurança para permitir ou negar que usuários e grupos façam chamadas remotas ao SAM.</span><span class="sxs-lookup"><span data-stu-id="39d3e-400">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="39d3e-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="39d3e-401">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="39d3e-402">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="39d3e-402">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="39d3e-403">Essa configuração de segurança permite que um cliente recarde a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="39d3e-403">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="39d3e-404">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-404">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="39d3e-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="39d3e-405">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="39d3e-406">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="39d3e-406">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="39d3e-407">Esta configuração de segurança permite que um servidor exige a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="39d3e-407">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="39d3e-408">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-408">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="39d3e-409">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="39d3e-409">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="39d3e-410">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="39d3e-410">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="39d3e-411">Esta configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede.</span><span class="sxs-lookup"><span data-stu-id="39d3e-411">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="39d3e-412">Os possíveis valores são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-412">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="39d3e-413">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="39d3e-413">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="39d3e-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-414">Boolean</span></span>|<span data-ttu-id="39d3e-415">Se habilitado, o cliente SMB permitirá logons de convidados inseguros.</span><span class="sxs-lookup"><span data-stu-id="39d3e-415">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="39d3e-416">Se não estiver configurado, o cliente SMB rejeitará logons de convidados inseguros.</span><span class="sxs-lookup"><span data-stu-id="39d3e-416">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="39d3e-417">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="39d3e-417">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="39d3e-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-418">Boolean</span></span>|<span data-ttu-id="39d3e-419">Esta configuração de segurança determina se o arquivo de página da memória virtual é limpo quando o sistema é desligado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-419">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="39d3e-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="39d3e-420">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="39d3e-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-421">Boolean</span></span>|<span data-ttu-id="39d3e-422">Esta configuração de segurança determina se um computador pode ser desligado sem ter que fazer logoff no Windows.</span><span class="sxs-lookup"><span data-stu-id="39d3e-422">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="39d3e-423">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="39d3e-423">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="39d3e-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-424">Boolean</span></span>|<span data-ttu-id="39d3e-425">Permita que os aplicativos UIAccess solicitam elevação sem usar a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="39d3e-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="39d3e-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="39d3e-426">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="39d3e-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-427">Boolean</span></span>|<span data-ttu-id="39d3e-428">Virtualizar falhas de gravação de arquivos e do Registro para locais por usuário</span><span class="sxs-lookup"><span data-stu-id="39d3e-428">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="39d3e-429">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="39d3e-429">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="39d3e-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-430">Boolean</span></span>|<span data-ttu-id="39d3e-431">Impor a validação do caminho de certificação PKI para um determinado arquivo executável antes que ele seja permitido para execução.</span><span class="sxs-lookup"><span data-stu-id="39d3e-431">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="39d3e-432">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="39d3e-432">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="39d3e-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="39d3e-433">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="39d3e-434">Defina o comportamento da solicitação de elevação para administradores no Modo de Aprovação de Administrador.</span><span class="sxs-lookup"><span data-stu-id="39d3e-434">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="39d3e-435">Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-435">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="39d3e-436">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="39d3e-436">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="39d3e-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="39d3e-437">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="39d3e-438">Defina o comportamento da solicitação de elevação para usuários padrão.</span><span class="sxs-lookup"><span data-stu-id="39d3e-438">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="39d3e-439">Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-439">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="39d3e-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="39d3e-440">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="39d3e-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-441">Boolean</span></span>|<span data-ttu-id="39d3e-442">Permitir que todas as solicitações de elevação acessem a área de trabalho interativa do usuário em vez da área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="39d3e-442">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="39d3e-443">Configurações de política de comportamento de aviso para administradores e usuários padrão são usadas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-443">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="39d3e-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="39d3e-444">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="39d3e-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-445">Boolean</span></span>|<span data-ttu-id="39d3e-446">Instalações de aplicativos que exigem privilégios elevados solicitarão credenciais de administrador. O padrão está habilitado</span><span class="sxs-lookup"><span data-stu-id="39d3e-446">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="39d3e-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="39d3e-447">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="39d3e-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-448">Boolean</span></span>|<span data-ttu-id="39d3e-449">Permita que os aplicativos UIAccess solicitam elevação sem usar a área de trabalho segura. O padrão está habilitado</span><span class="sxs-lookup"><span data-stu-id="39d3e-449">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="39d3e-450">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="39d3e-450">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="39d3e-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-451">Boolean</span></span>|<span data-ttu-id="39d3e-452">Define se a conta de administrador integrado usa o Modo de Aprovação de Administrador ou executa todos os aplicativos com todos os privilégios de administrador. O padrão está habilitado</span><span class="sxs-lookup"><span data-stu-id="39d3e-452">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="39d3e-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="39d3e-453">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="39d3e-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-454">Boolean</span></span>|<span data-ttu-id="39d3e-455">Definir se o Modo de Aprovação de Administrador e todas as configurações de política do UAC estão habilitados, o padrão está habilitado</span><span class="sxs-lookup"><span data-stu-id="39d3e-455">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="39d3e-456">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="39d3e-456">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="39d3e-457">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="39d3e-457">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="39d3e-458">Configure as informações do usuário exibidas quando a sessão estiver bloqueada.</span><span class="sxs-lookup"><span data-stu-id="39d3e-458">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="39d3e-459">Se não estiver configurado, o nome de exibição do usuário, o domínio e o nome de usuário serão mostrados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-459">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="39d3e-460">Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-460">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="39d3e-461">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="39d3e-461">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="39d3e-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="39d3e-462">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="39d3e-463">Configure as informações do usuário exibidas quando a sessão estiver bloqueada.</span><span class="sxs-lookup"><span data-stu-id="39d3e-463">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="39d3e-464">Se não estiver configurado, o nome de exibição do usuário, o domínio e o nome de usuário serão mostrados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-464">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="39d3e-465">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-465">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="39d3e-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="39d3e-466">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="39d3e-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-467">Boolean</span></span>|<span data-ttu-id="39d3e-468">Esta configuração de segurança determina se o cliente SMB tenta negociar a assinatura de pacote SMB.</span><span class="sxs-lookup"><span data-stu-id="39d3e-468">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="39d3e-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="39d3e-469">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="39d3e-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-470">Boolean</span></span>|<span data-ttu-id="39d3e-471">Esta configuração de segurança determina se a assinatura de pacote é necessária para o componente cliente SMB.</span><span class="sxs-lookup"><span data-stu-id="39d3e-471">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="39d3e-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="39d3e-472">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="39d3e-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-473">Boolean</span></span>|<span data-ttu-id="39d3e-474">Se essa configuração de segurança estiver habilitada, o redirecionador SMB (Bloco de Mensagens do Servidor) poderá enviar senhas de texto sem formatação para servidores SMB que não deem suporte à criptografia de senha durante a autenticação.</span><span class="sxs-lookup"><span data-stu-id="39d3e-474">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="39d3e-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="39d3e-475">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="39d3e-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-476">Boolean</span></span>|<span data-ttu-id="39d3e-477">Esta configuração de segurança determina se a assinatura de pacote é necessária para o componente do servidor SMB.</span><span class="sxs-lookup"><span data-stu-id="39d3e-477">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="39d3e-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="39d3e-478">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="39d3e-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-479">Boolean</span></span>|<span data-ttu-id="39d3e-480">Esta configuração de segurança determina se o servidor SMB negociará a assinatura de pacotes SMB com clientes que o solicitarem.</span><span class="sxs-lookup"><span data-stu-id="39d3e-480">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="39d3e-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="39d3e-481">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="39d3e-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-482">Boolean</span></span>|<span data-ttu-id="39d3e-483">Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e pipes às configurações de pipes nomeados que podem ser acessados anonimamente e Compartilhamentos que podem ser acessados anonimamente</span><span class="sxs-lookup"><span data-stu-id="39d3e-483">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="39d3e-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="39d3e-484">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="39d3e-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-485">Boolean</span></span>|<span data-ttu-id="39d3e-486">Esta configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas com o computador.</span><span class="sxs-lookup"><span data-stu-id="39d3e-486">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="39d3e-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="39d3e-487">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="39d3e-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-488">Boolean</span></span>|<span data-ttu-id="39d3e-489">Esta configuração de segurança determina se usuários anônimos podem realizar determinadas atividades, como enumerar os nomes de contas de domínio e compartilhamentos de rede.</span><span class="sxs-lookup"><span data-stu-id="39d3e-489">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="39d3e-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="39d3e-490">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="39d3e-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-491">Boolean</span></span>|<span data-ttu-id="39d3e-492">Esta configuração de segurança determina se, na próxima alteração de senha, o valor de hash do LAN Manager (LM) para a nova senha será armazenado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-492">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="39d3e-493">Ele não é armazenado por padrão.</span><span class="sxs-lookup"><span data-stu-id="39d3e-493">It’s not stored by default.</span></span>|
|<span data-ttu-id="39d3e-494">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="39d3e-494">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="39d3e-495">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="39d3e-495">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="39d3e-496">Esta configuração de segurança determina o que acontece quando o cartão inteligente de um usuário conectado é removido do leitor de cartão inteligente.</span><span class="sxs-lookup"><span data-stu-id="39d3e-496">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="39d3e-497">Os valores possíveis são: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-497">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="39d3e-498">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-498">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="39d3e-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-499">Boolean</span></span>|<span data-ttu-id="39d3e-500">Usado para desabilitar a exibição da área de proteção do aplicativo e do navegador.</span><span class="sxs-lookup"><span data-stu-id="39d3e-500">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="39d3e-501">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-501">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="39d3e-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-502">Boolean</span></span>|<span data-ttu-id="39d3e-503">Usado para desabilitar a exibição da área de opções da família.</span><span class="sxs-lookup"><span data-stu-id="39d3e-503">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="39d3e-504">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-504">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="39d3e-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-505">Boolean</span></span>|<span data-ttu-id="39d3e-506">Usado para desabilitar a exibição da área de desempenho e saúde do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-506">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="39d3e-507">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-507">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="39d3e-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-508">Boolean</span></span>|<span data-ttu-id="39d3e-509">Usado para desabilitar a exibição da área de proteção de rede e firewall.</span><span class="sxs-lookup"><span data-stu-id="39d3e-509">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="39d3e-510">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-510">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="39d3e-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-511">Boolean</span></span>|<span data-ttu-id="39d3e-512">Usado para desabilitar a exibição da área de proteção contra vírus e ameaças.</span><span class="sxs-lookup"><span data-stu-id="39d3e-512">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="39d3e-513">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-513">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="39d3e-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-514">Boolean</span></span>|<span data-ttu-id="39d3e-515">Usado para desabilitar a exibição da área de proteção da conta.</span><span class="sxs-lookup"><span data-stu-id="39d3e-515">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="39d3e-516">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-516">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="39d3e-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-517">Boolean</span></span>|<span data-ttu-id="39d3e-518">Usado para desabilitar a exibição do botão Limpar TPM.</span><span class="sxs-lookup"><span data-stu-id="39d3e-518">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="39d3e-519">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-519">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="39d3e-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-520">Boolean</span></span>|<span data-ttu-id="39d3e-521">Usado para desabilitar a exibição da área de proteção de hardware.</span><span class="sxs-lookup"><span data-stu-id="39d3e-521">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="39d3e-522">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-522">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="39d3e-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-523">Boolean</span></span>|<span data-ttu-id="39d3e-524">Usado para desabilitar a exibição do controle de área de notificação.</span><span class="sxs-lookup"><span data-stu-id="39d3e-524">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="39d3e-525">O usuário precisa sair e entrar ou reiniciar o computador para que essa configuração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="39d3e-525">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="39d3e-526">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-526">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="39d3e-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-527">Boolean</span></span>|<span data-ttu-id="39d3e-528">Usado para desabilitar a exibição da área de proteção ransomware.</span><span class="sxs-lookup"><span data-stu-id="39d3e-528">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="39d3e-529">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-529">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="39d3e-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-530">Boolean</span></span>|<span data-ttu-id="39d3e-531">Usado para desabilitar a exibição da área de inicialização segura em Segurança do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-531">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="39d3e-532">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-532">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="39d3e-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-533">Boolean</span></span>|<span data-ttu-id="39d3e-534">Usado para desabilitar a exibição da solução de problemas do processo de segurança em Segurança do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-534">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="39d3e-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="39d3e-535">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="39d3e-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-536">Boolean</span></span>|<span data-ttu-id="39d3e-537">Usado para desabilitar a exibição do firmware do TPM de atualização quando um firmware vulnerável é detectado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-537">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="39d3e-538">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="39d3e-538">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="39d3e-539">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-539">String</span></span>|<span data-ttu-id="39d3e-540">O nome da empresa exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="39d3e-540">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="39d3e-541">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="39d3e-541">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="39d3e-542">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-542">String</span></span>|<span data-ttu-id="39d3e-543">O endereço de email exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="39d3e-543">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="39d3e-544">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="39d3e-544">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="39d3e-545">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-545">String</span></span>|<span data-ttu-id="39d3e-546">O número de telefone ou a ID do Skype exibida aos usuários.</span><span class="sxs-lookup"><span data-stu-id="39d3e-546">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="39d3e-547">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="39d3e-547">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="39d3e-548">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-548">String</span></span>|<span data-ttu-id="39d3e-549">A URL do portal de ajuda exibida para os usuários.</span><span class="sxs-lookup"><span data-stu-id="39d3e-549">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="39d3e-550">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="39d3e-550">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="39d3e-551">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="39d3e-551">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="39d3e-552">Notificações para mostrar das áreas exibidas do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-552">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="39d3e-553">Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-553">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="39d3e-554">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="39d3e-554">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="39d3e-555">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="39d3e-555">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="39d3e-556">Configure onde exibir as informações de contato de IT para os usuários finais.</span><span class="sxs-lookup"><span data-stu-id="39d3e-556">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="39d3e-557">Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-557">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="39d3e-558">windowsDefenderTamperProtection</span><span class="sxs-lookup"><span data-stu-id="39d3e-558">windowsDefenderTamperProtection</span></span>|[<span data-ttu-id="39d3e-559">windowsDefenderTamperProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="39d3e-559">windowsDefenderTamperProtectionOptions</span></span>](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|<span data-ttu-id="39d3e-560">Definir as configurações do windows defender TamperProtection.</span><span class="sxs-lookup"><span data-stu-id="39d3e-560">Configure windows defender TamperProtection settings.</span></span> <span data-ttu-id="39d3e-561">Os valores possíveis são: `notConfigured`, `enable`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-561">Possible values are: `notConfigured`, `enable`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-562">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="39d3e-562">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="39d3e-563">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-563">Boolean</span></span>|<span data-ttu-id="39d3e-564">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="39d3e-564">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="39d3e-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="39d3e-565">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="39d3e-566">Int32</span><span class="sxs-lookup"><span data-stu-id="39d3e-566">Int32</span></span>|<span data-ttu-id="39d3e-567">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="39d3e-567">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="39d3e-568">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-568">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="39d3e-569">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="39d3e-569">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="39d3e-570">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="39d3e-570">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="39d3e-571">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="39d3e-571">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="39d3e-572">Selecione a codificação de tecla pré-compartilhada a ser usada.</span><span class="sxs-lookup"><span data-stu-id="39d3e-572">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="39d3e-573">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-573">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="39d3e-574">firewallIPSecExemptionsNone</span><span class="sxs-lookup"><span data-stu-id="39d3e-574">firewallIPSecExemptionsNone</span></span>|<span data-ttu-id="39d3e-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-575">Boolean</span></span>|<span data-ttu-id="39d3e-576">Configura isenções IPSec sem isenções</span><span class="sxs-lookup"><span data-stu-id="39d3e-576">Configures IPSec exemptions to no exemptions</span></span>|
|<span data-ttu-id="39d3e-577">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="39d3e-577">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="39d3e-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-578">Boolean</span></span>|<span data-ttu-id="39d3e-579">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="39d3e-579">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="39d3e-580">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="39d3e-580">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="39d3e-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-581">Boolean</span></span>|<span data-ttu-id="39d3e-582">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="39d3e-582">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="39d3e-583">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="39d3e-583">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="39d3e-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-584">Boolean</span></span>|<span data-ttu-id="39d3e-585">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="39d3e-585">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="39d3e-586">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="39d3e-586">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="39d3e-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-587">Boolean</span></span>|<span data-ttu-id="39d3e-588">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="39d3e-588">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="39d3e-589">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="39d3e-589">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="39d3e-590">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="39d3e-590">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="39d3e-591">Especifique como a lista de certificados revogados deve ser imposta.</span><span class="sxs-lookup"><span data-stu-id="39d3e-591">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="39d3e-592">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-592">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="39d3e-593">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="39d3e-593">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="39d3e-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-594">Boolean</span></span>|<span data-ttu-id="39d3e-595">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="39d3e-595">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="39d3e-596">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="39d3e-596">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="39d3e-597">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="39d3e-597">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="39d3e-598">Configura como o enfileiramento de pacotes deve ser aplicado no cenário de gateway de túnel.</span><span class="sxs-lookup"><span data-stu-id="39d3e-598">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="39d3e-599">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-599">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="39d3e-600">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="39d3e-600">firewallProfileDomain</span></span>|[<span data-ttu-id="39d3e-601">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="39d3e-601">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="39d3e-602">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="39d3e-602">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="39d3e-603">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="39d3e-603">firewallProfilePublic</span></span>|[<span data-ttu-id="39d3e-604">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="39d3e-604">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="39d3e-605">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="39d3e-605">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="39d3e-606">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="39d3e-606">firewallProfilePrivate</span></span>|[<span data-ttu-id="39d3e-607">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="39d3e-607">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="39d3e-608">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="39d3e-608">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="39d3e-609">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="39d3e-609">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="39d3e-610">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-610">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-611">Valor que indica o comportamento do Adobe Reader da criação de processos filho.</span><span class="sxs-lookup"><span data-stu-id="39d3e-611">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="39d3e-612">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-612">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-613">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="39d3e-613">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="39d3e-614">String collection</span><span class="sxs-lookup"><span data-stu-id="39d3e-614">String collection</span></span>|<span data-ttu-id="39d3e-615">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="39d3e-615">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="39d3e-616">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-616">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="39d3e-617">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="39d3e-617">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="39d3e-618">Valor que indica o comportamento de aplicativos do Office injetando em outros processos.</span><span class="sxs-lookup"><span data-stu-id="39d3e-618">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="39d3e-619">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-619">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-620">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="39d3e-620">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="39d3e-621">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-621">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-622">Valor que indica o comportamento de aplicativos do Office injetando em outros processos.</span><span class="sxs-lookup"><span data-stu-id="39d3e-622">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="39d3e-623">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-623">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-624">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="39d3e-624">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="39d3e-625">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-626">Valor que indica o comportamento dos aplicativos de comunicação do Office, incluindo o Microsoft Outlook, da criação de processos filho.</span><span class="sxs-lookup"><span data-stu-id="39d3e-626">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="39d3e-627">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-627">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-628">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="39d3e-628">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="39d3e-629">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="39d3e-629">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="39d3e-630">Valor que indica o comportamento de aplicativos/macros do Office que criam ou iniciam conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="39d3e-630">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="39d3e-631">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-631">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-632">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="39d3e-632">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="39d3e-633">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-633">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-634">Valor que indica o comportamento de aplicativos/macros do Office que criam ou iniciam conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="39d3e-634">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="39d3e-635">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-635">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-636">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="39d3e-636">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="39d3e-637">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="39d3e-637">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="39d3e-638">Valor que indica o comportamento do aplicativo do Office que inicia processos filho.</span><span class="sxs-lookup"><span data-stu-id="39d3e-638">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="39d3e-639">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-639">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-640">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="39d3e-640">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="39d3e-641">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-641">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-642">Valor que indica o comportamento do aplicativo do Office que inicia processos filho.</span><span class="sxs-lookup"><span data-stu-id="39d3e-642">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="39d3e-643">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-643">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-644">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="39d3e-644">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="39d3e-645">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="39d3e-645">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="39d3e-646">Valor que indica o comportamento das importações Win32 do código macro no Office.</span><span class="sxs-lookup"><span data-stu-id="39d3e-646">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="39d3e-647">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-647">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-648">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="39d3e-648">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="39d3e-649">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-649">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-650">Valor que indica o comportamento das importações Win32 do código macro no Office.</span><span class="sxs-lookup"><span data-stu-id="39d3e-650">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="39d3e-651">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-651">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-652">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="39d3e-652">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="39d3e-653">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="39d3e-653">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="39d3e-654">Valor que indica o comportamento do código js/vbs/ps/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-654">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="39d3e-655">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-655">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-656">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="39d3e-656">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="39d3e-657">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-657">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-658">Valor que indica o comportamento do código js/vbs/ps/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-658">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="39d3e-659">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-659">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-660">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-660">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="39d3e-661">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="39d3e-661">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="39d3e-662">Valor que indica o comportamento de js/vbs executando carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="39d3e-662">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="39d3e-663">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-663">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-664">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="39d3e-664">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="39d3e-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-666">Valor que indica o comportamento de js/vbs executando carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="39d3e-666">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="39d3e-667">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-667">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-668">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="39d3e-668">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="39d3e-669">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-669">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-670">Valor que indica se o roubo de credenciais do subsistema da autoridade de segurança local do Windows é permitido.</span><span class="sxs-lookup"><span data-stu-id="39d3e-670">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="39d3e-671">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-671">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-672">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="39d3e-672">defenderProcessCreationType</span></span>|[<span data-ttu-id="39d3e-673">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="39d3e-673">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="39d3e-674">Valor que indica a resposta às criações de processo provenientes dos comandos PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="39d3e-674">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="39d3e-675">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-675">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-676">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="39d3e-676">defenderProcessCreation</span></span>|[<span data-ttu-id="39d3e-677">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-677">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-678">Valor que indica a resposta às criações de processo provenientes dos comandos PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="39d3e-678">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="39d3e-679">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-679">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-680">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="39d3e-680">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="39d3e-681">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="39d3e-681">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="39d3e-682">Valor que indica a resposta a processos não assinados e não assinados que são executados a partir do USB.</span><span class="sxs-lookup"><span data-stu-id="39d3e-682">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="39d3e-683">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-683">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-684">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="39d3e-684">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="39d3e-685">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-685">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-686">Valor que indica a resposta a processos não assinados e não assinados que são executados a partir do USB.</span><span class="sxs-lookup"><span data-stu-id="39d3e-686">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="39d3e-687">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-687">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-688">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="39d3e-688">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="39d3e-689">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="39d3e-689">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="39d3e-690">Valor que indica a resposta a executáveis que não atendem a uma prevalência, idade ou critérios de lista confiáveis.</span><span class="sxs-lookup"><span data-stu-id="39d3e-690">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="39d3e-691">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-691">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-692">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="39d3e-692">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="39d3e-693">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-693">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-694">Valor que indica a resposta a executáveis que não atendem a uma prevalência, idade ou critérios de lista confiáveis.</span><span class="sxs-lookup"><span data-stu-id="39d3e-694">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="39d3e-695">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-695">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-696">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-696">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="39d3e-697">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="39d3e-697">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="39d3e-698">Valor que indica se a execução de conteúdo executável (exe, dll, ps, js, vbs, etc.) deve ser retirada do email (webmail/mail-client).</span><span class="sxs-lookup"><span data-stu-id="39d3e-698">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="39d3e-699">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-699">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-700">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="39d3e-700">defenderEmailContentExecution</span></span>|[<span data-ttu-id="39d3e-701">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-701">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-702">Valor que indica se a execução de conteúdo executável (exe, dll, ps, js, vbs, etc.) deve ser retirada do email (webmail/mail-client).</span><span class="sxs-lookup"><span data-stu-id="39d3e-702">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="39d3e-703">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-703">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-704">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-704">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="39d3e-705">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-705">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-706">Valor que indica o uso da proteção avançada contra ransomeware.</span><span class="sxs-lookup"><span data-stu-id="39d3e-706">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="39d3e-707">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-707">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-708">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="39d3e-708">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="39d3e-709">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-709">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="39d3e-710">Valor que indica o comportamento de pastas protegidas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-710">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="39d3e-711">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-711">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="39d3e-712">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="39d3e-712">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="39d3e-713">String collection</span><span class="sxs-lookup"><span data-stu-id="39d3e-713">String collection</span></span>|<span data-ttu-id="39d3e-714">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="39d3e-714">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="39d3e-715">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="39d3e-715">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="39d3e-716">String collection</span><span class="sxs-lookup"><span data-stu-id="39d3e-716">String collection</span></span>|<span data-ttu-id="39d3e-717">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="39d3e-717">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="39d3e-718">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-718">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="39d3e-719">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-719">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-720">Valor que indica o comportamento de NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="39d3e-720">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="39d3e-721">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-721">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-722">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="39d3e-722">defenderExploitProtectionXml</span></span>|<span data-ttu-id="39d3e-723">Binária</span><span class="sxs-lookup"><span data-stu-id="39d3e-723">Binary</span></span>|<span data-ttu-id="39d3e-724">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="39d3e-724">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="39d3e-725">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="39d3e-725">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="39d3e-726">String</span><span class="sxs-lookup"><span data-stu-id="39d3e-726">String</span></span>|<span data-ttu-id="39d3e-727">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="39d3e-727">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="39d3e-728">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="39d3e-728">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="39d3e-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-729">Boolean</span></span>|<span data-ttu-id="39d3e-730">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="39d3e-730">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="39d3e-731">defenderBlockPersistenceThroughWmiType</span><span class="sxs-lookup"><span data-stu-id="39d3e-731">defenderBlockPersistenceThroughWmiType</span></span>|[<span data-ttu-id="39d3e-732">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="39d3e-732">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="39d3e-733">Valor que indica o comportamento da persistência block por meio da assinatura de evento WMI.</span><span class="sxs-lookup"><span data-stu-id="39d3e-733">Value indicating the behavior of Block persistence through WMI event subscription.</span></span> <span data-ttu-id="39d3e-734">Os valores possíveis são: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-734">Possible values are: `userDefined`, `block`, `auditMode`, `warn`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-735">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="39d3e-735">appLockerApplicationControl</span></span>|[<span data-ttu-id="39d3e-736">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="39d3e-736">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="39d3e-737">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="39d3e-737">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="39d3e-738">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-738">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="39d3e-739">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="39d3e-739">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="39d3e-740">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="39d3e-740">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="39d3e-741">Ative o Credential Guard quando o nível de segurança da plataforma com inicialização segura e segurança baseada em virtualização estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-741">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="39d3e-742">Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-742">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`, `disable`.</span></span>|
|<span data-ttu-id="39d3e-743">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="39d3e-743">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="39d3e-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-744">Boolean</span></span>|<span data-ttu-id="39d3e-745">Liga a segurança baseada em virtualização (VBS).</span><span class="sxs-lookup"><span data-stu-id="39d3e-745">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="39d3e-746">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="39d3e-746">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="39d3e-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-747">Boolean</span></span>|<span data-ttu-id="39d3e-748">Essa propriedade será preterida em maio de 2019 e será substituída pela propriedade DeviceGuardSecureBootWithDMA.</span><span class="sxs-lookup"><span data-stu-id="39d3e-748">This property will be deprecated in May 2019 and will be replaced with property DeviceGuardSecureBootWithDMA.</span></span> <span data-ttu-id="39d3e-749">Especifica se o Nível de Segurança da Plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="39d3e-749">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="39d3e-750">deviceGuardSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="39d3e-750">deviceGuardSecureBootWithDMA</span></span>|[<span data-ttu-id="39d3e-751">secureBootWithDMAType</span><span class="sxs-lookup"><span data-stu-id="39d3e-751">secureBootWithDMAType</span></span>](../resources/intune-deviceconfig-securebootwithdmatype.md)|<span data-ttu-id="39d3e-752">Especifica se o Nível de Segurança da Plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="39d3e-752">Specifies whether Platform Security Level is enabled at next reboot.</span></span> <span data-ttu-id="39d3e-753">Os valores possíveis são: `notConfigured`, `withoutDMA`, `withDMA`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-753">Possible values are: `notConfigured`, `withoutDMA`, `withDMA`.</span></span>|
|<span data-ttu-id="39d3e-754">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="39d3e-754">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="39d3e-755">enablement</span><span class="sxs-lookup"><span data-stu-id="39d3e-755">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="39d3e-756">Permite que o administrador de IT configure o lançamento do System Guard.</span><span class="sxs-lookup"><span data-stu-id="39d3e-756">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="39d3e-757">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-757">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="39d3e-758">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="39d3e-758">smartScreenEnableInShell</span></span>|<span data-ttu-id="39d3e-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-759">Boolean</span></span>|<span data-ttu-id="39d3e-760">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="39d3e-760">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="39d3e-761">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="39d3e-761">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="39d3e-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-762">Boolean</span></span>|<span data-ttu-id="39d3e-763">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="39d3e-763">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="39d3e-764">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="39d3e-764">applicationGuardEnabled</span></span>|<span data-ttu-id="39d3e-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-765">Boolean</span></span>|<span data-ttu-id="39d3e-766">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="39d3e-766">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="39d3e-767">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="39d3e-767">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="39d3e-768">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="39d3e-768">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="39d3e-769">Habilita o Windows Defender Application Guard para versões mais novas do Windows.</span><span class="sxs-lookup"><span data-stu-id="39d3e-769">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="39d3e-770">Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-770">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="39d3e-771">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="39d3e-771">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="39d3e-772">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="39d3e-772">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="39d3e-773">Bloqueie a área de transferência para transferir arquivo de imagem, arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="39d3e-773">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="39d3e-774">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-774">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="39d3e-775">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="39d3e-775">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="39d3e-776">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-776">Boolean</span></span>|<span data-ttu-id="39d3e-777">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="39d3e-777">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="39d3e-778">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="39d3e-778">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="39d3e-779">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-779">Boolean</span></span>|<span data-ttu-id="39d3e-780">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="39d3e-780">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="39d3e-781">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="39d3e-781">applicationGuardForceAuditing</span></span>|<span data-ttu-id="39d3e-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-782">Boolean</span></span>|<span data-ttu-id="39d3e-783">A auditoria forçada persistirá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)</span><span class="sxs-lookup"><span data-stu-id="39d3e-783">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="39d3e-784">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="39d3e-784">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="39d3e-785">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="39d3e-785">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="39d3e-786">Impedir a área de transferência de compartilhar dados do host para o contêiner, do contêiner para o host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="39d3e-786">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="39d3e-787">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-787">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="39d3e-788">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="39d3e-788">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="39d3e-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-789">Boolean</span></span>|<span data-ttu-id="39d3e-790">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="39d3e-790">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="39d3e-791">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="39d3e-791">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="39d3e-792">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-792">Boolean</span></span>|<span data-ttu-id="39d3e-793">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="39d3e-793">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="39d3e-794">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="39d3e-794">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="39d3e-795">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-795">Boolean</span></span>|<span data-ttu-id="39d3e-796">Permitir a impressão em impressoras locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="39d3e-796">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="39d3e-797">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="39d3e-797">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="39d3e-798">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-798">Boolean</span></span>|<span data-ttu-id="39d3e-799">Permitir a impressão em impressoras da rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="39d3e-799">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="39d3e-800">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="39d3e-800">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="39d3e-801">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-801">Boolean</span></span>|<span data-ttu-id="39d3e-802">Permitir que o Application Guard use GPU virtual</span><span class="sxs-lookup"><span data-stu-id="39d3e-802">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="39d3e-803">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="39d3e-803">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="39d3e-804">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-804">Boolean</span></span>|<span data-ttu-id="39d3e-805">Permitir que os usuários baixem arquivos do Edge no contêiner do Application Guard e salve-os no sistema de arquivos host</span><span class="sxs-lookup"><span data-stu-id="39d3e-805">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="39d3e-806">applicationGuardAllowCameraMicrophoneRedirection</span><span class="sxs-lookup"><span data-stu-id="39d3e-806">applicationGuardAllowCameraMicrophoneRedirection</span></span>|<span data-ttu-id="39d3e-807">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-807">Boolean</span></span>|<span data-ttu-id="39d3e-808">Obtém ou define se os aplicativos dentro do Microsoft Defender Application Guard podem acessar a câmera e o microfone do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-808">Gets or sets whether applications inside Microsoft Defender Application Guard can access the device’s camera and microphone.</span></span>|
|<span data-ttu-id="39d3e-809">applicationGuardCertificateThumbprints</span><span class="sxs-lookup"><span data-stu-id="39d3e-809">applicationGuardCertificateThumbprints</span></span>|<span data-ttu-id="39d3e-810">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="39d3e-810">String collection</span></span>|<span data-ttu-id="39d3e-811">Permite que determinados certificados raiz de nível de dispositivo sejam compartilhados com o contêiner do Microsoft Defender Application Guard.</span><span class="sxs-lookup"><span data-stu-id="39d3e-811">Allows certain device level Root Certificates to be shared with the Microsoft Defender Application Guard container.</span></span>|
|<span data-ttu-id="39d3e-812">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="39d3e-812">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="39d3e-813">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-813">Boolean</span></span>|<span data-ttu-id="39d3e-814">Permite que o administrador permita que os usuários padrão habilitam a encrpytion durante o Azure AD Join.</span><span class="sxs-lookup"><span data-stu-id="39d3e-814">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="39d3e-815">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="39d3e-815">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="39d3e-816">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-816">Boolean</span></span>|<span data-ttu-id="39d3e-817">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="39d3e-817">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="39d3e-818">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="39d3e-818">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="39d3e-819">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-819">Boolean</span></span>|<span data-ttu-id="39d3e-820">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="39d3e-820">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="39d3e-821">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="39d3e-821">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="39d3e-822">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="39d3e-822">bitLockerEncryptDevice</span></span>|<span data-ttu-id="39d3e-823">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-823">Boolean</span></span>|<span data-ttu-id="39d3e-824">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="39d3e-824">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="39d3e-825">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="39d3e-825">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="39d3e-826">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="39d3e-826">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="39d3e-827">Política de unidade do sistema BitLocker.</span><span class="sxs-lookup"><span data-stu-id="39d3e-827">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="39d3e-828">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="39d3e-828">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="39d3e-829">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="39d3e-829">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="39d3e-830">Política de Unidade Fixa do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="39d3e-830">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="39d3e-831">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="39d3e-831">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="39d3e-832">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="39d3e-832">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="39d3e-833">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="39d3e-833">BitLocker Removable Drive Policy.</span></span>|
|<span data-ttu-id="39d3e-834">bitLockerRecoveryPasswordRotation</span><span class="sxs-lookup"><span data-stu-id="39d3e-834">bitLockerRecoveryPasswordRotation</span></span>|[<span data-ttu-id="39d3e-835">bitLockerRecoveryPasswordRotationType</span><span class="sxs-lookup"><span data-stu-id="39d3e-835">bitLockerRecoveryPasswordRotationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|<span data-ttu-id="39d3e-836">Essa configuração inicia uma rotação de senha de recuperação orientada pelo cliente após uma recuperação de unidade do sistema operacional (usando bootmgr ou WinRE).</span><span class="sxs-lookup"><span data-stu-id="39d3e-836">This setting initiates a client-driven recovery password rotation after an OS drive recovery (either by using bootmgr or WinRE).</span></span> <span data-ttu-id="39d3e-837">Os valores possíveis são: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-837">Possible values are: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.</span></span>|
|<span data-ttu-id="39d3e-838">defenderDisableScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="39d3e-838">defenderDisableScanArchiveFiles</span></span>|<span data-ttu-id="39d3e-839">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-839">Boolean</span></span>|<span data-ttu-id="39d3e-840">Permite ou não a verificação de arquivos.</span><span class="sxs-lookup"><span data-stu-id="39d3e-840">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="39d3e-841">defenderAllowScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="39d3e-841">defenderAllowScanArchiveFiles</span></span>|<span data-ttu-id="39d3e-842">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-842">Boolean</span></span>|<span data-ttu-id="39d3e-843">Permite ou não a verificação de arquivos.</span><span class="sxs-lookup"><span data-stu-id="39d3e-843">Allows or disallows scanning of archives.</span></span>|
|<span data-ttu-id="39d3e-844">defenderDisableBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="39d3e-844">defenderDisableBehaviorMonitoring</span></span>|<span data-ttu-id="39d3e-845">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-845">Boolean</span></span>|<span data-ttu-id="39d3e-846">Permite ou não a funcionalidade de Monitoramento de Comportamento do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="39d3e-846">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="39d3e-847">defenderAllowBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="39d3e-847">defenderAllowBehaviorMonitoring</span></span>|<span data-ttu-id="39d3e-848">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-848">Boolean</span></span>|<span data-ttu-id="39d3e-849">Permite ou não a funcionalidade de Monitoramento de Comportamento do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="39d3e-849">Allows or disallows Windows Defender Behavior Monitoring functionality.</span></span>|
|<span data-ttu-id="39d3e-850">defenderDisableCloudProtection</span><span class="sxs-lookup"><span data-stu-id="39d3e-850">defenderDisableCloudProtection</span></span>|<span data-ttu-id="39d3e-851">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-851">Boolean</span></span>|<span data-ttu-id="39d3e-852">Para proteger melhor seu computador, o Windows Defender enviará informações à Microsoft sobre quaisquer problemas encontrados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-852">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="39d3e-853">A Microsoft analisará essas informações, aprenderá mais sobre problemas que afetam você e outros clientes e oferecerá soluções aprimoradas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-853">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="39d3e-854">defenderAllowCloudProtection</span><span class="sxs-lookup"><span data-stu-id="39d3e-854">defenderAllowCloudProtection</span></span>|<span data-ttu-id="39d3e-855">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-855">Boolean</span></span>|<span data-ttu-id="39d3e-856">Para proteger melhor seu computador, o Windows Defender enviará informações à Microsoft sobre quaisquer problemas encontrados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-856">To best protect your PC, Windows Defender will send information to Microsoft about any problems it finds.</span></span> <span data-ttu-id="39d3e-857">A Microsoft analisará essas informações, aprenderá mais sobre problemas que afetam você e outros clientes e oferecerá soluções aprimoradas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-857">Microsoft will analyze that information, learn more about problems affecting you and other customers, and offer improved solutions.</span></span>|
|<span data-ttu-id="39d3e-858">defenderEnableScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="39d3e-858">defenderEnableScanIncomingMail</span></span>|<span data-ttu-id="39d3e-859">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-859">Boolean</span></span>|<span data-ttu-id="39d3e-860">Permite ou não a verificação de emails.</span><span class="sxs-lookup"><span data-stu-id="39d3e-860">Allows or disallows scanning of email.</span></span>|
|<span data-ttu-id="39d3e-861">defenderEnableScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="39d3e-861">defenderEnableScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="39d3e-862">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-862">Boolean</span></span>|<span data-ttu-id="39d3e-863">Permite ou não uma verificação completa das unidades de rede mapeadas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-863">Allows or disallows a full scan of mapped network drives.</span></span>|
|<span data-ttu-id="39d3e-864">defenderDisableScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="39d3e-864">defenderDisableScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="39d3e-865">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-865">Boolean</span></span>|<span data-ttu-id="39d3e-866">Permite ou não uma verificação completa de unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="39d3e-866">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="39d3e-867">Durante uma verificação rápida, as unidades removíveis ainda podem ser examinadas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-867">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="39d3e-868">defenderAllowScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="39d3e-868">defenderAllowScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="39d3e-869">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-869">Boolean</span></span>|<span data-ttu-id="39d3e-870">Permite ou não uma verificação completa de unidades removíveis.</span><span class="sxs-lookup"><span data-stu-id="39d3e-870">Allows or disallows a full scan of removable drives.</span></span> <span data-ttu-id="39d3e-871">Durante uma verificação rápida, as unidades removíveis ainda podem ser examinadas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-871">During a quick scan, removable drives may still be scanned.</span></span>|
|<span data-ttu-id="39d3e-872">defenderDisableScanDownloads</span><span class="sxs-lookup"><span data-stu-id="39d3e-872">defenderDisableScanDownloads</span></span>|<span data-ttu-id="39d3e-873">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-873">Boolean</span></span>|<span data-ttu-id="39d3e-874">Permite ou não a funcionalidade de Proteção IOAVP do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="39d3e-874">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="39d3e-875">defenderAllowScanDownloads</span><span class="sxs-lookup"><span data-stu-id="39d3e-875">defenderAllowScanDownloads</span></span>|<span data-ttu-id="39d3e-876">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-876">Boolean</span></span>|<span data-ttu-id="39d3e-877">Permite ou não a funcionalidade de Proteção IOAVP do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="39d3e-877">Allows or disallows Windows Defender IOAVP Protection functionality.</span></span>|
|<span data-ttu-id="39d3e-878">defenderDisableIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="39d3e-878">defenderDisableIntrusionPreventionSystem</span></span>|<span data-ttu-id="39d3e-879">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-879">Boolean</span></span>|<span data-ttu-id="39d3e-880">Permite ou não a funcionalidade de Prevenção contra Intrusões do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="39d3e-880">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="39d3e-881">defenderAllowIntrusionPreventionSystem</span><span class="sxs-lookup"><span data-stu-id="39d3e-881">defenderAllowIntrusionPreventionSystem</span></span>|<span data-ttu-id="39d3e-882">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-882">Boolean</span></span>|<span data-ttu-id="39d3e-883">Permite ou não a funcionalidade de Prevenção contra Intrusões do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="39d3e-883">Allows or disallows Windows Defender Intrusion Prevention functionality.</span></span>|
|<span data-ttu-id="39d3e-884">defenderDisableOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="39d3e-884">defenderDisableOnAccessProtection</span></span>|<span data-ttu-id="39d3e-885">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-885">Boolean</span></span>|<span data-ttu-id="39d3e-886">Permite ou não a funcionalidade do Windows Defender On Access Protection.</span><span class="sxs-lookup"><span data-stu-id="39d3e-886">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="39d3e-887">defenderAllowOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="39d3e-887">defenderAllowOnAccessProtection</span></span>|<span data-ttu-id="39d3e-888">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-888">Boolean</span></span>|<span data-ttu-id="39d3e-889">Permite ou não a funcionalidade do Windows Defender On Access Protection.</span><span class="sxs-lookup"><span data-stu-id="39d3e-889">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="39d3e-890">defenderDisableRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="39d3e-890">defenderDisableRealTimeMonitoring</span></span>|<span data-ttu-id="39d3e-891">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-891">Boolean</span></span>|<span data-ttu-id="39d3e-892">Permite ou não a funcionalidade de Monitoramento em Tempo Real do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="39d3e-892">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="39d3e-893">defenderAllowRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="39d3e-893">defenderAllowRealTimeMonitoring</span></span>|<span data-ttu-id="39d3e-894">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-894">Boolean</span></span>|<span data-ttu-id="39d3e-895">Permite ou não a funcionalidade de Monitoramento em Tempo Real do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="39d3e-895">Allows or disallows Windows Defender Realtime Monitoring functionality.</span></span>|
|<span data-ttu-id="39d3e-896">defenderDisableScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="39d3e-896">defenderDisableScanNetworkFiles</span></span>|<span data-ttu-id="39d3e-897">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-897">Boolean</span></span>|<span data-ttu-id="39d3e-898">Permite ou não uma verificação de arquivos de rede.</span><span class="sxs-lookup"><span data-stu-id="39d3e-898">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="39d3e-899">defenderAllowScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="39d3e-899">defenderAllowScanNetworkFiles</span></span>|<span data-ttu-id="39d3e-900">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-900">Boolean</span></span>|<span data-ttu-id="39d3e-901">Permite ou não uma verificação de arquivos de rede.</span><span class="sxs-lookup"><span data-stu-id="39d3e-901">Allows or disallows a scanning of network files.</span></span>|
|<span data-ttu-id="39d3e-902">defenderDisableScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="39d3e-902">defenderDisableScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="39d3e-903">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-903">Boolean</span></span>|<span data-ttu-id="39d3e-904">Permite ou não a funcionalidade de Verificação de Scripts do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="39d3e-904">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="39d3e-905">defenderAllowScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="39d3e-905">defenderAllowScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="39d3e-906">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-906">Boolean</span></span>|<span data-ttu-id="39d3e-907">Permite ou não a funcionalidade de Verificação de Scripts do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="39d3e-907">Allows or disallows Windows Defender Script Scanning functionality.</span></span>|
|<span data-ttu-id="39d3e-908">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="39d3e-908">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="39d3e-909">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-909">Boolean</span></span>|<span data-ttu-id="39d3e-910">Permite ou não o acesso do usuário à interface do usuário do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="39d3e-910">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="39d3e-911">Se não for permitido, todas as notificações do Windows Defender também serão suprimidas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-911">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="39d3e-912">defenderAllowEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="39d3e-912">defenderAllowEndUserAccess</span></span>|<span data-ttu-id="39d3e-913">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-913">Boolean</span></span>|<span data-ttu-id="39d3e-914">Permite ou não o acesso do usuário à interface do usuário do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="39d3e-914">Allows or disallows user access to the Windows Defender UI.</span></span> <span data-ttu-id="39d3e-915">Se não for permitido, todas as notificações do Windows Defender também serão suprimidas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-915">If disallowed, all Windows Defender notifications will also be suppressed.</span></span>|
|<span data-ttu-id="39d3e-916">defenderScanMaxCpuPercentage</span><span class="sxs-lookup"><span data-stu-id="39d3e-916">defenderScanMaxCpuPercentage</span></span>|<span data-ttu-id="39d3e-917">Int32</span><span class="sxs-lookup"><span data-stu-id="39d3e-917">Int32</span></span>|<span data-ttu-id="39d3e-918">Representa o fator de carga média da CPU para a verificação do Windows Defender (em porcentagem).</span><span class="sxs-lookup"><span data-stu-id="39d3e-918">Represents the average CPU load factor for the Windows Defender scan (in percent).</span></span> <span data-ttu-id="39d3e-919">O valor padrão é 50.</span><span class="sxs-lookup"><span data-stu-id="39d3e-919">The default value is 50.</span></span> <span data-ttu-id="39d3e-920">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="39d3e-920">Valid values 0 to 100</span></span>|
|<span data-ttu-id="39d3e-921">defenderCheckForSignaturesBeforeRunningScan</span><span class="sxs-lookup"><span data-stu-id="39d3e-921">defenderCheckForSignaturesBeforeRunningScan</span></span>|<span data-ttu-id="39d3e-922">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-922">Boolean</span></span>|<span data-ttu-id="39d3e-923">Esta configuração de política permite que você gerencie se uma verificação de novas definições de vírus e spyware ocorrerá antes de executar uma verificação.</span><span class="sxs-lookup"><span data-stu-id="39d3e-923">This policy setting allows you to manage whether a check for new virus and spyware definitions will occur before running a scan.</span></span>|
|<span data-ttu-id="39d3e-924">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="39d3e-924">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="39d3e-925">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="39d3e-925">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="39d3e-926">Adicionado ao Windows 10, versão 1709.</span><span class="sxs-lookup"><span data-stu-id="39d3e-926">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="39d3e-927">Esta configuração de política determina o quão agressivo o Windows Defender Antivírus será ao bloquear e verificar arquivos suspeitos.</span><span class="sxs-lookup"><span data-stu-id="39d3e-927">This policy setting determines how aggressive Windows Defender Antivirus will be in blocking and scanning suspicious files.</span></span> <span data-ttu-id="39d3e-928">O tipo de valor é inteiro.</span><span class="sxs-lookup"><span data-stu-id="39d3e-928">Value type is integer.</span></span> <span data-ttu-id="39d3e-929">Esse recurso requer a configuração "Ingressar no Microsoft MAPS" habilitada para funcionar.</span><span class="sxs-lookup"><span data-stu-id="39d3e-929">This feature requires the "Join Microsoft MAPS" setting enabled in order to function.</span></span> <span data-ttu-id="39d3e-930">Os valores possíveis são: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-930">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="39d3e-931">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="39d3e-931">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="39d3e-932">Int32</span><span class="sxs-lookup"><span data-stu-id="39d3e-932">Int32</span></span>|<span data-ttu-id="39d3e-933">Adicionado ao Windows 10, versão 1709.</span><span class="sxs-lookup"><span data-stu-id="39d3e-933">Added in Windows 10, version 1709.</span></span> <span data-ttu-id="39d3e-934">Esse recurso permite que o Windows Defender Antivírus bloqueie um arquivo suspeito por até 60 segundos e o digitalizar na nuvem para garantir que ele seja seguro.</span><span class="sxs-lookup"><span data-stu-id="39d3e-934">This feature allows Windows Defender Antivirus to block a suspicious file for up to 60 seconds, and scan it in the cloud to make sure it's safe.</span></span> <span data-ttu-id="39d3e-935">O tipo de valor é inteiro, o intervalo é de 0 a 50.</span><span class="sxs-lookup"><span data-stu-id="39d3e-935">Value type is integer, range is 0 - 50.</span></span> <span data-ttu-id="39d3e-936">Esse recurso depende de três outras configurações MAPS que devem estar todas habilitadas: "Configurar o recurso "Bloquear à Primeira Vista"; " Ingressar no Microsoft MAPS"; "Enviar amostras de arquivo quando outra análise for necessária".</span><span class="sxs-lookup"><span data-stu-id="39d3e-936">This feature depends on three other MAPS settings the must all be enabled- "Configure the 'Block at First Sight' feature; "Join Microsoft MAPS"; "Send file samples when further analysis is required".</span></span> <span data-ttu-id="39d3e-937">Valores válidos de 0 a 50</span><span class="sxs-lookup"><span data-stu-id="39d3e-937">Valid values 0 to 50</span></span>|
|<span data-ttu-id="39d3e-938">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="39d3e-938">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="39d3e-939">Int32</span><span class="sxs-lookup"><span data-stu-id="39d3e-939">Int32</span></span>|<span data-ttu-id="39d3e-940">Período de tempo (em dias) em que os itens de quarentena serão armazenados no sistema.</span><span class="sxs-lookup"><span data-stu-id="39d3e-940">Time period (in days) that quarantine items will be stored on the system.</span></span> <span data-ttu-id="39d3e-941">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="39d3e-941">Valid values 0 to 90</span></span>|
|<span data-ttu-id="39d3e-942">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="39d3e-942">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="39d3e-943">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-943">Boolean</span></span>|<span data-ttu-id="39d3e-944">Esta configuração de política permite que você configure verificações de at configuração para verificações completas agendadas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-944">This policy setting allows you to configure catch-up scans for scheduled full scans.</span></span> <span data-ttu-id="39d3e-945">Uma verificação de captura é uma verificação iniciada porque uma verificação agendada regularmente foi perdida.</span><span class="sxs-lookup"><span data-stu-id="39d3e-945">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="39d3e-946">Geralmente, essas verificações agendadas são perdidas porque o computador foi desligado no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-946">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="39d3e-947">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="39d3e-947">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="39d3e-948">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-948">Boolean</span></span>|<span data-ttu-id="39d3e-949">Esta configuração de política permite que você configure verificações de recuperação para verificações rápidas agendadas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-949">This policy setting allows you to configure catch-up scans for scheduled quick scans.</span></span> <span data-ttu-id="39d3e-950">Uma verificação de captura é uma verificação iniciada porque uma verificação agendada regularmente foi perdida.</span><span class="sxs-lookup"><span data-stu-id="39d3e-950">A catch-up scan is a scan that is initiated because a regularly scheduled scan was missed.</span></span> <span data-ttu-id="39d3e-951">Geralmente, essas verificações agendadas são perdidas porque o computador foi desligado no horário agendado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-951">Usually these scheduled scans are missed because the computer was turned off at the scheduled time.</span></span>|
|<span data-ttu-id="39d3e-952">defenderEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="39d3e-952">defenderEnableLowCpuPriority</span></span>|<span data-ttu-id="39d3e-953">Boolean</span><span class="sxs-lookup"><span data-stu-id="39d3e-953">Boolean</span></span>|<span data-ttu-id="39d3e-954">Esta configuração de política permite habilitar ou desabilitar baixa prioridade de CPU para verificações agendadas.</span><span class="sxs-lookup"><span data-stu-id="39d3e-954">This policy setting allows you to enable or disable low CPU priority for scheduled scans.</span></span>|
|<span data-ttu-id="39d3e-955">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="39d3e-955">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="39d3e-956">String collection</span><span class="sxs-lookup"><span data-stu-id="39d3e-956">String collection</span></span>|<span data-ttu-id="39d3e-957">Extensões de arquivo a serem excluídas das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="39d3e-957">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="39d3e-958">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="39d3e-958">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="39d3e-959">String collection</span><span class="sxs-lookup"><span data-stu-id="39d3e-959">String collection</span></span>|<span data-ttu-id="39d3e-960">Arquivos e pastas a serem excluídos das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="39d3e-960">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="39d3e-961">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="39d3e-961">defenderProcessesToExclude</span></span>|<span data-ttu-id="39d3e-962">String collection</span><span class="sxs-lookup"><span data-stu-id="39d3e-962">String collection</span></span>|<span data-ttu-id="39d3e-963">Processos a serem excluídos das verificações e da proteção em tempo real.</span><span class="sxs-lookup"><span data-stu-id="39d3e-963">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="39d3e-964">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="39d3e-964">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="39d3e-965">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="39d3e-965">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="39d3e-966">Adicionado no Windows 10, versão 1607.</span><span class="sxs-lookup"><span data-stu-id="39d3e-966">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="39d3e-967">Especifica o nível de detecção de aplicativos potencialmente indesejados (PUAs).</span><span class="sxs-lookup"><span data-stu-id="39d3e-967">Specifies the level of detection for potentially unwanted applications (PUAs).</span></span> <span data-ttu-id="39d3e-968">O Windows Defender alerta você quando um software potencialmente indesejado está sendo baixado ou tenta se instalar no computador.</span><span class="sxs-lookup"><span data-stu-id="39d3e-968">Windows Defender alerts you when potentially unwanted software is being downloaded or attempts to install itself on your computer.</span></span> <span data-ttu-id="39d3e-969">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-969">Possible values are: `userDefined`, `enable`, `auditMode`, `warn`, `notConfigured`.</span></span>|
|<span data-ttu-id="39d3e-970">defenderScanDirection</span><span class="sxs-lookup"><span data-stu-id="39d3e-970">defenderScanDirection</span></span>|[<span data-ttu-id="39d3e-971">defenderRealtimeScanDirection</span><span class="sxs-lookup"><span data-stu-id="39d3e-971">defenderRealtimeScanDirection</span></span>](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|<span data-ttu-id="39d3e-972">Controla quais conjuntos de arquivos devem ser monitorados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-972">Controls which sets of files should be monitored.</span></span> <span data-ttu-id="39d3e-973">Os valores possíveis são: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-973">Possible values are: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="39d3e-974">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="39d3e-974">defenderScanType</span></span>|[<span data-ttu-id="39d3e-975">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="39d3e-975">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="39d3e-976">Seleciona se será feita uma verificação rápida ou uma verificação completa.</span><span class="sxs-lookup"><span data-stu-id="39d3e-976">Selects whether to perform a quick scan or full scan.</span></span> <span data-ttu-id="39d3e-977">Os valores possíveis são: `userDefined`, `disabled`, `quick`, `full`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-977">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="39d3e-978">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="39d3e-978">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="39d3e-979">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="39d3e-979">TimeOfDay</span></span>|<span data-ttu-id="39d3e-980">Seleciona a hora do dia em que a verificação rápida do Windows Defender deve ser executado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-980">Selects the time of day that the Windows Defender quick scan should run.</span></span> <span data-ttu-id="39d3e-981">Por exemplo, um valor de 0=12:00AM, um valor de 60=1:00AM, um valor de 120=2:00 e assim por diante, até um valor de 1380=11:00PM.</span><span class="sxs-lookup"><span data-stu-id="39d3e-981">For example, a value of 0=12:00AM, a value of 60=1:00AM, a value of 120=2:00, and so on, up to a value of 1380=11:00PM.</span></span> <span data-ttu-id="39d3e-982">O valor padrão é 120</span><span class="sxs-lookup"><span data-stu-id="39d3e-982">The default value is 120</span></span>|
|<span data-ttu-id="39d3e-983">defenderScheduledScanDay</span><span class="sxs-lookup"><span data-stu-id="39d3e-983">defenderScheduledScanDay</span></span>|[<span data-ttu-id="39d3e-984">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="39d3e-984">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="39d3e-985">Seleciona o dia em que a verificação do Windows Defender deve ser executado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-985">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="39d3e-986">Os valores possíveis são: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-986">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="39d3e-987">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="39d3e-987">defenderScheduledScanTime</span></span>|<span data-ttu-id="39d3e-988">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="39d3e-988">TimeOfDay</span></span>|<span data-ttu-id="39d3e-989">Seleciona a hora do dia em que a verificação do Windows Defender deve ser executado.</span><span class="sxs-lookup"><span data-stu-id="39d3e-989">Selects the time of day that the Windows Defender scan should run.</span></span>|
|<span data-ttu-id="39d3e-990">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="39d3e-990">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="39d3e-991">Int32</span><span class="sxs-lookup"><span data-stu-id="39d3e-991">Int32</span></span>|<span data-ttu-id="39d3e-992">Especifica o intervalo (em horas) que será usado para verificar se há assinaturas, portanto, em vez de usar ScheduleDay e ScheduleTime, a verificação de novas assinaturas será definida de acordo com o intervalo.</span><span class="sxs-lookup"><span data-stu-id="39d3e-992">Specifies the interval (in hours) that will be used to check for signatures, so instead of using the ScheduleDay and ScheduleTime the check for new signatures will be set according to the interval.</span></span> <span data-ttu-id="39d3e-993">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="39d3e-993">Valid values 0 to 24</span></span>|
|<span data-ttu-id="39d3e-994">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="39d3e-994">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="39d3e-995">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="39d3e-995">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="39d3e-996">Verifica o nível de consentimento do usuário no Windows Defender para enviar dados.</span><span class="sxs-lookup"><span data-stu-id="39d3e-996">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="39d3e-997">Os valores possíveis são: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span><span class="sxs-lookup"><span data-stu-id="39d3e-997">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="39d3e-998">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="39d3e-998">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="39d3e-999">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="39d3e-999">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="39d3e-1000">Permite que um administrador especifique qualquer nível de severidade de ameaça válido e a ID de ação padrão correspondente a ser tomada.</span><span class="sxs-lookup"><span data-stu-id="39d3e-1000">Allows an administrator to specify any valid threat severity levels and the corresponding default action ID to take.</span></span>|



## <a name="response"></a><span data-ttu-id="39d3e-1001">Resposta</span><span class="sxs-lookup"><span data-stu-id="39d3e-1001">Response</span></span>
<span data-ttu-id="39d3e-1002">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39d3e-1002">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39d3e-1003">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39d3e-1003">Example</span></span>

### <a name="request"></a><span data-ttu-id="39d3e-1004">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39d3e-1004">Request</span></span>
<span data-ttu-id="39d3e-1005">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39d3e-1005">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="39d3e-1006">Resposta</span><span class="sxs-lookup"><span data-stu-id="39d3e-1006">Response</span></span>
<span data-ttu-id="39d3e-p226">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39d3e-p226">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




