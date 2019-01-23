---
title: Atualizar windows10EndpointProtectionConfiguration
description: Atualizar as propriedades de um objeto windows10EndpointProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9bb398da325f6895eee7dd5e53938f8dafc5d5f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393617"
---
# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="e51de-103">Atualizar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="e51de-103">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="e51de-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e51de-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e51de-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e51de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e51de-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e51de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e51de-107">Atualizar as propriedades de um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e51de-107">Update the properties of a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e51de-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e51de-108">Prerequisites</span></span>
<span data-ttu-id="e51de-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e51de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e51de-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e51de-111">Permission type</span></span>|<span data-ttu-id="e51de-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e51de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e51de-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e51de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e51de-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e51de-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e51de-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e51de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e51de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e51de-116">Not supported.</span></span>|
|<span data-ttu-id="e51de-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e51de-117">Application</span></span>|<span data-ttu-id="e51de-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e51de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e51de-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e51de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e51de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e51de-120">Request headers</span></span>
|<span data-ttu-id="e51de-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e51de-121">Header</span></span>|<span data-ttu-id="e51de-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e51de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e51de-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e51de-123">Authorization</span></span>|<span data-ttu-id="e51de-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e51de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e51de-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e51de-125">Accept</span></span>|<span data-ttu-id="e51de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e51de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e51de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e51de-127">Request body</span></span>
<span data-ttu-id="e51de-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e51de-128">In the request body, supply a JSON representation for the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="e51de-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e51de-129">The following table shows the properties that are required when you create the [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="e51de-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e51de-130">Property</span></span>|<span data-ttu-id="e51de-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e51de-131">Type</span></span>|<span data-ttu-id="e51de-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e51de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e51de-133">id</span><span class="sxs-lookup"><span data-stu-id="e51de-133">id</span></span>|<span data-ttu-id="e51de-134">String</span><span class="sxs-lookup"><span data-stu-id="e51de-134">String</span></span>|<span data-ttu-id="e51de-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e51de-135">Key of the entity.</span></span> <span data-ttu-id="e51de-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e51de-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e51de-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e51de-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e51de-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e51de-138">DateTimeOffset</span></span>|<span data-ttu-id="e51de-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e51de-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e51de-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e51de-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e51de-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e51de-141">roleScopeTagIds</span></span>|<span data-ttu-id="e51de-142">String collection</span><span class="sxs-lookup"><span data-stu-id="e51de-142">String collection</span></span>|<span data-ttu-id="e51de-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="e51de-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e51de-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e51de-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e51de-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e51de-145">supportsScopeTags</span></span>|<span data-ttu-id="e51de-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-146">Boolean</span></span>|<span data-ttu-id="e51de-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e51de-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e51de-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e51de-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e51de-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="e51de-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e51de-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e51de-150">This property is read-only.</span></span> <span data-ttu-id="e51de-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e51de-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e51de-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e51de-152">createdDateTime</span></span>|<span data-ttu-id="e51de-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e51de-153">DateTimeOffset</span></span>|<span data-ttu-id="e51de-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e51de-154">DateTime the object was created.</span></span> <span data-ttu-id="e51de-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e51de-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e51de-156">description</span><span class="sxs-lookup"><span data-stu-id="e51de-156">description</span></span>|<span data-ttu-id="e51de-157">String</span><span class="sxs-lookup"><span data-stu-id="e51de-157">String</span></span>|<span data-ttu-id="e51de-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e51de-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e51de-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e51de-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e51de-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e51de-160">displayName</span></span>|<span data-ttu-id="e51de-161">String</span><span class="sxs-lookup"><span data-stu-id="e51de-161">String</span></span>|<span data-ttu-id="e51de-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e51de-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e51de-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e51de-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e51de-164">version</span><span class="sxs-lookup"><span data-stu-id="e51de-164">version</span></span>|<span data-ttu-id="e51de-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e51de-165">Int32</span></span>|<span data-ttu-id="e51de-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e51de-166">Version of the device configuration.</span></span> <span data-ttu-id="e51de-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e51de-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e51de-168">dmaGuardDeviceEnumerationPolicy</span><span class="sxs-lookup"><span data-stu-id="e51de-168">dmaGuardDeviceEnumerationPolicy</span></span>|[<span data-ttu-id="e51de-169">dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="e51de-169">dmaGuardDeviceEnumerationPolicyType</span></span>](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|<span data-ttu-id="e51de-170">Essa diretiva destina-se para fornecer segurança adicional em relação a dispositivos externos de capaz de DMA.</span><span class="sxs-lookup"><span data-stu-id="e51de-170">This policy is intended to provide additional security against external DMA capable devices.</span></span> <span data-ttu-id="e51de-171">Ele permite mais controle sobre a enumeração de dispositivos externos de capaz de DMA incompatível com área restrita e isolamento de memória DMA Remapping/dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e51de-171">It allows for more control over the enumeration of external DMA capable devices incompatible with DMA Remapping/device memory isolation and sandboxing.</span></span> <span data-ttu-id="e51de-172">Essa diretiva só entrará em vigor quando Kernel DMA proteção é suportada e ativada pelo firmware do sistema.</span><span class="sxs-lookup"><span data-stu-id="e51de-172">This policy only takes effect when Kernel DMA Protection is supported and enabled by the system firmware.</span></span> <span data-ttu-id="e51de-173">Proteção de DMA kernel é um recurso de plataforma que não pode ser controlado por meio da diretiva ou pelo usuário final.</span><span class="sxs-lookup"><span data-stu-id="e51de-173">Kernel DMA Protection is a platform feature that cannot be controlled via policy or by end user.</span></span> <span data-ttu-id="e51de-174">Ele deve ser suportada pelo sistema no momento da fabricação.</span><span class="sxs-lookup"><span data-stu-id="e51de-174">It has to be supported by the system at the time of manufacturing.</span></span> <span data-ttu-id="e51de-175">Para verificar se o sistema suporta Kernel DMA proteção, verifique o campo de proteção do Kernel DMA na página Resumo da MSINFO32.exe.</span><span class="sxs-lookup"><span data-stu-id="e51de-175">To check if the system supports Kernel DMA Protection, please check the Kernel DMA Protection field in the Summary page of MSINFO32.exe.</span></span> <span data-ttu-id="e51de-176">Os valores possíveis são: `deviceDefault`, `blockAll`, `allowAll`.</span><span class="sxs-lookup"><span data-stu-id="e51de-176">Possible values are: `deviceDefault`, `blockAll`, `allowAll`.</span></span>|
|<span data-ttu-id="e51de-177">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="e51de-177">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="e51de-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-179">Esse direito de usuário é usado pelo Gerenciador de credenciais durante Backup/restauração.</span><span class="sxs-lookup"><span data-stu-id="e51de-179">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="e51de-180">As credenciais dos usuários salvas podem ficar comprometidas se esse privilégio é fornecido a outras entidades.</span><span class="sxs-lookup"><span data-stu-id="e51de-180">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="e51de-181">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="e51de-181">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="e51de-182">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="e51de-182">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="e51de-183">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-183">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-184">Este direito de usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="e51de-184">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="e51de-185">Há suporte para o estado permitidos.</span><span class="sxs-lookup"><span data-stu-id="e51de-185">State Allowed is supported.</span></span>|
|<span data-ttu-id="e51de-186">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="e51de-186">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="e51de-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-188">Esse direito de usuário determina quais usuários e grupos estão bloco de conectar-se ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="e51de-188">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="e51de-189">Bloco de controle de sessão é suportado.</span><span class="sxs-lookup"><span data-stu-id="e51de-189">State Block is supported.</span></span>|
|<span data-ttu-id="e51de-190">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e51de-190">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="e51de-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-192">Esse direito de usuário permite que um processo representar qualquer usuário sem autenticação.</span><span class="sxs-lookup"><span data-stu-id="e51de-192">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="e51de-193">O processo, portanto, pode ter acesso aos mesmos recursos locais que esse usuário.</span><span class="sxs-lookup"><span data-stu-id="e51de-193">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="e51de-194">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="e51de-194">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="e51de-195">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="e51de-195">userRightsLocalLogOn</span></span>|[<span data-ttu-id="e51de-196">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-196">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-197">Esse direito de usuário determina quais usuários podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="e51de-197">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="e51de-198">Estados de não-configuradas, permitidos e bloqueados são suportados</span><span class="sxs-lookup"><span data-stu-id="e51de-198">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="e51de-199">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="e51de-199">userRightsBackupData</span></span>|[<span data-ttu-id="e51de-200">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-200">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-201">Esse direito de usuário determina quais usuários podem ignorar arquivo, diretório, registro e outras permissões de objetos persistentes ao fazer backup de arquivos e diretórios.</span><span class="sxs-lookup"><span data-stu-id="e51de-201">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="e51de-202">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="e51de-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="e51de-203">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="e51de-203">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="e51de-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-205">Esse direito de usuário determina quais usuários e grupos podem alterar a hora e data do relógio interno do computador.</span><span class="sxs-lookup"><span data-stu-id="e51de-205">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="e51de-206">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="e51de-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="e51de-207">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="e51de-207">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="e51de-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-209">Essa configuração determina se os usuários podem criar objetos globais que estão disponíveis para todas as sessões.</span><span class="sxs-lookup"><span data-stu-id="e51de-209">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="e51de-210">Usuários que podem criar objetos globais poderá afetar os processos executados em sessões de outros usuários, que pode levar à corrupção de dados ou falha do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e51de-210">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="e51de-211">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="e51de-211">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="e51de-212">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="e51de-212">userRightsCreatePageFile</span></span>|[<span data-ttu-id="e51de-213">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-213">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-214">Este direito de usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de paginação.</span><span class="sxs-lookup"><span data-stu-id="e51de-214">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="e51de-215">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="e51de-215">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="e51de-216">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="e51de-216">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="e51de-217">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-217">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-218">Esse direito de usuário determina quais contas podem ser usadas por processos para criar um objeto de diretório usando o objeto Gerenciador.</span><span class="sxs-lookup"><span data-stu-id="e51de-218">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="e51de-219">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="e51de-219">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="e51de-220">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="e51de-220">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="e51de-221">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-221">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-222">Esse direito de usuário determina se o usuário pode criar um link simbólico do computador ao qual ele esteja conectados.</span><span class="sxs-lookup"><span data-stu-id="e51de-222">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="e51de-223">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="e51de-223">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="e51de-224">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="e51de-224">userRightsCreateToken</span></span>|[<span data-ttu-id="e51de-225">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-225">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-226">Este direito de usuário determina quais usuários/grupos podem ser usados por processos para criar um token que pode ser usado para obter acesso a qualquer recurso local quando o processo usa uma API interna para criar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="e51de-226">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="e51de-227">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="e51de-227">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="e51de-228">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="e51de-228">userRightsDebugPrograms</span></span>|[<span data-ttu-id="e51de-229">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-229">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-230">Esse direito de usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel.</span><span class="sxs-lookup"><span data-stu-id="e51de-230">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="e51de-231">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="e51de-231">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="e51de-232">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="e51de-232">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="e51de-233">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-233">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-234">Esse direito de usuário determina quais usuários e grupos estão proibidos de fazer logon como um cliente de serviços de área de trabalho remota.</span><span class="sxs-lookup"><span data-stu-id="e51de-234">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="e51de-235">Somente os estados não-configuradas e bloqueados são suportados</span><span class="sxs-lookup"><span data-stu-id="e51de-235">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="e51de-236">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="e51de-236">userRightsDelegation</span></span>|[<span data-ttu-id="e51de-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-238">Esse direito de usuário determina quais usuários podem definir a configuração confiável para delegação em um objeto de usuário ou computador.</span><span class="sxs-lookup"><span data-stu-id="e51de-238">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="e51de-239">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-239">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-240">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="e51de-240">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="e51de-241">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-241">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-242">Esse direito de usuário determina quais contas podem ser utilizadas por um processo para adicionar entradas no log de segurança.</span><span class="sxs-lookup"><span data-stu-id="e51de-242">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="e51de-243">O log de segurança é usado para rastrear o acesso ao sistema não autorizado.</span><span class="sxs-lookup"><span data-stu-id="e51de-243">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="e51de-244">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-245">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="e51de-245">userRightsImpersonateClient</span></span>|[<span data-ttu-id="e51de-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-247">A atribuição desse direito de usuário a um usuário permite que programas em execução em nome desse usuário representar um cliente.</span><span class="sxs-lookup"><span data-stu-id="e51de-247">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="e51de-248">Exigir este direito de usuário para esse tipo de representação impede que um usuário não autorizado convença um cliente para se conectar a um serviço que tenha criado e, em seguida, representar o cliente, que pode elevar as permissões do usuário não autorizado para administrativas ou níveis de sistema.</span><span class="sxs-lookup"><span data-stu-id="e51de-248">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="e51de-249">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-249">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-250">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="e51de-250">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="e51de-251">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-251">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-252">Esse direito de usuário determina quais contas podem usar um processo com acesso propriedade gravação a outro processo para aumentar a prioridade de execução atribuída ao outro processo.</span><span class="sxs-lookup"><span data-stu-id="e51de-252">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="e51de-253">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-253">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-254">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="e51de-254">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="e51de-255">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-255">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-256">Esse direito de usuário determina quais usuários podem carregar e descarregar drivers de dispositivo ou outros códigos para o modo kernel dinamicamente.</span><span class="sxs-lookup"><span data-stu-id="e51de-256">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="e51de-257">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-257">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-258">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="e51de-258">userRightsLockMemory</span></span>|[<span data-ttu-id="e51de-259">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-259">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-260">Esse direito de usuário determina quais contas podem usar um processo para manter dados na memória física, o que impede o sistema de colocar os dados na memória virtual em disco.</span><span class="sxs-lookup"><span data-stu-id="e51de-260">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="e51de-261">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-261">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-262">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="e51de-262">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="e51de-263">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-263">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-264">Este direito de usuário determina quais usuários podem especificar opções para recursos individuais, como arquivos, objetos do Active Directory e chaves do registro de auditoria de acesso do objeto.</span><span class="sxs-lookup"><span data-stu-id="e51de-264">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="e51de-265">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-265">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-266">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="e51de-266">userRightsManageVolumes</span></span>|[<span data-ttu-id="e51de-267">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-267">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-268">Esse direito de usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como a desfragmentação remota.</span><span class="sxs-lookup"><span data-stu-id="e51de-268">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="e51de-269">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-269">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-270">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="e51de-270">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="e51de-271">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-271">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-272">Este direito de usuário determina quem pode modificar valores de ambiente de firmware.</span><span class="sxs-lookup"><span data-stu-id="e51de-272">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="e51de-273">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-273">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-274">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="e51de-274">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="e51de-275">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-275">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-276">Esse direito de usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves do registro ou processos pertencentes a outros usuários.</span><span class="sxs-lookup"><span data-stu-id="e51de-276">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="e51de-277">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-278">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="e51de-278">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="e51de-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-280">Esse direito de usuário determina quais usuários podem usar ferramentas de monitoramento de desempenho para monitorar o desempenho de processos do sistema.</span><span class="sxs-lookup"><span data-stu-id="e51de-280">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="e51de-281">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-282">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="e51de-282">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="e51de-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-284">Esse direito de usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede.</span><span class="sxs-lookup"><span data-stu-id="e51de-284">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="e51de-285">Uso indevido desse direito de usuário pode resultar em uma negação de serviço.</span><span class="sxs-lookup"><span data-stu-id="e51de-285">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="e51de-286">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-286">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-287">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="e51de-287">userRightsRestoreData</span></span>|[<span data-ttu-id="e51de-288">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-288">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-289">Esse direito de usuário determina quais usuários podem ignorar o arquivo, diretório, registro e outros objetos persistentes permissões ao restaurar backup de arquivos e diretórios e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto.</span><span class="sxs-lookup"><span data-stu-id="e51de-289">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="e51de-290">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-290">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-291">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="e51de-291">userRightsTakeOwnership</span></span>|[<span data-ttu-id="e51de-292">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-292">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-293">Esse direito de usuário determina quais usuários podem apropriar-se de qualquer objeto protegível no sistema, incluindo objetos do Active Directory, arquivos e pastas, impressoras, chaves do registro, processos e segmentos.</span><span class="sxs-lookup"><span data-stu-id="e51de-293">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="e51de-294">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="e51de-294">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="e51de-295">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="e51de-295">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="e51de-296">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="e51de-296">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="e51de-297">Essa configuração de segurança determina quais contas de serviço são impedidas de registrar um processo como um serviço.</span><span class="sxs-lookup"><span data-stu-id="e51de-297">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="e51de-298">Observação: Essa configuração de segurança não se aplica às contas de sistema, serviço Local ou serviço de rede.</span><span class="sxs-lookup"><span data-stu-id="e51de-298">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="e51de-299">Único estado bloqueado é suportado.</span><span class="sxs-lookup"><span data-stu-id="e51de-299">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="e51de-300">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="e51de-300">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="e51de-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-301">Boolean</span></span>|<span data-ttu-id="e51de-302">Essa configuração determina se salvar jogo do xbox está habilitado (1) ou desativada (0).</span><span class="sxs-lookup"><span data-stu-id="e51de-302">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="e51de-303">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="e51de-303">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="e51de-304">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="e51de-304">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="e51de-305">Essa configuração determina se o tipo de início do serviço de gerenciamento de acessório é Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="e51de-305">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="e51de-306">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="e51de-306">Default: Manual.</span></span> <span data-ttu-id="e51de-307">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="e51de-307">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="e51de-308">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="e51de-308">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="e51de-309">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="e51de-309">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="e51de-310">Essa configuração determina se o tipo de início do serviço do Gerenciador de autenticação Live é Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="e51de-310">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="e51de-311">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="e51de-311">Default: Manual.</span></span> <span data-ttu-id="e51de-312">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="e51de-312">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="e51de-313">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="e51de-313">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="e51de-314">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="e51de-314">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="e51de-315">Essa configuração determina se o jogo Live salvar o tipo de início do serviço é Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="e51de-315">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="e51de-316">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="e51de-316">Default: Manual.</span></span> <span data-ttu-id="e51de-317">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="e51de-317">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="e51de-318">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="e51de-318">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="e51de-319">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="e51de-319">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="e51de-320">Essa configuração determina se o tipo de início do serviço de rede é Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="e51de-320">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="e51de-321">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="e51de-321">Default: Manual.</span></span> <span data-ttu-id="e51de-322">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="e51de-322">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="e51de-323">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="e51de-323">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="e51de-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-324">Boolean</span></span>|<span data-ttu-id="e51de-325">Impedir que os usuários adicionem novas contas da Microsoft para este computador.</span><span class="sxs-lookup"><span data-stu-id="e51de-325">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="e51de-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="e51de-326">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="e51de-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-327">Boolean</span></span>|<span data-ttu-id="e51de-328">Habilite as contas locais que não são protegida para logon de locais que não seja o dispositivo físico de senha. É habilitada por padrão</span><span class="sxs-lookup"><span data-stu-id="e51de-328">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="e51de-329">localSecurityOptionsDisableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="e51de-329">localSecurityOptionsDisableAdministratorAccount</span></span>|<span data-ttu-id="e51de-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-330">Boolean</span></span>|<span data-ttu-id="e51de-331">Determina se a conta de Administrador Local está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="e51de-331">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="e51de-332">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="e51de-332">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="e51de-333">String</span><span class="sxs-lookup"><span data-stu-id="e51de-333">String</span></span>|<span data-ttu-id="e51de-334">Defina um nome de conta diferente a ser associado com o identificador de segurança (SID) da conta "Administrador".</span><span class="sxs-lookup"><span data-stu-id="e51de-334">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="e51de-335">localSecurityOptionsDisableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="e51de-335">localSecurityOptionsDisableGuestAccount</span></span>|<span data-ttu-id="e51de-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-336">Boolean</span></span>|<span data-ttu-id="e51de-337">Determina se a conta de convidado está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="e51de-337">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="e51de-338">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="e51de-338">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="e51de-339">String</span><span class="sxs-lookup"><span data-stu-id="e51de-339">String</span></span>|<span data-ttu-id="e51de-340">Defina um nome de conta diferente a ser associado com o identificador de segurança (SID) da conta "Convidado".</span><span class="sxs-lookup"><span data-stu-id="e51de-340">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="e51de-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="e51de-341">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="e51de-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-342">Boolean</span></span>|<span data-ttu-id="e51de-343">Impedir que um computador portátil sendo não encaixado sem precisar fazer logon.</span><span class="sxs-lookup"><span data-stu-id="e51de-343">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="e51de-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="e51de-344">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="e51de-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-345">Boolean</span></span>|<span data-ttu-id="e51de-346">Restringir instalando drivers de impressora como parte da conexão a uma impressora compartilhada ao grupo Administradores apenas.</span><span class="sxs-lookup"><span data-stu-id="e51de-346">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="e51de-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="e51de-347">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="e51de-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-348">Boolean</span></span>|<span data-ttu-id="e51de-349">A ativação dessa configuração permite que somente usuário conectado interativamente mídia de CD-ROM do access.</span><span class="sxs-lookup"><span data-stu-id="e51de-349">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="e51de-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="e51de-350">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="e51de-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="e51de-351">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="e51de-352">Defina quem tem permissão para formatar e ejeção mídia NTFS removível.</span><span class="sxs-lookup"><span data-stu-id="e51de-352">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="e51de-353">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="e51de-353">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="e51de-354">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="e51de-354">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="e51de-355">Int32</span><span class="sxs-lookup"><span data-stu-id="e51de-355">Int32</span></span>|<span data-ttu-id="e51de-356">Defina o máximo de minutos de inatividade na tela de login da área de trabalho interativo até o protetor de tela é executado.</span><span class="sxs-lookup"><span data-stu-id="e51de-356">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="e51de-357">Valores válidos 0 e 9999</span><span class="sxs-lookup"><span data-stu-id="e51de-357">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="e51de-358">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="e51de-358">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="e51de-359">Int32</span><span class="sxs-lookup"><span data-stu-id="e51de-359">Int32</span></span>|<span data-ttu-id="e51de-360">Defina o máximo de minutos de inatividade na tela de login da área de trabalho interativo até o protetor de tela é executado.</span><span class="sxs-lookup"><span data-stu-id="e51de-360">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="e51de-361">Valores válidos 0 e 9999</span><span class="sxs-lookup"><span data-stu-id="e51de-361">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="e51de-362">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="e51de-362">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="e51de-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-363">Boolean</span></span>|<span data-ttu-id="e51de-364">Exigir CTRL + ALT + DEL a ser pressionada para que um usuário possa fazer logon.</span><span class="sxs-lookup"><span data-stu-id="e51de-364">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="e51de-365">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="e51de-365">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="e51de-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-366">Boolean</span></span>|<span data-ttu-id="e51de-367">Não exibe o nome de usuário da última pessoa que entraram nesse dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e51de-367">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="e51de-368">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="e51de-368">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="e51de-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-369">Boolean</span></span>|<span data-ttu-id="e51de-370">Não exibe o nome de usuário da pessoa entrando para este dispositivo após credenciais são inseridas e antes de área de trabalho do dispositivo é mostrada.</span><span class="sxs-lookup"><span data-stu-id="e51de-370">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="e51de-371">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="e51de-371">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="e51de-372">String</span><span class="sxs-lookup"><span data-stu-id="e51de-372">String</span></span>|<span data-ttu-id="e51de-373">Defina o título da mensagem para usuários tentando fazer logon.</span><span class="sxs-lookup"><span data-stu-id="e51de-373">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="e51de-374">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="e51de-374">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="e51de-375">String</span><span class="sxs-lookup"><span data-stu-id="e51de-375">String</span></span>|<span data-ttu-id="e51de-376">Definir o texto da mensagem para os usuários que tentarem fazer logon.</span><span class="sxs-lookup"><span data-stu-id="e51de-376">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="e51de-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="e51de-377">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="e51de-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-378">Boolean</span></span>|<span data-ttu-id="e51de-379">Solicitações de autenticação de bloco PKU2U para este dispositivo usar identidades on-line.</span><span class="sxs-lookup"><span data-stu-id="e51de-379">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="e51de-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="e51de-380">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="e51de-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-381">Boolean</span></span>|<span data-ttu-id="e51de-382">Auxiliar da UI do boolean para entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="e51de-382">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="e51de-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="e51de-383">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="e51de-384">String</span><span class="sxs-lookup"><span data-stu-id="e51de-384">String</span></span>|<span data-ttu-id="e51de-385">Edite a cadeia de caracteres de linguagem de definição de descritor de segurança padrão para permitir ou negar a usuários e grupos para fazer chamadas remotas para o SAM.</span><span class="sxs-lookup"><span data-stu-id="e51de-385">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="e51de-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="e51de-386">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="e51de-387">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="e51de-387">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="e51de-388">Essa configuração de segurança permite que um cliente exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="e51de-388">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="e51de-389">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="e51de-389">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="e51de-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="e51de-390">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="e51de-391">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="e51de-391">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="e51de-392">Essa configuração de segurança permite que um servidor exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="e51de-392">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="e51de-393">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="e51de-393">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="e51de-394">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="e51de-394">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="e51de-395">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="e51de-395">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="e51de-396">Essa configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede.</span><span class="sxs-lookup"><span data-stu-id="e51de-396">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="e51de-397">Os possíveis valores são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="e51de-397">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="e51de-398">lanManagerWorkstationDisableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="e51de-398">lanManagerWorkstationDisableInsecureGuestLogons</span></span>|<span data-ttu-id="e51de-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-399">Boolean</span></span>|<span data-ttu-id="e51de-400">Se for habilitada, o cliente SMB permitirá que os logons de convidado inseguros.</span><span class="sxs-lookup"><span data-stu-id="e51de-400">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="e51de-401">Se não estiver configurado, o cliente SMB rejeitará logons de convidado inseguros.</span><span class="sxs-lookup"><span data-stu-id="e51de-401">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="e51de-402">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="e51de-402">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="e51de-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-403">Boolean</span></span>|<span data-ttu-id="e51de-404">Essa configuração de segurança determina se o arquivo de paginação de memória virtual será limpo quando o sistema for desligado.</span><span class="sxs-lookup"><span data-stu-id="e51de-404">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="e51de-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="e51de-405">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="e51de-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-406">Boolean</span></span>|<span data-ttu-id="e51de-407">Essa configuração de segurança determina se um computador pode ser desligado sem precisar fazer logon no Windows.</span><span class="sxs-lookup"><span data-stu-id="e51de-407">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="e51de-408">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="e51de-408">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="e51de-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-409">Boolean</span></span>|<span data-ttu-id="e51de-410">Permitir aplicativos UIAccess solicitar elevação sem usar a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="e51de-410">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="e51de-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="e51de-411">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="e51de-412">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-412">Boolean</span></span>|<span data-ttu-id="e51de-413">Virtualizar falhas de gravação de arquivo e registro a para por usuário locais</span><span class="sxs-lookup"><span data-stu-id="e51de-413">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="e51de-414">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="e51de-414">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="e51de-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-415">Boolean</span></span>|<span data-ttu-id="e51de-416">Impor a validação de caminho de certificação PKI para um determinado arquivo executável antes que ele tem permissão para executar.</span><span class="sxs-lookup"><span data-stu-id="e51de-416">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="e51de-417">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="e51de-417">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="e51de-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="e51de-418">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="e51de-419">Defina o comportamento da solicitação de elevação para administradores no modo de aprovação de administrador.</span><span class="sxs-lookup"><span data-stu-id="e51de-419">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="e51de-420">Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="e51de-420">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="e51de-421">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="e51de-421">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="e51de-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="e51de-422">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="e51de-423">Defina o comportamento da solicitação de elevação para usuários padrão.</span><span class="sxs-lookup"><span data-stu-id="e51de-423">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="e51de-424">Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="e51de-424">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="e51de-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="e51de-425">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="e51de-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-426">Boolean</span></span>|<span data-ttu-id="e51de-427">Habilite todas as solicitações de elevação ir para a área de trabalho do usuário interativa em vez de área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="e51de-427">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="e51de-428">Configurações de diretiva de comportamento de solicitação para administradores e usuários padrão são usadas.</span><span class="sxs-lookup"><span data-stu-id="e51de-428">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="e51de-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="e51de-429">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="e51de-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-430">Boolean</span></span>|<span data-ttu-id="e51de-431">Instalações de aplicativo exigir privilégios elevados vai solicitar credenciais de administrador. É habilitada por padrão</span><span class="sxs-lookup"><span data-stu-id="e51de-431">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="e51de-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="e51de-432">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="e51de-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-433">Boolean</span></span>|<span data-ttu-id="e51de-434">Permitir aplicativos UIAccess solicitar elevação sem usar a área de trabalho segura. É habilitada por padrão</span><span class="sxs-lookup"><span data-stu-id="e51de-434">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="e51de-435">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="e51de-435">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="e51de-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-436">Boolean</span></span>|<span data-ttu-id="e51de-437">Define se a conta de administrador interna usa o modo de aprovação de administrador ou executa todos os aplicativos com privilégios de administrador completo. É habilitada por padrão</span><span class="sxs-lookup"><span data-stu-id="e51de-437">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="e51de-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="e51de-438">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="e51de-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-439">Boolean</span></span>|<span data-ttu-id="e51de-440">Defina se o modo de aprovação de administrador e todas as configurações de diretiva UAC estão habilitadas, é habilitada por padrão</span><span class="sxs-lookup"><span data-stu-id="e51de-440">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="e51de-441">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="e51de-441">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="e51de-442">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="e51de-442">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="e51de-443">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="e51de-443">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="e51de-444">Se não estiver configurado, username, domínio e nome de exibição do usuário são mostrados.</span><span class="sxs-lookup"><span data-stu-id="e51de-444">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="e51de-445">Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="e51de-445">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="e51de-446">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="e51de-446">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="e51de-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="e51de-447">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="e51de-448">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="e51de-448">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="e51de-449">Se não estiver configurado, username, domínio e nome de exibição do usuário são mostrados.</span><span class="sxs-lookup"><span data-stu-id="e51de-449">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="e51de-450">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="e51de-450">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="e51de-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="e51de-451">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="e51de-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-452">Boolean</span></span>|<span data-ttu-id="e51de-453">Essa configuração determina se o cliente SMB tentará negociar a assinatura de pacotes SMB.</span><span class="sxs-lookup"><span data-stu-id="e51de-453">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="e51de-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="e51de-454">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="e51de-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-455">Boolean</span></span>|<span data-ttu-id="e51de-456">Essa configuração de segurança determina se a assinatura de pacotes é exigida pelo componente cliente do SMB.</span><span class="sxs-lookup"><span data-stu-id="e51de-456">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="e51de-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="e51de-457">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="e51de-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-458">Boolean</span></span>|<span data-ttu-id="e51de-459">Se essa configuração de segurança estiver habilitada, o redirecionador de bloco de mensagens do servidor (SMB) é permitido para enviar senhas de texto sem formatação para servidores SMB não Microsoft que não têm suporte para criptografia de senha durante a autenticação.</span><span class="sxs-lookup"><span data-stu-id="e51de-459">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="e51de-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="e51de-460">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="e51de-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-461">Boolean</span></span>|<span data-ttu-id="e51de-462">Essa configuração de segurança determina se a assinatura de pacotes é exigida pelo componente de servidor SMB.</span><span class="sxs-lookup"><span data-stu-id="e51de-462">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="e51de-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="e51de-463">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="e51de-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-464">Boolean</span></span>|<span data-ttu-id="e51de-465">Essa configuração de segurança determina se o servidor SMB irá negociar assinatura com clientes que solicitarem de pacotes SMB.</span><span class="sxs-lookup"><span data-stu-id="e51de-465">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="e51de-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="e51de-466">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="e51de-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-467">Boolean</span></span>|<span data-ttu-id="e51de-468">Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e pipes para as configurações de pipes nomeados que podem ser acessados anonimamente e compartilhamentos que podem ser acessados anonimamente</span><span class="sxs-lookup"><span data-stu-id="e51de-468">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="e51de-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="e51de-469">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="e51de-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-470">Boolean</span></span>|<span data-ttu-id="e51de-471">Essa configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas ao computador.</span><span class="sxs-lookup"><span data-stu-id="e51de-471">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="e51de-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="e51de-472">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="e51de-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-473">Boolean</span></span>|<span data-ttu-id="e51de-474">Essa configuração de segurança determina se deve ser permite que usuários anônimos executem determinadas atividades, como enumeração de nomes de contas de domínio e compartilhamentos de rede.</span><span class="sxs-lookup"><span data-stu-id="e51de-474">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="e51de-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="e51de-475">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="e51de-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-476">Boolean</span></span>|<span data-ttu-id="e51de-477">Essa configuração de segurança determina se, na próxima alteração de senha, o valor de hash do LM (LAN Manager) para a nova senha é armazenado.</span><span class="sxs-lookup"><span data-stu-id="e51de-477">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="e51de-478">Ele não é armazenado por padrão.</span><span class="sxs-lookup"><span data-stu-id="e51de-478">It’s not stored by default.</span></span>|
|<span data-ttu-id="e51de-479">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="e51de-479">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="e51de-480">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="e51de-480">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="e51de-481">Essa configuração de segurança determina o que acontece quando o cartão inteligente de um usuário conectado é removido do leitor de cartão inteligente.</span><span class="sxs-lookup"><span data-stu-id="e51de-481">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="e51de-482">Os valores possíveis são: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="e51de-482">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="e51de-483">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="e51de-483">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="e51de-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-484">Boolean</span></span>|<span data-ttu-id="e51de-485">Usada para desabilitar a exibição da área de proteção de aplicativo e de navegador.</span><span class="sxs-lookup"><span data-stu-id="e51de-485">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="e51de-486">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="e51de-486">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="e51de-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-487">Boolean</span></span>|<span data-ttu-id="e51de-488">Usada para desabilitar a exibição da área de opções da família.</span><span class="sxs-lookup"><span data-stu-id="e51de-488">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="e51de-489">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="e51de-489">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="e51de-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-490">Boolean</span></span>|<span data-ttu-id="e51de-491">Usada para desabilitar a exibição da área de integridade e desempenho do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e51de-491">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="e51de-492">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="e51de-492">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="e51de-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-493">Boolean</span></span>|<span data-ttu-id="e51de-494">Usada para desabilitar a exibição da área de proteção de rede e de firewall.</span><span class="sxs-lookup"><span data-stu-id="e51de-494">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="e51de-495">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="e51de-495">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="e51de-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-496">Boolean</span></span>|<span data-ttu-id="e51de-497">Usada para desabilitar a exibição da área de proteção de vírus e ameaças.</span><span class="sxs-lookup"><span data-stu-id="e51de-497">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="e51de-498">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="e51de-498">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="e51de-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-499">Boolean</span></span>|<span data-ttu-id="e51de-500">Usada para desabilitar a exibição da área de proteção de conta.</span><span class="sxs-lookup"><span data-stu-id="e51de-500">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="e51de-501">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="e51de-501">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="e51de-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-502">Boolean</span></span>|<span data-ttu-id="e51de-503">Usada para desabilitar a exibição da área de proteção de hardware.</span><span class="sxs-lookup"><span data-stu-id="e51de-503">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="e51de-504">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="e51de-504">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="e51de-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-505">Boolean</span></span>|<span data-ttu-id="e51de-506">Usada para desabilitar a exibição da área de proteção do ransomware.</span><span class="sxs-lookup"><span data-stu-id="e51de-506">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="e51de-507">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="e51de-507">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="e51de-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-508">Boolean</span></span>|<span data-ttu-id="e51de-509">Usada para desabilitar a exibição da área de inicialização segura em segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e51de-509">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="e51de-510">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="e51de-510">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="e51de-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-511">Boolean</span></span>|<span data-ttu-id="e51de-512">Usada para desabilitar a exibição do processo de segurança, a solução de problemas em segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e51de-512">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="e51de-513">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="e51de-513">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="e51de-514">String</span><span class="sxs-lookup"><span data-stu-id="e51de-514">String</span></span>|<span data-ttu-id="e51de-515">O nome de empresa que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="e51de-515">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="e51de-516">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="e51de-516">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="e51de-517">String</span><span class="sxs-lookup"><span data-stu-id="e51de-517">String</span></span>|<span data-ttu-id="e51de-518">O endereço de email que será exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="e51de-518">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="e51de-519">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="e51de-519">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="e51de-520">String</span><span class="sxs-lookup"><span data-stu-id="e51de-520">String</span></span>|<span data-ttu-id="e51de-521">O número de telefone ou o ID do Skype que será exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="e51de-521">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="e51de-522">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="e51de-522">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="e51de-523">String</span><span class="sxs-lookup"><span data-stu-id="e51de-523">String</span></span>|<span data-ttu-id="e51de-524">Portal da Ajuda URL isso será exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="e51de-524">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="e51de-525">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="e51de-525">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="e51de-526">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="e51de-526">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="e51de-527">Notificações para mostrar de exibido áreas de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e51de-527">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="e51de-528">Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="e51de-528">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="e51de-529">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="e51de-529">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="e51de-530">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="e51de-530">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="e51de-531">Configurar onde exibir contato de TI informações aos usuários finais.</span><span class="sxs-lookup"><span data-stu-id="e51de-531">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="e51de-532">Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="e51de-532">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="e51de-533">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="e51de-533">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="e51de-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-534">Boolean</span></span>|<span data-ttu-id="e51de-535">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="e51de-535">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="e51de-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="e51de-536">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="e51de-537">Int32</span><span class="sxs-lookup"><span data-stu-id="e51de-537">Int32</span></span>|<span data-ttu-id="e51de-538">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="e51de-538">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="e51de-539">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="e51de-539">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="e51de-540">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="e51de-540">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="e51de-541">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="e51de-541">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="e51de-542">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="e51de-542">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="e51de-543">Selecione a chave pré compartilhada codificação a ser usada.</span><span class="sxs-lookup"><span data-stu-id="e51de-543">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="e51de-544">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="e51de-544">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="e51de-545">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="e51de-545">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="e51de-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-546">Boolean</span></span>|<span data-ttu-id="e51de-547">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="e51de-547">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="e51de-548">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="e51de-548">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="e51de-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-549">Boolean</span></span>|<span data-ttu-id="e51de-550">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="e51de-550">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="e51de-551">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="e51de-551">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="e51de-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-552">Boolean</span></span>|<span data-ttu-id="e51de-553">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="e51de-553">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="e51de-554">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="e51de-554">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="e51de-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-555">Boolean</span></span>|<span data-ttu-id="e51de-556">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="e51de-556">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="e51de-557">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="e51de-557">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="e51de-558">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="e51de-558">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="e51de-559">Especifique como a lista de revogação de certificado deve ser impostas.</span><span class="sxs-lookup"><span data-stu-id="e51de-559">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="e51de-560">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="e51de-560">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="e51de-561">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="e51de-561">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="e51de-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-562">Boolean</span></span>|<span data-ttu-id="e51de-563">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="e51de-563">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="e51de-564">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="e51de-564">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="e51de-565">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="e51de-565">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="e51de-566">Configura como queueing pacotes deve ser aplicada no cenário túnel gateway.</span><span class="sxs-lookup"><span data-stu-id="e51de-566">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="e51de-567">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="e51de-567">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="e51de-568">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="e51de-568">firewallProfileDomain</span></span>|[<span data-ttu-id="e51de-569">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="e51de-569">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="e51de-570">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="e51de-570">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="e51de-571">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="e51de-571">firewallProfilePublic</span></span>|[<span data-ttu-id="e51de-572">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="e51de-572">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="e51de-573">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="e51de-573">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="e51de-574">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="e51de-574">firewallProfilePrivate</span></span>|[<span data-ttu-id="e51de-575">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="e51de-575">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="e51de-576">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="e51de-576">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="e51de-577">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="e51de-577">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="e51de-578">String collection</span><span class="sxs-lookup"><span data-stu-id="e51de-578">String collection</span></span>|<span data-ttu-id="e51de-579">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="e51de-579">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="e51de-580">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-580">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="e51de-581">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="e51de-581">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="e51de-582">Valor que indica o comportamento dos aplicativos do Office injeção aos outros processos.</span><span class="sxs-lookup"><span data-stu-id="e51de-582">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="e51de-583">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-583">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-584">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="e51de-584">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="e51de-585">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-585">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-586">Valor que indica o comportamento dos aplicativos do Office injeção aos outros processos.</span><span class="sxs-lookup"><span data-stu-id="e51de-586">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="e51de-587">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-587">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="e51de-588">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="e51de-589">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="e51de-589">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="e51de-590">Valor que indica o comportamento de macros aplicativos/Office criando ou launching conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="e51de-590">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="e51de-591">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-591">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="e51de-592">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="e51de-593">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-593">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-594">Valor que indica o comportamento de macros aplicativos/Office criando ou launching conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="e51de-594">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="e51de-595">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-595">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-596">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="e51de-596">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="e51de-597">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="e51de-597">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="e51de-598">Valor que indica o comportamento do aplicativo Office launching processos filho.</span><span class="sxs-lookup"><span data-stu-id="e51de-598">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="e51de-599">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-599">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-600">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="e51de-600">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="e51de-601">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-601">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-602">Valor que indica o comportamento do aplicativo Office launching processos filho.</span><span class="sxs-lookup"><span data-stu-id="e51de-602">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="e51de-603">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-603">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-604">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="e51de-604">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="e51de-605">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="e51de-605">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="e51de-606">O valor que indica que o comportamento do Win32 importa do código de Macro no Office.</span><span class="sxs-lookup"><span data-stu-id="e51de-606">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="e51de-607">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-607">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-608">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="e51de-608">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="e51de-609">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-609">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-610">O valor que indica que o comportamento do Win32 importa do código de Macro no Office.</span><span class="sxs-lookup"><span data-stu-id="e51de-610">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="e51de-611">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-611">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-612">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="e51de-612">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="e51de-613">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="e51de-613">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="e51de-614">Valor que indica o comportamento do código de js/vbs/ps/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="e51de-614">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="e51de-615">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-615">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-616">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="e51de-616">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="e51de-617">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-617">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-618">Valor que indica o comportamento do código de js/vbs/ps/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="e51de-618">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="e51de-619">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-619">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-620">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="e51de-620">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="e51de-621">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="e51de-621">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="e51de-622">Valor que indica o comportamento do js/vbs executá-lo carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="e51de-622">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="e51de-623">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-623">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-624">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="e51de-624">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="e51de-625">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-625">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-626">Valor que indica o comportamento do js/vbs executá-lo carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="e51de-626">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="e51de-627">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-627">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-628">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="e51de-628">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="e51de-629">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-629">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-630">Valor que indica se a credencial roubar do subsistema de autoridade de segurança local do Windows será permitida.</span><span class="sxs-lookup"><span data-stu-id="e51de-630">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="e51de-631">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-631">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-632">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="e51de-632">defenderProcessCreationType</span></span>|[<span data-ttu-id="e51de-633">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="e51de-633">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="e51de-634">O valor de resposta indica a criações de processo provenientes de comandos PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="e51de-634">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="e51de-635">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-635">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-636">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="e51de-636">defenderProcessCreation</span></span>|[<span data-ttu-id="e51de-637">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-637">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-638">O valor de resposta indica a criações de processo provenientes de comandos PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="e51de-638">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="e51de-639">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-639">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-640">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="e51de-640">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="e51de-641">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="e51de-641">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="e51de-642">Valor que indica a resposta para processos assinados e não confiáveis que executam o USB.</span><span class="sxs-lookup"><span data-stu-id="e51de-642">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="e51de-643">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-643">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-644">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="e51de-644">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="e51de-645">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-645">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-646">Valor que indica a resposta para processos assinados e não confiáveis que executam o USB.</span><span class="sxs-lookup"><span data-stu-id="e51de-646">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="e51de-647">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-647">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-648">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="e51de-648">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="e51de-649">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="e51de-649">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="e51de-650">Valor que indica a resposta para executáveis que não atendem a uma chamadas, idade ou lista de confiável critérios.</span><span class="sxs-lookup"><span data-stu-id="e51de-650">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="e51de-651">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-651">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-652">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="e51de-652">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="e51de-653">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-653">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-654">Valor que indica a resposta para executáveis que não atendem a uma chamadas, idade ou lista de confiável critérios.</span><span class="sxs-lookup"><span data-stu-id="e51de-654">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="e51de-655">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-655">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-656">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="e51de-656">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="e51de-657">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="e51de-657">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="e51de-658">Valor que indica se a execução de conteúdo executável (exe, dll, ps, js, vbs, etc.) deve ser retirada da email (email/webmail-cliente).</span><span class="sxs-lookup"><span data-stu-id="e51de-658">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="e51de-659">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-659">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-660">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="e51de-660">defenderEmailContentExecution</span></span>|[<span data-ttu-id="e51de-661">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-661">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-662">Valor que indica se a execução de conteúdo executável (exe, dll, ps, js, vbs, etc.) deve ser retirada da email (email/webmail-cliente).</span><span class="sxs-lookup"><span data-stu-id="e51de-662">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="e51de-663">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-663">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-664">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-664">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="e51de-665">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-665">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-666">Valor que indica o uso de proteção avançada contra ransomeware.</span><span class="sxs-lookup"><span data-stu-id="e51de-666">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="e51de-667">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-667">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-668">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="e51de-668">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="e51de-669">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-669">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="e51de-670">Valor que indica o comportamento de pastas protegidas.</span><span class="sxs-lookup"><span data-stu-id="e51de-670">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="e51de-671">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="e51de-671">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="e51de-672">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="e51de-672">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="e51de-673">String collection</span><span class="sxs-lookup"><span data-stu-id="e51de-673">String collection</span></span>|<span data-ttu-id="e51de-674">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="e51de-674">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="e51de-675">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="e51de-675">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="e51de-676">String collection</span><span class="sxs-lookup"><span data-stu-id="e51de-676">String collection</span></span>|<span data-ttu-id="e51de-677">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="e51de-677">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="e51de-678">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-678">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="e51de-679">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="e51de-679">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="e51de-680">Valor que indica o comportamento do NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="e51de-680">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="e51de-681">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="e51de-681">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="e51de-682">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="e51de-682">defenderExploitProtectionXml</span></span>|<span data-ttu-id="e51de-683">Binária</span><span class="sxs-lookup"><span data-stu-id="e51de-683">Binary</span></span>|<span data-ttu-id="e51de-684">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="e51de-684">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="e51de-685">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="e51de-685">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="e51de-686">String</span><span class="sxs-lookup"><span data-stu-id="e51de-686">String</span></span>|<span data-ttu-id="e51de-687">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="e51de-687">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="e51de-688">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="e51de-688">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="e51de-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-689">Boolean</span></span>|<span data-ttu-id="e51de-690">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="e51de-690">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="e51de-691">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="e51de-691">appLockerApplicationControl</span></span>|[<span data-ttu-id="e51de-692">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="e51de-692">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="e51de-693">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e51de-693">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="e51de-694">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="e51de-694">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="e51de-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="e51de-695">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="e51de-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="e51de-696">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="e51de-697">Ative o protetor de credencial quando o nível de segurança de plataforma com inicialização seguro e virtualização com base em segurança estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="e51de-697">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="e51de-698">Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="e51de-698">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="e51de-699">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="e51de-699">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="e51de-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-700">Boolean</span></span>|<span data-ttu-id="e51de-701">Ativa as teclas de virtualização com base em Security(VBS).</span><span class="sxs-lookup"><span data-stu-id="e51de-701">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="e51de-702">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="e51de-702">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="e51de-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-703">Boolean</span></span>|<span data-ttu-id="e51de-704">Especifica se o nível de segurança de plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="e51de-704">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="e51de-705">deviceGuardLaunchSystemGuard</span><span class="sxs-lookup"><span data-stu-id="e51de-705">deviceGuardLaunchSystemGuard</span></span>|<span data-ttu-id="e51de-706">[habilitação] (.. /Resources/Intune-Shared-Enablement</span><span class="sxs-lookup"><span data-stu-id="e51de-706">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="e51de-707">.MD)</span><span class="sxs-lookup"><span data-stu-id="e51de-707">.md)</span></span>|<span data-ttu-id="e51de-708">Permite que o administrador de TI configurar o lançamento do protetor de sistema.</span><span class="sxs-lookup"><span data-stu-id="e51de-708">Allows the IT admin to configure the launch of System Guard.</span></span> <span data-ttu-id="e51de-709">Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="e51de-709">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="e51de-710">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="e51de-710">smartScreenEnableInShell</span></span>|<span data-ttu-id="e51de-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-711">Boolean</span></span>|<span data-ttu-id="e51de-712">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="e51de-712">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="e51de-713">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="e51de-713">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="e51de-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-714">Boolean</span></span>|<span data-ttu-id="e51de-715">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="e51de-715">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="e51de-716">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="e51de-716">applicationGuardEnabled</span></span>|<span data-ttu-id="e51de-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-717">Boolean</span></span>|<span data-ttu-id="e51de-718">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="e51de-718">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="e51de-719">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="e51de-719">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="e51de-720">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="e51de-720">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="e51de-721">Habilite o protetor de aplicativo do Windows Defender para versões mais recentes do Windows.</span><span class="sxs-lookup"><span data-stu-id="e51de-721">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="e51de-722">Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="e51de-722">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="e51de-723">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="e51de-723">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="e51de-724">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="e51de-724">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="e51de-725">Área de transferência de bloqueio para um arquivo de imagem de transferência, arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="e51de-725">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="e51de-726">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="e51de-726">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="e51de-727">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="e51de-727">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="e51de-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-728">Boolean</span></span>|<span data-ttu-id="e51de-729">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="e51de-729">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="e51de-730">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="e51de-730">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="e51de-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-731">Boolean</span></span>|<span data-ttu-id="e51de-732">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="e51de-732">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="e51de-733">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="e51de-733">applicationGuardForceAuditing</span></span>|<span data-ttu-id="e51de-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-734">Boolean</span></span>|<span data-ttu-id="e51de-735">A auditoria forçada manterá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)
</span><span class="sxs-lookup"><span data-stu-id="e51de-735">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="e51de-736">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="e51de-736">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="e51de-737">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="e51de-737">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="e51de-738">Impedir a área de transferência de compartilhar dados do Host para o Contêiner, do Contêiner para o Host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="e51de-738">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="e51de-739">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="e51de-739">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="e51de-740">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="e51de-740">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="e51de-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-741">Boolean</span></span>|<span data-ttu-id="e51de-742">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="e51de-742">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="e51de-743">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="e51de-743">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="e51de-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-744">Boolean</span></span>|<span data-ttu-id="e51de-745">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="e51de-745">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="e51de-746">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="e51de-746">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="e51de-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-747">Boolean</span></span>|<span data-ttu-id="e51de-748">Permitir a impressão em Impressoras Locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="e51de-748">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="e51de-749">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="e51de-749">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="e51de-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-750">Boolean</span></span>|<span data-ttu-id="e51de-751">Permitir a impressão em Impressoras da Rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="e51de-751">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="e51de-752">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="e51de-752">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="e51de-753">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-753">Boolean</span></span>|<span data-ttu-id="e51de-754">Permitir guard aplicativo usar GPU virtual</span><span class="sxs-lookup"><span data-stu-id="e51de-754">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="e51de-755">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="e51de-755">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="e51de-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-756">Boolean</span></span>|<span data-ttu-id="e51de-757">Permitir que os usuários baixem arquivos de borda no contêiner do protetor de aplicativo e salvá-los no host do sistema de arquivos</span><span class="sxs-lookup"><span data-stu-id="e51de-757">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="e51de-758">bitLockerAllowStandardUserEncryption</span><span class="sxs-lookup"><span data-stu-id="e51de-758">bitLockerAllowStandardUserEncryption</span></span>|<span data-ttu-id="e51de-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-759">Boolean</span></span>|<span data-ttu-id="e51de-760">Permite que o administrador permitir que usuários padrão habilitar o encrpytion durante ingressar do Windows Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e51de-760">Allows the admin to allow standard users to enable encrpytion during Azure AD Join.</span></span>|
|<span data-ttu-id="e51de-761">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="e51de-761">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="e51de-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-762">Boolean</span></span>|<span data-ttu-id="e51de-763">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="e51de-763">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="e51de-764">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="e51de-764">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="e51de-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-765">Boolean</span></span>|<span data-ttu-id="e51de-766">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="e51de-766">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="e51de-767">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="e51de-767">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="e51de-768">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="e51de-768">bitLockerEncryptDevice</span></span>|<span data-ttu-id="e51de-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="e51de-769">Boolean</span></span>|<span data-ttu-id="e51de-770">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="e51de-770">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="e51de-771">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="e51de-771">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="e51de-772">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="e51de-772">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="e51de-773">Política de unidade de disco BitLocker sistema.</span><span class="sxs-lookup"><span data-stu-id="e51de-773">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="e51de-774">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="e51de-774">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="e51de-775">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="e51de-775">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="e51de-776">O BitLocker fixa direcionar a política.</span><span class="sxs-lookup"><span data-stu-id="e51de-776">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="e51de-777">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="e51de-777">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="e51de-778">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="e51de-778">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="e51de-779">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="e51de-779">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="e51de-780">Resposta</span><span class="sxs-lookup"><span data-stu-id="e51de-780">Response</span></span>
<span data-ttu-id="e51de-781">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e51de-781">If successful, this method returns a `200 OK` response code and an updated [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e51de-782">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e51de-782">Example</span></span>

### <a name="request"></a><span data-ttu-id="e51de-783">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e51de-783">Request</span></span>
<span data-ttu-id="e51de-784">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e51de-784">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 26475

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
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
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
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
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

### <a name="response"></a><span data-ttu-id="e51de-785">Resposta</span><span class="sxs-lookup"><span data-stu-id="e51de-785">Response</span></span>
<span data-ttu-id="e51de-p196">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e51de-p196">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 26647

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
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
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
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "block",
  "defenderOfficeAppsOtherProcessInjection": "enable",
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




