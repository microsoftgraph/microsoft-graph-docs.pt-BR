---
title: Atualizar windows10EndpointProtectionConfiguration
description: Atualizar as propriedades de um objeto windows10EndpointProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f2680e25560d8211067a37f160d1341fd94b28a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155087"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="f3caf-103">Atualizar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="f3caf-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="f3caf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3caf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3caf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3caf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3caf-106">Atualizar as propriedades de um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3caf-106">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3caf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3caf-107">Prerequisites</span></span>
<span data-ttu-id="f3caf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f3caf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f3caf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3caf-110">Permission type</span></span>|<span data-ttu-id="f3caf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f3caf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3caf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3caf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3caf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3caf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3caf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3caf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3caf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3caf-115">Not supported.</span></span>|
|<span data-ttu-id="f3caf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3caf-116">Application</span></span>|<span data-ttu-id="f3caf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3caf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3caf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3caf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f3caf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3caf-119">Request headers</span></span>
|<span data-ttu-id="f3caf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3caf-120">Header</span></span>|<span data-ttu-id="f3caf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f3caf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3caf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3caf-122">Authorization</span></span>|<span data-ttu-id="f3caf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3caf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3caf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f3caf-124">Accept</span></span>|<span data-ttu-id="f3caf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3caf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3caf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3caf-126">Request body</span></span>
<span data-ttu-id="f3caf-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3caf-127">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="f3caf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3caf-128">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="f3caf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3caf-129">Property</span></span>|<span data-ttu-id="f3caf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3caf-130">Type</span></span>|<span data-ttu-id="f3caf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3caf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3caf-132">id</span><span class="sxs-lookup"><span data-stu-id="f3caf-132">id</span></span>|<span data-ttu-id="f3caf-133">String</span><span class="sxs-lookup"><span data-stu-id="f3caf-133">String</span></span>|<span data-ttu-id="f3caf-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f3caf-134">Key of the entity.</span></span> <span data-ttu-id="f3caf-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3caf-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3caf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3caf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f3caf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3caf-137">DateTimeOffset</span></span>|<span data-ttu-id="f3caf-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f3caf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f3caf-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3caf-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3caf-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f3caf-140">roleScopeTagIds</span></span>|<span data-ttu-id="f3caf-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3caf-141">String collection</span></span>|<span data-ttu-id="f3caf-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f3caf-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f3caf-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3caf-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3caf-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f3caf-144">supportsScopeTags</span></span>|<span data-ttu-id="f3caf-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-145">Boolean</span></span>|<span data-ttu-id="f3caf-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f3caf-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f3caf-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f3caf-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f3caf-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f3caf-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f3caf-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3caf-149">This property is read-only.</span></span> <span data-ttu-id="f3caf-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3caf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3caf-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3caf-151">createdDateTime</span></span>|<span data-ttu-id="f3caf-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3caf-152">DateTimeOffset</span></span>|<span data-ttu-id="f3caf-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f3caf-153">DateTime the object was created.</span></span> <span data-ttu-id="f3caf-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3caf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3caf-155">description</span><span class="sxs-lookup"><span data-stu-id="f3caf-155">description</span></span>|<span data-ttu-id="f3caf-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3caf-156">String</span></span>|<span data-ttu-id="f3caf-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3caf-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f3caf-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3caf-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3caf-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f3caf-159">displayName</span></span>|<span data-ttu-id="f3caf-160">String</span><span class="sxs-lookup"><span data-stu-id="f3caf-160">String</span></span>|<span data-ttu-id="f3caf-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3caf-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f3caf-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3caf-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3caf-163">version</span><span class="sxs-lookup"><span data-stu-id="f3caf-163">version</span></span>|<span data-ttu-id="f3caf-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f3caf-164">Int32</span></span>|<span data-ttu-id="f3caf-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3caf-165">Version of the device configuration.</span></span> <span data-ttu-id="f3caf-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3caf-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3caf-167">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="f3caf-167">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="f3caf-168">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="f3caf-168">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="f3caf-169">Essa política destina-se a fornecer segurança adicional contra dispositivos compatíveis com DMA externo.</span><span class="sxs-lookup"><span data-stu-id="f3caf-169">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="f3caf-170">Permite mais controle sobre a enumeração de dispositivos compatíveis com DMA externo incompatíveis com o remapeamento de DMA/isolamento de memória do dispositivo e área restrita.</span><span class="sxs-lookup"><span data-stu-id="f3caf-170">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="f3caf-171">Essa política só entra em vigor quando a proteção DMA de kernel é suportada e habilitada pelo firmware do sistema.</span><span class="sxs-lookup"><span data-stu-id="f3caf-171">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="f3caf-172">A proteção DMA de kernel é um recurso de plataforma que não pode ser controlado via política ou pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="f3caf-172">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="f3caf-173">É preciso ter suporte do sistema no momento da fabricação.</span><span class="sxs-lookup"><span data-stu-id="f3caf-173">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="f3caf-174">Para verificar se o sistema suporta a proteção DMA de kernel, verifique o campo proteção DMA de kernel na página Resumo de MSINFO32. exe.</span><span class="sxs-lookup"><span data-stu-id="f3caf-174">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="f3caf-175">Os valores possíveis são: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-175">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="f3caf-176">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="f3caf-176">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="f3caf-177">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-177">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-178">Esse direito de usuário é usado pelo Gerenciador de credenciais durante o backup/restauração.</span><span class="sxs-lookup"><span data-stu-id="f3caf-178">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="f3caf-179">As credenciais salvas dos usuários podem ser comprometidas se esse privilégio for dado a outras entidades.</span><span class="sxs-lookup"><span data-stu-id="f3caf-179">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="f3caf-180">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="f3caf-180">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3caf-181">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="f3caf-181">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="f3caf-182">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-182">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-183">Esse direito de usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="f3caf-183">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="f3caf-184">O estado permitido é suportado.</span><span class="sxs-lookup"><span data-stu-id="f3caf-184">State Allowed is supported.</span></span>|
|<span data-ttu-id="f3caf-185">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="f3caf-185">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="f3caf-186">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-186">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-187">Esse direito de usuário determina quais usuários e grupos são bloqueados para se conectarem ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="f3caf-187">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="f3caf-188">Há suporte para o bloco de estado.</span><span class="sxs-lookup"><span data-stu-id="f3caf-188">State Block is supported.</span></span>|
|<span data-ttu-id="f3caf-189">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f3caf-189">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="f3caf-190">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-190">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-191">Esse direito de usuário permite que um processo represente qualquer usuário sem autenticação.</span><span class="sxs-lookup"><span data-stu-id="f3caf-191">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="f3caf-192">Portanto, o processo pode ter acesso aos mesmos recursos locais que esse usuário.</span><span class="sxs-lookup"><span data-stu-id="f3caf-192">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="f3caf-193">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="f3caf-193">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3caf-194">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="f3caf-194">userRightsLocalLogOn</span></span>|[<span data-ttu-id="f3caf-195">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-195">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-196">Esse direito de usuário determina quais usuários podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="f3caf-196">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="f3caf-197">Estados não conFigurados, permitidos e bloqueados são todos suportados</span><span class="sxs-lookup"><span data-stu-id="f3caf-197">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="f3caf-198">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="f3caf-198">userRightsBackupData</span></span>|[<span data-ttu-id="f3caf-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-200">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao fazer backup de arquivos e diretórios.</span><span class="sxs-lookup"><span data-stu-id="f3caf-200">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="f3caf-201">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="f3caf-201">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3caf-202">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="f3caf-202">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="f3caf-203">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-203">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-204">Este direito de usuário determina quais usuários e grupos podem alterar a hora e a data no relógio interno do computador.</span><span class="sxs-lookup"><span data-stu-id="f3caf-204">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="f3caf-205">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="f3caf-205">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3caf-206">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="f3caf-206">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="f3caf-207">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-207">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-208">Configuração de segurança que determina se os usuários podem criar objetos globais que estão disponíveis para todas as sessões.</span><span class="sxs-lookup"><span data-stu-id="f3caf-208">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="f3caf-209">Os usuários que podem criar objetos globais podem afetar processos executados em sessões de outros usuários, o que pode levar a falhas de aplicativos ou corrupção de dados.</span><span class="sxs-lookup"><span data-stu-id="f3caf-209">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="f3caf-210">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="f3caf-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3caf-211">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="f3caf-211">userRightsCreatePageFile</span></span>|[<span data-ttu-id="f3caf-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-213">Esse direito de usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de paginação.</span><span class="sxs-lookup"><span data-stu-id="f3caf-213">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="f3caf-214">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="f3caf-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3caf-215">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="f3caf-215">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="f3caf-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-217">Este direito de usuário determina quais contas podem ser usadas por processos para criar um objeto de diretório usando o Gerenciador de objetos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-217">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="f3caf-218">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="f3caf-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3caf-219">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="f3caf-219">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="f3caf-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-221">Esse direito de usuário determina se o usuário pode criar um link simbólico do computador no qual está conectado.</span><span class="sxs-lookup"><span data-stu-id="f3caf-221">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="f3caf-222">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="f3caf-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3caf-223">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="f3caf-223">userRightsCreateToken</span></span>|[<span data-ttu-id="f3caf-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-225">Esse direito de usuário determina quais usuários/grupos podem ser usados por processos para criar um token que pode ser usado para obter acesso a qualquer recurso local quando o processo usa uma API interna para criar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="f3caf-225">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="f3caf-226">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="f3caf-226">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3caf-227">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="f3caf-227">userRightsDebugPrograms</span></span>|[<span data-ttu-id="f3caf-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-229">Esse direito de usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel.</span><span class="sxs-lookup"><span data-stu-id="f3caf-229">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="f3caf-230">Há suporte apenas para os Estados não configurado e permitido</span><span class="sxs-lookup"><span data-stu-id="f3caf-230">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="f3caf-231">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="f3caf-231">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="f3caf-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-233">Este direito de usuário determina quais usuários e grupos estão proibidos de fazer logon como um cliente de serviços de área de trabalho remota.</span><span class="sxs-lookup"><span data-stu-id="f3caf-233">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="f3caf-234">Há suporte apenas para os Estados não conFigurados e bloqueados</span><span class="sxs-lookup"><span data-stu-id="f3caf-234">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="f3caf-235">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="f3caf-235">userRightsDelegation</span></span>|[<span data-ttu-id="f3caf-236">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-236">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-237">Este direito de usuário determina quais usuários podem definir a configuração confiável para delegação em um objeto de usuário ou computador.</span><span class="sxs-lookup"><span data-stu-id="f3caf-237">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="f3caf-238">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-238">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-239">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="f3caf-239">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="f3caf-240">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-240">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-241">Este direito de usuário determina quais contas podem ser usadas por um processo para adicionar entradas ao log de segurança.</span><span class="sxs-lookup"><span data-stu-id="f3caf-241">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="f3caf-242">O log de segurança é usado para rastrear o acesso de sistema não autorizado.</span><span class="sxs-lookup"><span data-stu-id="f3caf-242">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="f3caf-243">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-243">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-244">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="f3caf-244">userRightsImpersonateClient</span></span>|[<span data-ttu-id="f3caf-245">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-245">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-246">A atribuição desse direito de usuário a um usuário permite que programas executados em nome desse usuário representem um cliente.</span><span class="sxs-lookup"><span data-stu-id="f3caf-246">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="f3caf-247">A exigência desse direito de usuário para esse tipo de representação impede que um usuário não autorizado convença um cliente a se conectar a um serviço que ele criou e, em seguida, representando esse cliente, o que pode elevar as permissões do usuário não autorizado para níveis administrativos ou de sistema.</span><span class="sxs-lookup"><span data-stu-id="f3caf-247">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="f3caf-248">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-248">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-249">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="f3caf-249">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="f3caf-250">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-250">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-251">Este direito de usuário determina quais contas podem usar um processo com acesso de propriedade de gravação a outro processo para aumentar a prioridade de execução atribuída ao outro processo.</span><span class="sxs-lookup"><span data-stu-id="f3caf-251">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="f3caf-252">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-253">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="f3caf-253">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="f3caf-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-255">Esse direito de usuário determina quais usuários podem carregar e descarregar dinamicamente drivers de dispositivo ou outro código no modo kernel.</span><span class="sxs-lookup"><span data-stu-id="f3caf-255">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="f3caf-256">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-257">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="f3caf-257">userRightsLockMemory</span></span>|[<span data-ttu-id="f3caf-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-259">Esse direito de usuário determina quais contas podem usar um processo para manter os dados na memória física, o que impede que o sistema pagine os dados para a memória virtual em disco.</span><span class="sxs-lookup"><span data-stu-id="f3caf-259">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="f3caf-260">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-261">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="f3caf-261">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="f3caf-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-263">Esse direito de usuário determina quais usuários podem especificar opções de auditoria de acesso a objetos para recursos individuais, como arquivos, objetos do Active Directory e chaves do registro.</span><span class="sxs-lookup"><span data-stu-id="f3caf-263">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="f3caf-264">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-265">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="f3caf-265">userRightsManageVolumes</span></span>|[<span data-ttu-id="f3caf-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-267">Esse direito de usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como a desfragmentação remota.</span><span class="sxs-lookup"><span data-stu-id="f3caf-267">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="f3caf-268">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-269">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="f3caf-269">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="f3caf-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-271">Esse direito de usuário determina quem pode modificar os valores de ambiente de firmware.</span><span class="sxs-lookup"><span data-stu-id="f3caf-271">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="f3caf-272">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-273">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="f3caf-273">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="f3caf-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-275">Este direito de usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves de registro ou processos pertencentes a outros usuários.</span><span class="sxs-lookup"><span data-stu-id="f3caf-275">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="f3caf-276">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-276">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-277">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="f3caf-277">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="f3caf-278">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-278">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-279">Esse direito de usuário determina quais usuários podem usar ferramentas de monitoramento de desempenho para monitorar o desempenho de processos do sistema.</span><span class="sxs-lookup"><span data-stu-id="f3caf-279">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="f3caf-280">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-280">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-281">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="f3caf-281">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="f3caf-282">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-282">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-283">Esse direito de usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede.</span><span class="sxs-lookup"><span data-stu-id="f3caf-283">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="f3caf-284">O mau uso desse direito de usuário pode resultar em uma negação de serviço.</span><span class="sxs-lookup"><span data-stu-id="f3caf-284">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="f3caf-285">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-286">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="f3caf-286">userRightsRestoreData</span></span>|[<span data-ttu-id="f3caf-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-288">Esse direito de usuário determina quais usuários podem ignorar permissões de arquivo, diretório, registro e outros objetos persistentes ao restaurar backups de arquivos e diretórios e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto.</span><span class="sxs-lookup"><span data-stu-id="f3caf-288">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="f3caf-289">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-289">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-290">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="f3caf-290">userRightsTakeOwnership</span></span>|[<span data-ttu-id="f3caf-291">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-291">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-292">Esse direito de usuário determina quais usuários podem assumir a propriedade de qualquer objeto protegível no sistema, incluindo objetos do Active Directory, arquivos e pastas, impressoras, chaves do registro, processos e threads.</span><span class="sxs-lookup"><span data-stu-id="f3caf-292">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="f3caf-293">Há suporte apenas para os Estados não conFigurados e permitidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-293">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="f3caf-294">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="f3caf-294">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="f3caf-295">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="f3caf-295">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="f3caf-296">Essa configuração de segurança determina quais contas de serviço são impedidas de registrar um processo como um serviço.</span><span class="sxs-lookup"><span data-stu-id="f3caf-296">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="f3caf-297">Observação: esta configuração de segurança não se aplica às contas de sistema, serviço local ou serviço de rede.</span><span class="sxs-lookup"><span data-stu-id="f3caf-297">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="f3caf-298">Só há suporte para o estado bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f3caf-298">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="f3caf-299">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="f3caf-299">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="f3caf-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-300">Boolean</span></span>|<span data-ttu-id="f3caf-301">Essa configuração determina se o salvamento de jogos do Xbox está habilitado (1) ou desabilitado (0).</span><span class="sxs-lookup"><span data-stu-id="f3caf-301">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="f3caf-302">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f3caf-302">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="f3caf-303">inStarttype</span><span class="sxs-lookup"><span data-stu-id="f3caf-303">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f3caf-304">Esta configuração determina se o tipo de início do serviço de gerenciamento de acessórios é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="f3caf-304">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f3caf-305">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="f3caf-305">Default: Manual.</span></span> <span data-ttu-id="f3caf-306">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-306">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f3caf-307">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f3caf-307">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="f3caf-308">inStarttype</span><span class="sxs-lookup"><span data-stu-id="f3caf-308">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f3caf-309">Essa configuração determina se o tipo de início do serviço do Live Authentication Manager é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="f3caf-309">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f3caf-310">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="f3caf-310">Default: Manual.</span></span> <span data-ttu-id="f3caf-311">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-311">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f3caf-312">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f3caf-312">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="f3caf-313">inStarttype</span><span class="sxs-lookup"><span data-stu-id="f3caf-313">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f3caf-314">Essa configuração determina se o tipo de início do serviço de salvamento do Live Game é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="f3caf-314">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f3caf-315">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="f3caf-315">Default: Manual.</span></span> <span data-ttu-id="f3caf-316">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-316">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f3caf-317">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="f3caf-317">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="f3caf-318">inStarttype</span><span class="sxs-lookup"><span data-stu-id="f3caf-318">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="f3caf-319">Esta configuração determina se o tipo de início do serviço de rede é automático (2), manual (3), desabilitado (4).</span><span class="sxs-lookup"><span data-stu-id="f3caf-319">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="f3caf-320">Padrão: manual.</span><span class="sxs-lookup"><span data-stu-id="f3caf-320">Default: Manual.</span></span> <span data-ttu-id="f3caf-321">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-321">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="f3caf-322">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="f3caf-322">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="f3caf-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-323">Boolean</span></span>|<span data-ttu-id="f3caf-324">Impedir que os usuários adicionem novas contas da Microsoft a este computador.</span><span class="sxs-lookup"><span data-stu-id="f3caf-324">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="f3caf-325">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="f3caf-325">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="f3caf-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-326">Boolean</span></span>|<span data-ttu-id="f3caf-327">Habilitar contas locais que não estão protegidas por senha para fazer logon de locais diferentes do dispositivo físico. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="f3caf-327">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="f3caf-328">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="f3caf-328">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="f3caf-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-329">Boolean</span></span>|<span data-ttu-id="f3caf-330">Determina se a conta de administrador local está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="f3caf-330">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="f3caf-331">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="f3caf-331">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="f3caf-332">String</span><span class="sxs-lookup"><span data-stu-id="f3caf-332">String</span></span>|<span data-ttu-id="f3caf-333">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "administrador".</span><span class="sxs-lookup"><span data-stu-id="f3caf-333">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="f3caf-334">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="f3caf-334">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="f3caf-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-335">Boolean</span></span>|<span data-ttu-id="f3caf-336">Determina se a conta de convidado está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="f3caf-336">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="f3caf-337">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="f3caf-337">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="f3caf-338">String</span><span class="sxs-lookup"><span data-stu-id="f3caf-338">String</span></span>|<span data-ttu-id="f3caf-339">Defina um nome de conta diferente a ser associado ao identificador de segurança (SID) da conta "convidado".</span><span class="sxs-lookup"><span data-stu-id="f3caf-339">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="f3caf-340">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="f3caf-340">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="f3caf-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-341">Boolean</span></span>|<span data-ttu-id="f3caf-342">Impedir que um computador portátil seja desencaixado sem ter que fazer logon.</span><span class="sxs-lookup"><span data-stu-id="f3caf-342">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="f3caf-343">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="f3caf-343">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="f3caf-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-344">Boolean</span></span>|<span data-ttu-id="f3caf-345">Restringir a instalação dos drivers de impressora como parte da conexão a uma impressora compartilhada somente para administradores.</span><span class="sxs-lookup"><span data-stu-id="f3caf-345">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="f3caf-346">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="f3caf-346">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="f3caf-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-347">Boolean</span></span>|<span data-ttu-id="f3caf-348">Habilitar essa configuração permite que somente o usuário conectado interativamente acesse a mídia de CD-ROM.</span><span class="sxs-lookup"><span data-stu-id="f3caf-348">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="f3caf-349">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="f3caf-349">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="f3caf-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="f3caf-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="f3caf-351">Defina quem tem permissão para formatar e ejetar a mídia NTFS removível.</span><span class="sxs-lookup"><span data-stu-id="f3caf-351">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="f3caf-352">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-352">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="f3caf-353">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="f3caf-353">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="f3caf-354">Int32</span><span class="sxs-lookup"><span data-stu-id="f3caf-354">Int32</span></span>|<span data-ttu-id="f3caf-355">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="f3caf-355">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="f3caf-356">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="f3caf-356">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="f3caf-357">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="f3caf-357">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="f3caf-358">Int32</span><span class="sxs-lookup"><span data-stu-id="f3caf-358">Int32</span></span>|<span data-ttu-id="f3caf-359">Defina o máximo de minutos de inatividade na tela de logon do desktop interativo até que a proteção de tela seja executada.</span><span class="sxs-lookup"><span data-stu-id="f3caf-359">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="f3caf-360">Valores válidos de 0 a 9999</span><span class="sxs-lookup"><span data-stu-id="f3caf-360">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="f3caf-361">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="f3caf-361">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="f3caf-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-362">Boolean</span></span>|<span data-ttu-id="f3caf-363">Exigir CTRL + ALT + DEL para ser pressionada para que um usuário possa fazer logon.</span><span class="sxs-lookup"><span data-stu-id="f3caf-363">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="f3caf-364">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="f3caf-364">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="f3caf-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-365">Boolean</span></span>|<span data-ttu-id="f3caf-366">Não exibe o nome de usuário da última pessoa que entrou neste dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3caf-366">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="f3caf-367">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="f3caf-367">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="f3caf-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-368">Boolean</span></span>|<span data-ttu-id="f3caf-369">Não exibe o nome de usuário da pessoa que está entrando neste dispositivo depois que as credenciais são inseridas e antes da área de trabalho do dispositivo ser exibida.</span><span class="sxs-lookup"><span data-stu-id="f3caf-369">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="f3caf-370">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="f3caf-370">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="f3caf-371">String</span><span class="sxs-lookup"><span data-stu-id="f3caf-371">String</span></span>|<span data-ttu-id="f3caf-372">Defina o título da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="f3caf-372">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="f3caf-373">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="f3caf-373">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="f3caf-374">String</span><span class="sxs-lookup"><span data-stu-id="f3caf-374">String</span></span>|<span data-ttu-id="f3caf-375">Definir o texto da mensagem para usuários que tentam fazer logon.</span><span class="sxs-lookup"><span data-stu-id="f3caf-375">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="f3caf-376">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="f3caf-376">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="f3caf-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-377">Boolean</span></span>|<span data-ttu-id="f3caf-378">Bloquear solicitações de autenticação PKU2U para este dispositivo para usar identidades online.</span><span class="sxs-lookup"><span data-stu-id="f3caf-378">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="f3caf-379">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="f3caf-379">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="f3caf-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-380">Boolean</span></span>|<span data-ttu-id="f3caf-381">Boolean do auxiliar da interface do usuário para entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="f3caf-381">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="f3caf-382">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="f3caf-382">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="f3caf-383">String</span><span class="sxs-lookup"><span data-stu-id="f3caf-383">String</span></span>|<span data-ttu-id="f3caf-384">Edite a cadeia de caracteres de definição de descritor de segurança padrão para permitir ou impedir que usuários e grupos façam chamadas remotas para o SAM.</span><span class="sxs-lookup"><span data-stu-id="f3caf-384">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="f3caf-385">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="f3caf-385">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="f3caf-386">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="f3caf-386">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="f3caf-387">Essa configuração de segurança permite que um cliente exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="f3caf-387">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="f3caf-388">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-388">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="f3caf-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="f3caf-389">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="f3caf-390">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="f3caf-390">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="f3caf-391">Essa configuração de segurança permite que um servidor exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="f3caf-391">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="f3caf-392">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-392">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="f3caf-393">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="f3caf-393">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="f3caf-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="f3caf-394">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="f3caf-395">Essa configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede.</span><span class="sxs-lookup"><span data-stu-id="f3caf-395">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="f3caf-396">Os possíveis valores são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-396">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="f3caf-397">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="f3caf-397">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="f3caf-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-398">Boolean</span></span>|<span data-ttu-id="f3caf-399">Se for habilitada, o cliente SMB permitirá logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="f3caf-399">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="f3caf-400">Se não configurada, o cliente SMB rejeitará logons de convidados não seguros.</span><span class="sxs-lookup"><span data-stu-id="f3caf-400">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="f3caf-401">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="f3caf-401">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="f3caf-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-402">Boolean</span></span>|<span data-ttu-id="f3caf-403">Configuração de segurança que determina se o arquivo de paginação de memória virtual será limpo quando o sistema for desligado.</span><span class="sxs-lookup"><span data-stu-id="f3caf-403">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="f3caf-404">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="f3caf-404">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="f3caf-405">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-405">Boolean</span></span>|<span data-ttu-id="f3caf-406">Configuração de segurança que determina se um computador pode ser desligado sem a necessidade de fazer logon no Windows.</span><span class="sxs-lookup"><span data-stu-id="f3caf-406">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="f3caf-407">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="f3caf-407">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="f3caf-408">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-408">Boolean</span></span>|<span data-ttu-id="f3caf-409">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="f3caf-409">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="f3caf-410">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="f3caf-410">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="f3caf-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-411">Boolean</span></span>|<span data-ttu-id="f3caf-412">Virtualizar falhas de gravação de arquivo e registro para locais por usuário</span><span class="sxs-lookup"><span data-stu-id="f3caf-412">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="f3caf-413">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="f3caf-413">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="f3caf-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-414">Boolean</span></span>|<span data-ttu-id="f3caf-415">Impor a validação de caminho de certificação PKI para um determinado arquivo executável antes que seja permitido executar.</span><span class="sxs-lookup"><span data-stu-id="f3caf-415">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="f3caf-416">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="f3caf-416">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="f3caf-417">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="f3caf-417">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="f3caf-418">Definir o comportamento do prompt de elevação para administradores no modo de aprovação de administrador.</span><span class="sxs-lookup"><span data-stu-id="f3caf-418">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="f3caf-419">Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-419">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="f3caf-420">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="f3caf-420">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="f3caf-421">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="f3caf-421">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="f3caf-422">Definir o comportamento do prompt de elevação para usuários padrão.</span><span class="sxs-lookup"><span data-stu-id="f3caf-422">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="f3caf-423">Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-423">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="f3caf-424">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="f3caf-424">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="f3caf-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-425">Boolean</span></span>|<span data-ttu-id="f3caf-426">Habilite todas as solicitações de elevação para ir para a área de trabalho do usuário interativo, e não para a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="f3caf-426">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="f3caf-427">As configurações de política de comportamento de prompt para administradores e usuários padrão são usadas.</span><span class="sxs-lookup"><span data-stu-id="f3caf-427">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="f3caf-428">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="f3caf-428">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="f3caf-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-429">Boolean</span></span>|<span data-ttu-id="f3caf-430">Instalações de aplicativos que exigem privilégios elevados solicitarão credenciais de administrador. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="f3caf-430">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="f3caf-431">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="f3caf-431">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="f3caf-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-432">Boolean</span></span>|<span data-ttu-id="f3caf-433">Permitir que aplicativos UIAccess solicitem elevação sem usar a área de trabalho segura. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="f3caf-433">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="f3caf-434">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="f3caf-434">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="f3caf-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-435">Boolean</span></span>|<span data-ttu-id="f3caf-436">Define se a conta de administrador interna usa o modo de aprovação de administrador ou executa todos os aplicativos com privilégios de administrador completo. O padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="f3caf-436">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="f3caf-437">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="f3caf-437">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="f3caf-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-438">Boolean</span></span>|<span data-ttu-id="f3caf-439">Definir se o modo de aprovação de administrador e todas as configurações de política de UAC estão habilitados, o padrão é habilitado</span><span class="sxs-lookup"><span data-stu-id="f3caf-439">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="f3caf-440">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="f3caf-440">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="f3caf-441">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="f3caf-441">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="f3caf-442">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f3caf-442">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="f3caf-443">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-443">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="f3caf-444">Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-444">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="f3caf-445">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="f3caf-445">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="f3caf-446">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="f3caf-446">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="f3caf-447">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="f3caf-447">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="f3caf-448">Se não configurada, o nome de exibição do usuário, o domínio e o nome de usuário serão exibidos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-448">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="f3caf-449">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-449">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="f3caf-450">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="f3caf-450">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="f3caf-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-451">Boolean</span></span>|<span data-ttu-id="f3caf-452">Configuração de segurança que determina se o cliente SMB tentará negociar assinatura de pacote SMB.</span><span class="sxs-lookup"><span data-stu-id="f3caf-452">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="f3caf-453">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="f3caf-453">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="f3caf-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-454">Boolean</span></span>|<span data-ttu-id="f3caf-455">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do cliente SMB.</span><span class="sxs-lookup"><span data-stu-id="f3caf-455">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="f3caf-456">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="f3caf-456">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="f3caf-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-457">Boolean</span></span>|<span data-ttu-id="f3caf-458">Se essa configuração de segurança estiver habilitada, o redirecionador de bloco de mensagens de servidor (SMB) terá permissão para enviar senhas de texto não criptografado para servidores SMB não Microsoft que não ofereçam suporte à criptografia de senha durante a autenticação.</span><span class="sxs-lookup"><span data-stu-id="f3caf-458">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="f3caf-459">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="f3caf-459">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="f3caf-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-460">Boolean</span></span>|<span data-ttu-id="f3caf-461">Configuração de segurança que determina se a assinatura de pacotes é necessária para o componente do servidor SMB.</span><span class="sxs-lookup"><span data-stu-id="f3caf-461">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="f3caf-462">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="f3caf-462">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="f3caf-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-463">Boolean</span></span>|<span data-ttu-id="f3caf-464">Configuração de segurança que determina se o servidor SMB negociará assinatura de pacote SMB com clientes que solicitarem.</span><span class="sxs-lookup"><span data-stu-id="f3caf-464">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="f3caf-465">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="f3caf-465">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="f3caf-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-466">Boolean</span></span>|<span data-ttu-id="f3caf-467">Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e pipes para as configurações de pipes nomeados que podem ser acessados anonimamente e comPartilhamentos que podem ser acessados anonimamente</span><span class="sxs-lookup"><span data-stu-id="f3caf-467">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="f3caf-468">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="f3caf-468">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="f3caf-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-469">Boolean</span></span>|<span data-ttu-id="f3caf-470">Essa configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas com o computador.</span><span class="sxs-lookup"><span data-stu-id="f3caf-470">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="f3caf-471">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="f3caf-471">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="f3caf-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-472">Boolean</span></span>|<span data-ttu-id="f3caf-473">Configuração de segurança que determina se os usuários anônimos devem executar determinadas atividades, como enumeração de nomes de contas de domínio e compartilhamentos de rede.</span><span class="sxs-lookup"><span data-stu-id="f3caf-473">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="f3caf-474">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="f3caf-474">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="f3caf-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-475">Boolean</span></span>|<span data-ttu-id="f3caf-476">Essa configuração de segurança determina se, na próxima alteração de senha, o valor de hash do LM (LAN Manager) para a nova senha é armazenado.</span><span class="sxs-lookup"><span data-stu-id="f3caf-476">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="f3caf-477">Ele não é armazenado por padrão.</span><span class="sxs-lookup"><span data-stu-id="f3caf-477">It’s not stored by default.</span></span>|
|<span data-ttu-id="f3caf-478">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="f3caf-478">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="f3caf-479">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="f3caf-479">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="f3caf-480">Essa configuração de segurança determina o que acontece quando o cartão inteligente de um usuário conectado é removido do leitor de cartão inteligente.</span><span class="sxs-lookup"><span data-stu-id="f3caf-480">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="f3caf-481">Os valores possíveis são: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-481">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="f3caf-482">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-482">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="f3caf-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-483">Boolean</span></span>|<span data-ttu-id="f3caf-484">Usado para desabilitar a exibição da área de proteção de aplicativo e navegador.</span><span class="sxs-lookup"><span data-stu-id="f3caf-484">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="f3caf-485">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-485">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="f3caf-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-486">Boolean</span></span>|<span data-ttu-id="f3caf-487">Usado para desabilitar a exibição da área de opções da família.</span><span class="sxs-lookup"><span data-stu-id="f3caf-487">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="f3caf-488">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-488">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="f3caf-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-489">Boolean</span></span>|<span data-ttu-id="f3caf-490">Usado para desabilitar a exibição da área de desempenho e integridade do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3caf-490">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="f3caf-491">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-491">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="f3caf-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-492">Boolean</span></span>|<span data-ttu-id="f3caf-493">Usado para desabilitar a exibição da área de firewall e proteção de rede.</span><span class="sxs-lookup"><span data-stu-id="f3caf-493">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="f3caf-494">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-494">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="f3caf-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-495">Boolean</span></span>|<span data-ttu-id="f3caf-496">Usado para desabilitar a exibição da área de proteção contra vírus e ameaças.</span><span class="sxs-lookup"><span data-stu-id="f3caf-496">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="f3caf-497">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-497">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="f3caf-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-498">Boolean</span></span>|<span data-ttu-id="f3caf-499">Usado para desabilitar a exibição da área de proteção da conta.</span><span class="sxs-lookup"><span data-stu-id="f3caf-499">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="f3caf-500">defenderSecurityCenterDisableClearTpmUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-500">defenderSecurityCenterDisableClearTpmUI</span></span>|<span data-ttu-id="f3caf-501">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-501">Boolean</span></span>|<span data-ttu-id="f3caf-502">Usado para desabilitar a exibição do botão limpar TPM.</span><span class="sxs-lookup"><span data-stu-id="f3caf-502">Used to disable the display of the Clear TPM button.</span></span>|
|<span data-ttu-id="f3caf-503">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-503">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="f3caf-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-504">Boolean</span></span>|<span data-ttu-id="f3caf-505">Usado para desabilitar a exibição da área de proteção de hardware.</span><span class="sxs-lookup"><span data-stu-id="f3caf-505">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="f3caf-506">defenderSecurityCenterDisableNotificationAreaUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-506">defenderSecurityCenterDisableNotificationAreaUI</span></span>|<span data-ttu-id="f3caf-507">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-507">Boolean</span></span>|<span data-ttu-id="f3caf-508">Usado para desabilitar a exibição do controle da área de notificação.</span><span class="sxs-lookup"><span data-stu-id="f3caf-508">Used to disable the display of the notification area control.</span></span> <span data-ttu-id="f3caf-509">O usuário precisa sair e entrar ou reiniciar o computador para que essa configuração entre em vigor.</span><span class="sxs-lookup"><span data-stu-id="f3caf-509">The user needs to either sign out and sign in or reboot the computer for this setting to take effect.</span></span>|
|<span data-ttu-id="f3caf-510">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-510">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="f3caf-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-511">Boolean</span></span>|<span data-ttu-id="f3caf-512">Usado para desabilitar a exibição da área de proteção contra ransomware.</span><span class="sxs-lookup"><span data-stu-id="f3caf-512">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="f3caf-513">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-513">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="f3caf-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-514">Boolean</span></span>|<span data-ttu-id="f3caf-515">Usado para desabilitar a exibição da área de inicialização segura sob segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3caf-515">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="f3caf-516">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-516">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="f3caf-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-517">Boolean</span></span>|<span data-ttu-id="f3caf-518">Usado para desabilitar a exibição do processo de segurança Solucionando problemas de segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3caf-518">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="f3caf-519">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span><span class="sxs-lookup"><span data-stu-id="f3caf-519">defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI</span></span>|<span data-ttu-id="f3caf-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-520">Boolean</span></span>|<span data-ttu-id="f3caf-521">Usado para desabilitar a exibição de atualizar o firmware do TPM quando um firmware vulnerável é detectado.</span><span class="sxs-lookup"><span data-stu-id="f3caf-521">Used to disable the display of update TPM Firmware when a vulnerable firmware is detected.</span></span>|
|<span data-ttu-id="f3caf-522">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="f3caf-522">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="f3caf-523">String</span><span class="sxs-lookup"><span data-stu-id="f3caf-523">String</span></span>|<span data-ttu-id="f3caf-524">O nome da empresa que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="f3caf-524">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="f3caf-525">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="f3caf-525">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="f3caf-526">String</span><span class="sxs-lookup"><span data-stu-id="f3caf-526">String</span></span>|<span data-ttu-id="f3caf-527">O endereço de email que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="f3caf-527">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="f3caf-528">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="f3caf-528">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="f3caf-529">String</span><span class="sxs-lookup"><span data-stu-id="f3caf-529">String</span></span>|<span data-ttu-id="f3caf-530">O número de telefone ou Skype ID que é exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="f3caf-530">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="f3caf-531">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="f3caf-531">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="f3caf-532">String</span><span class="sxs-lookup"><span data-stu-id="f3caf-532">String</span></span>|<span data-ttu-id="f3caf-533">A URL do portal da ajuda que é exibida para os usuários.</span><span class="sxs-lookup"><span data-stu-id="f3caf-533">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="f3caf-534">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="f3caf-534">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="f3caf-535">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="f3caf-535">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="f3caf-536">Notificações para mostrar das áreas de aplicativo exibidas.</span><span class="sxs-lookup"><span data-stu-id="f3caf-536">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="f3caf-537">Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-537">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="f3caf-538">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="f3caf-538">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="f3caf-539">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="f3caf-539">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="f3caf-540">Configurar onde exibir informações de contato de ti para usuários finais.</span><span class="sxs-lookup"><span data-stu-id="f3caf-540">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="f3caf-541">Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-541">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="f3caf-542">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="f3caf-542">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="f3caf-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-543">Boolean</span></span>|<span data-ttu-id="f3caf-544">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="f3caf-544">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="f3caf-545">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="f3caf-545">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="f3caf-546">Int32</span><span class="sxs-lookup"><span data-stu-id="f3caf-546">Int32</span></span>|<span data-ttu-id="f3caf-547">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="f3caf-547">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="f3caf-548">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="f3caf-548">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="f3caf-549">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="f3caf-549">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="f3caf-550">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="f3caf-550">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="f3caf-551">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="f3caf-551">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="f3caf-552">Selecione a codificação de chave pré-compartilhada a ser usada.</span><span class="sxs-lookup"><span data-stu-id="f3caf-552">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="f3caf-553">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-553">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="f3caf-554">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="f3caf-554">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="f3caf-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-555">Boolean</span></span>|<span data-ttu-id="f3caf-556">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="f3caf-556">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="f3caf-557">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="f3caf-557">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="f3caf-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-558">Boolean</span></span>|<span data-ttu-id="f3caf-559">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="f3caf-559">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="f3caf-560">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="f3caf-560">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="f3caf-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-561">Boolean</span></span>|<span data-ttu-id="f3caf-562">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="f3caf-562">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="f3caf-563">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="f3caf-563">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="f3caf-564">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-564">Boolean</span></span>|<span data-ttu-id="f3caf-565">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="f3caf-565">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="f3caf-566">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="f3caf-566">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="f3caf-567">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="f3caf-567">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="f3caf-568">Especifique como a lista de certificados revogados será imposta.</span><span class="sxs-lookup"><span data-stu-id="f3caf-568">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="f3caf-569">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-569">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="f3caf-570">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="f3caf-570">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="f3caf-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-571">Boolean</span></span>|<span data-ttu-id="f3caf-572">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="f3caf-572">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="f3caf-573">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="f3caf-573">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="f3caf-574">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="f3caf-574">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="f3caf-575">Configura como o enfileiramento de pacotes deve ser aplicado no cenário de gateway de túnel.</span><span class="sxs-lookup"><span data-stu-id="f3caf-575">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="f3caf-576">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-576">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="f3caf-577">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="f3caf-577">firewallProfileDomain</span></span>|[<span data-ttu-id="f3caf-578">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f3caf-578">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="f3caf-579">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="f3caf-579">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="f3caf-580">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="f3caf-580">firewallProfilePublic</span></span>|[<span data-ttu-id="f3caf-581">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f3caf-581">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="f3caf-582">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="f3caf-582">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="f3caf-583">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="f3caf-583">firewallProfilePrivate</span></span>|[<span data-ttu-id="f3caf-584">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f3caf-584">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="f3caf-585">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="f3caf-585">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="f3caf-586">defenderAdobeReaderLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="f3caf-586">defenderAdobeReaderLaunchChildProcess</span></span>|[<span data-ttu-id="f3caf-587">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-587">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-588">O valor que indica o comportamento do Adobe Reader de criar processos filhos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-588">Value indicating the behavior of Adobe Reader from creating child processes.</span></span> <span data-ttu-id="f3caf-589">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-589">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-590">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="f3caf-590">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="f3caf-591">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f3caf-591">String collection</span></span>|<span data-ttu-id="f3caf-592">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="f3caf-592">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="f3caf-593">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-593">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="f3caf-594">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3caf-594">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3caf-595">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-595">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="f3caf-596">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-596">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-597">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="f3caf-597">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="f3caf-598">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-598">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-599">Valor que indica o comportamento dos aplicativos do Office que injetam em outros processos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-599">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="f3caf-600">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-600">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-601">defenderOfficeCommunicationAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="f3caf-601">defenderOfficeCommunicationAppsLaunchChildProcess</span></span>|[<span data-ttu-id="f3caf-602">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-602">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-603">O valor que indica o comportamento dos aplicativos de comunicação do Office, incluindo o Microsoft Outlook, da criação de processos filhos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-603">Value indicating the behavior of Office communication applications, including Microsoft Outlook, from creating child processes.</span></span> <span data-ttu-id="f3caf-604">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-604">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-605">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="f3caf-605">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="f3caf-606">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3caf-606">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3caf-607">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="f3caf-607">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="f3caf-608">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-608">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-609">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="f3caf-609">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="f3caf-610">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-610">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-611">Valor que indica o comportamento de aplicativos/macros do Office criando ou iniciando conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="f3caf-611">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="f3caf-612">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-612">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-613">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="f3caf-613">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="f3caf-614">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3caf-614">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3caf-615">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-615">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="f3caf-616">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-616">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-617">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="f3caf-617">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="f3caf-618">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-618">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-619">Valor que indica o comportamento do aplicativo do Office que está iniciando processos filhos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-619">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="f3caf-620">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-620">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-621">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="f3caf-621">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="f3caf-622">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3caf-622">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3caf-623">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="f3caf-623">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="f3caf-624">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-624">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-625">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="f3caf-625">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="f3caf-626">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-626">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-627">Valor que indica o comportamento das importações Win32 do código de macro no Office.</span><span class="sxs-lookup"><span data-stu-id="f3caf-627">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="f3caf-628">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-628">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-629">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="f3caf-629">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="f3caf-630">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3caf-630">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3caf-631">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="f3caf-631">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="f3caf-632">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-632">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-633">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="f3caf-633">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="f3caf-634">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-634">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-635">Valor que indica o comportamento do código js/vbs/PS/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="f3caf-635">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="f3caf-636">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-636">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-637">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-637">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="f3caf-638">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3caf-638">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3caf-639">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="f3caf-639">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="f3caf-640">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-640">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-641">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="f3caf-641">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="f3caf-642">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-642">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-643">O valor que indica o comportamento do js/vbs executando a carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="f3caf-643">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="f3caf-644">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-644">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-645">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="f3caf-645">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="f3caf-646">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-646">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-647">Valor que indica se a credencial que está sendo roubada do subsistema de autoridade de segurança local do Windows é permitida.</span><span class="sxs-lookup"><span data-stu-id="f3caf-647">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="f3caf-648">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-648">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-649">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="f3caf-649">defenderProcessCreationType</span></span>|[<span data-ttu-id="f3caf-650">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3caf-650">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3caf-651">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="f3caf-651">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="f3caf-652">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-652">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-653">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="f3caf-653">defenderProcessCreation</span></span>|[<span data-ttu-id="f3caf-654">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-654">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-655">O valor que indica a resposta a criações de processos que se originam de comandos do PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="f3caf-655">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="f3caf-656">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-656">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-657">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="f3caf-657">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="f3caf-658">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3caf-658">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3caf-659">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="f3caf-659">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="f3caf-660">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-660">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-661">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="f3caf-661">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="f3caf-662">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-662">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-663">Valor que indica a resposta a processos não confiáveis e não assinados executados no USB.</span><span class="sxs-lookup"><span data-stu-id="f3caf-663">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="f3caf-664">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-664">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-665">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="f3caf-665">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="f3caf-666">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3caf-666">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3caf-667">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="f3caf-667">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="f3caf-668">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-668">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-669">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="f3caf-669">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="f3caf-670">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-671">Valor que indica a resposta a executáveis que não atendem a um critério de lista predominante, de idade ou confiável.</span><span class="sxs-lookup"><span data-stu-id="f3caf-671">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="f3caf-672">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-673">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-673">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="f3caf-674">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="f3caf-674">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="f3caf-675">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="f3caf-675">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="f3caf-676">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-676">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-677">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="f3caf-677">defenderEmailContentExecution</span></span>|[<span data-ttu-id="f3caf-678">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-678">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-679">O valor que indica se a execução do conteúdo executável (exe, dll, PS, js, vbs, etc.) deve ser cancelada de email (webmail/email).</span><span class="sxs-lookup"><span data-stu-id="f3caf-679">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="f3caf-680">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-680">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-681">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-681">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="f3caf-682">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-682">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-683">O valor que indica o uso da proteção avançada contra o Ransomeware.</span><span class="sxs-lookup"><span data-stu-id="f3caf-683">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="f3caf-684">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-684">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-685">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="f3caf-685">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="f3caf-686">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-686">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="f3caf-687">Valor que indica o comportamento das pastas protegidas.</span><span class="sxs-lookup"><span data-stu-id="f3caf-687">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="f3caf-688">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-688">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="f3caf-689">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="f3caf-689">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="f3caf-690">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3caf-690">String collection</span></span>|<span data-ttu-id="f3caf-691">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="f3caf-691">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="f3caf-692">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="f3caf-692">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="f3caf-693">Coleção String</span><span class="sxs-lookup"><span data-stu-id="f3caf-693">String collection</span></span>|<span data-ttu-id="f3caf-694">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="f3caf-694">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="f3caf-695">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-695">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="f3caf-696">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="f3caf-696">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="f3caf-697">Valor que indica o comportamento de NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="f3caf-697">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="f3caf-698">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-698">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="f3caf-699">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="f3caf-699">defenderExploitProtectionXml</span></span>|<span data-ttu-id="f3caf-700">Binária</span><span class="sxs-lookup"><span data-stu-id="f3caf-700">Binary</span></span>|<span data-ttu-id="f3caf-701">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="f3caf-701">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="f3caf-702">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="f3caf-702">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="f3caf-703">String</span><span class="sxs-lookup"><span data-stu-id="f3caf-703">String</span></span>|<span data-ttu-id="f3caf-704">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="f3caf-704">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="f3caf-705">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="f3caf-705">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="f3caf-706">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-706">Boolean</span></span>|<span data-ttu-id="f3caf-707">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="f3caf-707">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="f3caf-708">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="f3caf-708">appLockerApplicationControl</span></span>|[<span data-ttu-id="f3caf-709">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="f3caf-709">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="f3caf-710">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-710">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="f3caf-711">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-711">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="f3caf-712">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="f3caf-712">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="f3caf-713">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="f3caf-713">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="f3caf-714">Ative o Credential Guard quando o nível de segurança da plataforma com segurança baseada em inicialização e virtualização segura estiverem habilitados.</span><span class="sxs-lookup"><span data-stu-id="f3caf-714">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="f3caf-715">Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-715">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="f3caf-716">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="f3caf-716">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="f3caf-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-717">Boolean</span></span>|<span data-ttu-id="f3caf-718">Ativa a segurança baseada em virtualização (VBS).</span><span class="sxs-lookup"><span data-stu-id="f3caf-718">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="f3caf-719">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="f3caf-719">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="f3caf-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-720">Boolean</span></span>|<span data-ttu-id="f3caf-721">Especifica se o nível de segurança da plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="f3caf-721">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="f3caf-722">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="f3caf-722">deviceGuardLaunchSystemGuard</span></span>|[<span data-ttu-id="f3caf-723">habilitação</span><span class="sxs-lookup"><span data-stu-id="f3caf-723">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f3caf-724">Permite que o administrador de ti configure o lançamento do System Guard.</span><span class="sxs-lookup"><span data-stu-id="f3caf-724">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="f3caf-725">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-725">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f3caf-726">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="f3caf-726">smartScreenEnableInShell</span></span>|<span data-ttu-id="f3caf-727">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-727">Boolean</span></span>|<span data-ttu-id="f3caf-728">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="f3caf-728">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="f3caf-729">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="f3caf-729">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="f3caf-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-730">Boolean</span></span>|<span data-ttu-id="f3caf-731">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="f3caf-731">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="f3caf-732">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="f3caf-732">applicationGuardEnabled</span></span>|<span data-ttu-id="f3caf-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-733">Boolean</span></span>|<span data-ttu-id="f3caf-734">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="f3caf-734">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="f3caf-735">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="f3caf-735">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="f3caf-736">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="f3caf-736">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="f3caf-737">Habilitar o Windows Defender Application Guard para novas versões do Windows.</span><span class="sxs-lookup"><span data-stu-id="f3caf-737">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="f3caf-738">Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-738">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="f3caf-739">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="f3caf-739">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="f3caf-740">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="f3caf-740">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="f3caf-741">Bloquear a área de transferência para transferir o arquivo de imagem, o arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="f3caf-741">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="f3caf-742">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-742">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="f3caf-743">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="f3caf-743">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="f3caf-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-744">Boolean</span></span>|<span data-ttu-id="f3caf-745">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="f3caf-745">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="f3caf-746">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="f3caf-746">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="f3caf-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-747">Boolean</span></span>|<span data-ttu-id="f3caf-748">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="f3caf-748">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="f3caf-749">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="f3caf-749">applicationGuardForceAuditing</span></span>|<span data-ttu-id="f3caf-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-750">Boolean</span></span>|<span data-ttu-id="f3caf-751">A auditoria forçada manterá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)
</span><span class="sxs-lookup"><span data-stu-id="f3caf-751">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="f3caf-752">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="f3caf-752">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="f3caf-753">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="f3caf-753">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="f3caf-754">Impedir a área de transferência de compartilhar dados do Host para o Contêiner, do Contêiner para o Host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="f3caf-754">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="f3caf-755">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="f3caf-755">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="f3caf-756">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="f3caf-756">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="f3caf-757">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-757">Boolean</span></span>|<span data-ttu-id="f3caf-758">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="f3caf-758">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="f3caf-759">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="f3caf-759">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="f3caf-760">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-760">Boolean</span></span>|<span data-ttu-id="f3caf-761">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="f3caf-761">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="f3caf-762">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="f3caf-762">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="f3caf-763">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-763">Boolean</span></span>|<span data-ttu-id="f3caf-764">Permitir a impressão em Impressoras Locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="f3caf-764">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="f3caf-765">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="f3caf-765">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="f3caf-766">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-766">Boolean</span></span>|<span data-ttu-id="f3caf-767">Permitir a impressão em Impressoras da Rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="f3caf-767">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="f3caf-768">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="f3caf-768">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="f3caf-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-769">Boolean</span></span>|<span data-ttu-id="f3caf-770">Permitir que o Application Guard use virtual GPU</span><span class="sxs-lookup"><span data-stu-id="f3caf-770">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="f3caf-771">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="f3caf-771">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="f3caf-772">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-772">Boolean</span></span>|<span data-ttu-id="f3caf-773">Permitir que os usuários baixem arquivos da borda no contêiner do Application Guard e salve-os no sistema de arquivos host</span><span class="sxs-lookup"><span data-stu-id="f3caf-773">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="f3caf-774">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="f3caf-774">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="f3caf-775">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-775">Boolean</span></span>|<span data-ttu-id="f3caf-776">Permite que o administrador permita que os usuários padrão habilitem o encrpytion durante o ingresso no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f3caf-776">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="f3caf-777">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="f3caf-777">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="f3caf-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-778">Boolean</span></span>|<span data-ttu-id="f3caf-779">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="f3caf-779">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="f3caf-780">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="f3caf-780">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="f3caf-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-781">Boolean</span></span>|<span data-ttu-id="f3caf-782">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="f3caf-782">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="f3caf-783">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="f3caf-783">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="f3caf-784">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="f3caf-784">bitLockerEncryptDevice</span></span>|<span data-ttu-id="f3caf-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3caf-785">Boolean</span></span>|<span data-ttu-id="f3caf-786">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="f3caf-786">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="f3caf-787">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f3caf-787">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="f3caf-788">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f3caf-788">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="f3caf-789">Política de unidade de sistema BitLocker.</span><span class="sxs-lookup"><span data-stu-id="f3caf-789">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="f3caf-790">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f3caf-790">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="f3caf-791">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f3caf-791">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="f3caf-792">Política de unidade fixa do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="f3caf-792">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="f3caf-793">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f3caf-793">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="f3caf-794">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="f3caf-794">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="f3caf-795">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="f3caf-795">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="f3caf-796">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3caf-796">Response</span></span>
<span data-ttu-id="f3caf-797">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3caf-797">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3caf-798">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3caf-798">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3caf-799">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3caf-799">Request</span></span>
<span data-ttu-id="f3caf-800">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3caf-800">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 26778

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

### <a name="response"></a><span data-ttu-id="f3caf-801">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3caf-801">Response</span></span>
<span data-ttu-id="f3caf-p198">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3caf-p198">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 26950

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




