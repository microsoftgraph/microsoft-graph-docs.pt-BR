---
title: Criar windows10EndpointProtectionConfiguration
description: Criar um novo objeto windows10EndpointProtectionConfiguration.
author: tfitzmac
ms.openlocfilehash: 121beda2aa8d8f9da4d652f608511f8ee72364b9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360988"
---
# <a name="create-windows10endpointprotectionconfiguration"></a><span data-ttu-id="1952d-103">Criar windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="1952d-103">Create windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="1952d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1952d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1952d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1952d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1952d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1952d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1952d-107">Criar um novo objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1952d-107">Create a new [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1952d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1952d-108">Prerequisites</span></span>
<span data-ttu-id="1952d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1952d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1952d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1952d-111">Permission type</span></span>|<span data-ttu-id="1952d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1952d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1952d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1952d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1952d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1952d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1952d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1952d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1952d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1952d-116">Not supported.</span></span>|
|<span data-ttu-id="1952d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1952d-117">Application</span></span>|<span data-ttu-id="1952d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1952d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1952d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1952d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1952d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1952d-120">Request headers</span></span>
|<span data-ttu-id="1952d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1952d-121">Header</span></span>|<span data-ttu-id="1952d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1952d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1952d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1952d-123">Authorization</span></span>|<span data-ttu-id="1952d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1952d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1952d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1952d-125">Accept</span></span>|<span data-ttu-id="1952d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1952d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1952d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1952d-127">Request body</span></span>
<span data-ttu-id="1952d-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1952d-128">In the request body, supply a JSON representation for the windows10EndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="1952d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10EndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1952d-129">The following table shows the properties that are required when you create the windows10EndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="1952d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1952d-130">Property</span></span>|<span data-ttu-id="1952d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1952d-131">Type</span></span>|<span data-ttu-id="1952d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1952d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1952d-133">id</span><span class="sxs-lookup"><span data-stu-id="1952d-133">id</span></span>|<span data-ttu-id="1952d-134">String</span><span class="sxs-lookup"><span data-stu-id="1952d-134">String</span></span>|<span data-ttu-id="1952d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1952d-135">Key of the entity.</span></span> <span data-ttu-id="1952d-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1952d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1952d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1952d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1952d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1952d-138">DateTimeOffset</span></span>|<span data-ttu-id="1952d-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1952d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1952d-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1952d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1952d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1952d-141">roleScopeTagIds</span></span>|<span data-ttu-id="1952d-142">String collection</span><span class="sxs-lookup"><span data-stu-id="1952d-142">String collection</span></span>|<span data-ttu-id="1952d-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="1952d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1952d-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1952d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1952d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1952d-145">supportsScopeTags</span></span>|<span data-ttu-id="1952d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-146">Boolean</span></span>|<span data-ttu-id="1952d-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1952d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1952d-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1952d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1952d-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="1952d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1952d-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1952d-150">This property is read-only.</span></span> <span data-ttu-id="1952d-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1952d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1952d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1952d-152">createdDateTime</span></span>|<span data-ttu-id="1952d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1952d-153">DateTimeOffset</span></span>|<span data-ttu-id="1952d-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1952d-154">DateTime the object was created.</span></span> <span data-ttu-id="1952d-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1952d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1952d-156">description</span><span class="sxs-lookup"><span data-stu-id="1952d-156">description</span></span>|<span data-ttu-id="1952d-157">String</span><span class="sxs-lookup"><span data-stu-id="1952d-157">String</span></span>|<span data-ttu-id="1952d-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1952d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1952d-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1952d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1952d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1952d-160">displayName</span></span>|<span data-ttu-id="1952d-161">String</span><span class="sxs-lookup"><span data-stu-id="1952d-161">String</span></span>|<span data-ttu-id="1952d-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1952d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1952d-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1952d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1952d-164">version</span><span class="sxs-lookup"><span data-stu-id="1952d-164">version</span></span>|<span data-ttu-id="1952d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1952d-165">Int32</span></span>|<span data-ttu-id="1952d-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1952d-166">Version of the device configuration.</span></span> <span data-ttu-id="1952d-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1952d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1952d-168">userRightsAccessCredentialManagerAsTrustedCaller</span><span class="sxs-lookup"><span data-stu-id="1952d-168">userRightsAccessCredentialManagerAsTrustedCaller</span></span>|[<span data-ttu-id="1952d-169">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-169">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-170">Esse direito de usuário é usado pelo Gerenciador de credenciais durante Backup/restauração.</span><span class="sxs-lookup"><span data-stu-id="1952d-170">This user right is used by Credential Manager during Backup/Restore.</span></span> <span data-ttu-id="1952d-171">As credenciais dos usuários salvas podem ficar comprometidas se esse privilégio é fornecido a outras entidades.</span><span class="sxs-lookup"><span data-stu-id="1952d-171">Users' saved credentials might be compromised if this privilege is given to other entities.</span></span> <span data-ttu-id="1952d-172">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="1952d-172">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1952d-173">userRightsAllowAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="1952d-173">userRightsAllowAccessFromNetwork</span></span>|[<span data-ttu-id="1952d-174">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-174">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-175">Este direito de usuário determina quais usuários e grupos têm permissão para se conectar ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="1952d-175">This user right determines which users and groups are allowed to connect to the computer over the network.</span></span> <span data-ttu-id="1952d-176">Há suporte para o estado permitidos.</span><span class="sxs-lookup"><span data-stu-id="1952d-176">State Allowed is supported.</span></span>|
|<span data-ttu-id="1952d-177">userRightsBlockAccessFromNetwork</span><span class="sxs-lookup"><span data-stu-id="1952d-177">userRightsBlockAccessFromNetwork</span></span>|[<span data-ttu-id="1952d-178">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-178">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-179">Esse direito de usuário determina quais usuários e grupos estão bloco de conectar-se ao computador pela rede.</span><span class="sxs-lookup"><span data-stu-id="1952d-179">This user right determines which users and groups are block from connecting to the computer over the network.</span></span> <span data-ttu-id="1952d-180">Bloco de controle de sessão é suportado.</span><span class="sxs-lookup"><span data-stu-id="1952d-180">State Block is supported.</span></span>|
|<span data-ttu-id="1952d-181">userRightsActAsPartOfTheOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1952d-181">userRightsActAsPartOfTheOperatingSystem</span></span>|[<span data-ttu-id="1952d-182">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-182">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-183">Esse direito de usuário permite que um processo representar qualquer usuário sem autenticação.</span><span class="sxs-lookup"><span data-stu-id="1952d-183">This user right allows a process to impersonate any user without authentication.</span></span> <span data-ttu-id="1952d-184">O processo, portanto, pode ter acesso aos mesmos recursos locais que esse usuário.</span><span class="sxs-lookup"><span data-stu-id="1952d-184">The process can therefore gain access to the same local resources as that user.</span></span> <span data-ttu-id="1952d-185">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="1952d-185">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1952d-186">userRightsLocalLogOn</span><span class="sxs-lookup"><span data-stu-id="1952d-186">userRightsLocalLogOn</span></span>|[<span data-ttu-id="1952d-187">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-187">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-188">Esse direito de usuário determina quais usuários podem fazer logon no computador.</span><span class="sxs-lookup"><span data-stu-id="1952d-188">This user right determines which users can log on to the computer.</span></span> <span data-ttu-id="1952d-189">Estados de não-configuradas, permitidos e bloqueados são suportados</span><span class="sxs-lookup"><span data-stu-id="1952d-189">States NotConfigured, Allowed and Blocked are all supported</span></span> |
|<span data-ttu-id="1952d-190">userRightsBackupData</span><span class="sxs-lookup"><span data-stu-id="1952d-190">userRightsBackupData</span></span>|[<span data-ttu-id="1952d-191">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-191">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-192">Esse direito de usuário determina quais usuários podem ignorar arquivo, diretório, registro e outras permissões de objetos persistentes ao fazer backup de arquivos e diretórios.</span><span class="sxs-lookup"><span data-stu-id="1952d-192">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when backing up files and directories.</span></span> <span data-ttu-id="1952d-193">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="1952d-193">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1952d-194">userRightsChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="1952d-194">userRightsChangeSystemTime</span></span>|[<span data-ttu-id="1952d-195">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-195">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-196">Esse direito de usuário determina quais usuários e grupos podem alterar a hora e data do relógio interno do computador.</span><span class="sxs-lookup"><span data-stu-id="1952d-196">This user right determines which users and groups can change the time and date on the internal clock of the computer.</span></span> <span data-ttu-id="1952d-197">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="1952d-197">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1952d-198">userRightsCreateGlobalObjects</span><span class="sxs-lookup"><span data-stu-id="1952d-198">userRightsCreateGlobalObjects</span></span>|[<span data-ttu-id="1952d-199">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-199">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-200">Essa configuração determina se os usuários podem criar objetos globais que estão disponíveis para todas as sessões.</span><span class="sxs-lookup"><span data-stu-id="1952d-200">This security setting determines whether users can create global objects that are available to all sessions.</span></span> <span data-ttu-id="1952d-201">Usuários que podem criar objetos globais poderá afetar os processos executados em sessões de outros usuários, que pode levar à corrupção de dados ou falha do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1952d-201">Users who can create global objects could affect processes that run under other users' sessions, which could lead to application failure or data corruption.</span></span> <span data-ttu-id="1952d-202">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="1952d-202">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1952d-203">userRightsCreatePageFile</span><span class="sxs-lookup"><span data-stu-id="1952d-203">userRightsCreatePageFile</span></span>|[<span data-ttu-id="1952d-204">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-204">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-205">Este direito de usuário determina quais usuários e grupos podem chamar uma API interna para criar e alterar o tamanho de um arquivo de paginação.</span><span class="sxs-lookup"><span data-stu-id="1952d-205">This user right determines which users and groups can call an internal API to create and change the size of a page file.</span></span> <span data-ttu-id="1952d-206">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="1952d-206">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1952d-207">userRightsCreatePermanentSharedObjects</span><span class="sxs-lookup"><span data-stu-id="1952d-207">userRightsCreatePermanentSharedObjects</span></span>|[<span data-ttu-id="1952d-208">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-208">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-209">Esse direito de usuário determina quais contas podem ser usadas por processos para criar um objeto de diretório usando o objeto Gerenciador.</span><span class="sxs-lookup"><span data-stu-id="1952d-209">This user right determines which accounts can be used by processes to create a directory object using the object manager.</span></span> <span data-ttu-id="1952d-210">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="1952d-210">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1952d-211">userRightsCreateSymbolicLinks</span><span class="sxs-lookup"><span data-stu-id="1952d-211">userRightsCreateSymbolicLinks</span></span>|[<span data-ttu-id="1952d-212">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-212">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-213">Esse direito de usuário determina se o usuário pode criar um link simbólico do computador ao qual ele esteja conectados.</span><span class="sxs-lookup"><span data-stu-id="1952d-213">This user right determines if the user can create a symbolic link from the computer to which they are logged on.</span></span> <span data-ttu-id="1952d-214">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="1952d-214">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1952d-215">userRightsCreateToken</span><span class="sxs-lookup"><span data-stu-id="1952d-215">userRightsCreateToken</span></span>|[<span data-ttu-id="1952d-216">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-216">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-217">Este direito de usuário determina quais usuários/grupos podem ser usados por processos para criar um token que pode ser usado para obter acesso a qualquer recurso local quando o processo usa uma API interna para criar um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="1952d-217">This user right determines which users/groups can be used by processes to create a token that can then be used to get access to any local resources when the process uses an internal API to create an access token.</span></span> <span data-ttu-id="1952d-218">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="1952d-218">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1952d-219">userRightsDebugPrograms</span><span class="sxs-lookup"><span data-stu-id="1952d-219">userRightsDebugPrograms</span></span>|[<span data-ttu-id="1952d-220">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-220">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-221">Esse direito de usuário determina quais usuários podem anexar um depurador a qualquer processo ou ao kernel.</span><span class="sxs-lookup"><span data-stu-id="1952d-221">This user right determines which users can attach a debugger to any process or to the kernel.</span></span> <span data-ttu-id="1952d-222">Somente os estados não-configuradas e permitidos são suportados</span><span class="sxs-lookup"><span data-stu-id="1952d-222">Only states NotConfigured and Allowed are supported</span></span>|
|<span data-ttu-id="1952d-223">userRightsRemoteDesktopServicesLogOn</span><span class="sxs-lookup"><span data-stu-id="1952d-223">userRightsRemoteDesktopServicesLogOn</span></span>|[<span data-ttu-id="1952d-224">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-224">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-225">Esse direito de usuário determina quais usuários e grupos estão proibidos de fazer logon como um cliente de serviços de área de trabalho remota.</span><span class="sxs-lookup"><span data-stu-id="1952d-225">This user right determines which users and groups are prohibited from logging on as a Remote Desktop Services client.</span></span> <span data-ttu-id="1952d-226">Somente os estados não-configuradas e bloqueados são suportados</span><span class="sxs-lookup"><span data-stu-id="1952d-226">Only states NotConfigured and Blocked are supported</span></span>|
|<span data-ttu-id="1952d-227">userRightsDelegation</span><span class="sxs-lookup"><span data-stu-id="1952d-227">userRightsDelegation</span></span>|[<span data-ttu-id="1952d-228">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-228">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-229">Esse direito de usuário determina quais usuários podem definir a configuração confiável para delegação em um objeto de usuário ou computador.</span><span class="sxs-lookup"><span data-stu-id="1952d-229">This user right determines which users can set the Trusted for Delegation setting on a user or computer object.</span></span> <span data-ttu-id="1952d-230">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-230">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-231">userRightsGenerateSecurityAudits</span><span class="sxs-lookup"><span data-stu-id="1952d-231">userRightsGenerateSecurityAudits</span></span>|[<span data-ttu-id="1952d-232">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-232">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-233">Esse direito de usuário determina quais contas podem ser utilizadas por um processo para adicionar entradas no log de segurança.</span><span class="sxs-lookup"><span data-stu-id="1952d-233">This user right determines which accounts can be used by a process to add entries to the security log.</span></span> <span data-ttu-id="1952d-234">O log de segurança é usado para rastrear o acesso ao sistema não autorizado.</span><span class="sxs-lookup"><span data-stu-id="1952d-234">The security log is used to trace unauthorized system access.</span></span>  <span data-ttu-id="1952d-235">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-235">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-236">userRightsImpersonateClient</span><span class="sxs-lookup"><span data-stu-id="1952d-236">userRightsImpersonateClient</span></span>|[<span data-ttu-id="1952d-237">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-237">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-238">A atribuição desse direito de usuário a um usuário permite que programas em execução em nome desse usuário representar um cliente.</span><span class="sxs-lookup"><span data-stu-id="1952d-238">Assigning this user right to a user allows programs running on behalf of that user to impersonate a client.</span></span> <span data-ttu-id="1952d-239">Exigir este direito de usuário para esse tipo de representação impede que um usuário não autorizado convença um cliente para se conectar a um serviço que tenha criado e, em seguida, representar o cliente, que pode elevar as permissões do usuário não autorizado para administrativas ou níveis de sistema.</span><span class="sxs-lookup"><span data-stu-id="1952d-239">Requiring this user right for this kind of impersonation prevents an unauthorized user from convincing a client to connect to a service that they have created and then impersonating that client, which can elevate the unauthorized user's permissions to administrative or system levels.</span></span> <span data-ttu-id="1952d-240">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-240">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-241">userRightsIncreaseSchedulingPriority</span><span class="sxs-lookup"><span data-stu-id="1952d-241">userRightsIncreaseSchedulingPriority</span></span>|[<span data-ttu-id="1952d-242">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-242">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-243">Esse direito de usuário determina quais contas podem usar um processo com acesso propriedade gravação a outro processo para aumentar a prioridade de execução atribuída ao outro processo.</span><span class="sxs-lookup"><span data-stu-id="1952d-243">This user right determines which accounts can use a process with Write Property access to another process to increase the execution priority assigned to the other process.</span></span> <span data-ttu-id="1952d-244">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-244">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-245">userRightsLoadUnloadDrivers</span><span class="sxs-lookup"><span data-stu-id="1952d-245">userRightsLoadUnloadDrivers</span></span>|[<span data-ttu-id="1952d-246">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-246">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-247">Esse direito de usuário determina quais usuários podem carregar e descarregar drivers de dispositivo ou outros códigos para o modo kernel dinamicamente.</span><span class="sxs-lookup"><span data-stu-id="1952d-247">This user right determines which users can dynamically load and unload device drivers or other code in to kernel mode.</span></span> <span data-ttu-id="1952d-248">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-248">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-249">userRightsLockMemory</span><span class="sxs-lookup"><span data-stu-id="1952d-249">userRightsLockMemory</span></span>|[<span data-ttu-id="1952d-250">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-250">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-251">Esse direito de usuário determina quais contas podem usar um processo para manter dados na memória física, o que impede o sistema de colocar os dados na memória virtual em disco.</span><span class="sxs-lookup"><span data-stu-id="1952d-251">This user right determines which accounts can use a process to keep data in physical memory, which prevents the system from paging the data to virtual memory on disk.</span></span> <span data-ttu-id="1952d-252">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-252">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-253">userRightsManageAuditingAndSecurityLogs</span><span class="sxs-lookup"><span data-stu-id="1952d-253">userRightsManageAuditingAndSecurityLogs</span></span>|[<span data-ttu-id="1952d-254">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-254">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-255">Este direito de usuário determina quais usuários podem especificar opções para recursos individuais, como arquivos, objetos do Active Directory e chaves do registro de auditoria de acesso do objeto.</span><span class="sxs-lookup"><span data-stu-id="1952d-255">This user right determines which users can specify object access auditing options for individual resources, such as files, Active Directory objects, and registry keys.</span></span> <span data-ttu-id="1952d-256">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-256">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-257">userRightsManageVolumes</span><span class="sxs-lookup"><span data-stu-id="1952d-257">userRightsManageVolumes</span></span>|[<span data-ttu-id="1952d-258">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-258">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-259">Esse direito de usuário determina quais usuários e grupos podem executar tarefas de manutenção em um volume, como a desfragmentação remota.</span><span class="sxs-lookup"><span data-stu-id="1952d-259">This user right determines which users and groups can run maintenance tasks on a volume, such as remote defragmentation.</span></span> <span data-ttu-id="1952d-260">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-260">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-261">userRightsModifyFirmwareEnvironment</span><span class="sxs-lookup"><span data-stu-id="1952d-261">userRightsModifyFirmwareEnvironment</span></span>|[<span data-ttu-id="1952d-262">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-262">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-263">Este direito de usuário determina quem pode modificar valores de ambiente de firmware.</span><span class="sxs-lookup"><span data-stu-id="1952d-263">This user right determines who can modify firmware environment values.</span></span> <span data-ttu-id="1952d-264">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-264">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-265">userRightsModifyObjectLabels</span><span class="sxs-lookup"><span data-stu-id="1952d-265">userRightsModifyObjectLabels</span></span>|[<span data-ttu-id="1952d-266">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-266">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-267">Esse direito de usuário determina quais contas de usuário podem modificar o rótulo de integridade de objetos, como arquivos, chaves do registro ou processos pertencentes a outros usuários.</span><span class="sxs-lookup"><span data-stu-id="1952d-267">This user right determines which user accounts can modify the integrity label of objects, such as files, registry keys, or processes owned by other users.</span></span> <span data-ttu-id="1952d-268">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-268">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-269">userRightsProfileSingleProcess</span><span class="sxs-lookup"><span data-stu-id="1952d-269">userRightsProfileSingleProcess</span></span>|[<span data-ttu-id="1952d-270">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-270">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-271">Esse direito de usuário determina quais usuários podem usar ferramentas de monitoramento de desempenho para monitorar o desempenho de processos do sistema.</span><span class="sxs-lookup"><span data-stu-id="1952d-271">This user right determines which users can use performance monitoring tools to monitor the performance of system processes.</span></span> <span data-ttu-id="1952d-272">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-272">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-273">userRightsRemoteShutdown</span><span class="sxs-lookup"><span data-stu-id="1952d-273">userRightsRemoteShutdown</span></span>|[<span data-ttu-id="1952d-274">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-274">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-275">Esse direito de usuário determina quais usuários têm permissão para desligar um computador de um local remoto na rede.</span><span class="sxs-lookup"><span data-stu-id="1952d-275">This user right determines which users are allowed to shut down a computer from a remote location on the network.</span></span> <span data-ttu-id="1952d-276">Uso indevido desse direito de usuário pode resultar em uma negação de serviço.</span><span class="sxs-lookup"><span data-stu-id="1952d-276">Misuse of this user right can result in a denial of service.</span></span> <span data-ttu-id="1952d-277">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-277">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-278">userRightsRestoreData</span><span class="sxs-lookup"><span data-stu-id="1952d-278">userRightsRestoreData</span></span>|[<span data-ttu-id="1952d-279">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-279">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-280">Esse direito de usuário determina quais usuários podem ignorar o arquivo, diretório, registro e outros objetos persistentes permissões ao restaurar backup de arquivos e diretórios e determina quais usuários podem definir qualquer entidade de segurança válida como o proprietário de um objeto.</span><span class="sxs-lookup"><span data-stu-id="1952d-280">This user right determines which users can bypass file, directory, registry, and other persistent objects permissions when restoring backed up files and directories, and determines which users can set any valid security principal as the owner of an object.</span></span> <span data-ttu-id="1952d-281">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-281">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-282">userRightsTakeOwnership</span><span class="sxs-lookup"><span data-stu-id="1952d-282">userRightsTakeOwnership</span></span>|[<span data-ttu-id="1952d-283">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-283">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-284">Esse direito de usuário determina quais usuários podem apropriar-se de qualquer objeto protegível no sistema, incluindo objetos do Active Directory, arquivos e pastas, impressoras, chaves do registro, processos e segmentos.</span><span class="sxs-lookup"><span data-stu-id="1952d-284">This user right determines which users can take ownership of any securable object in the system, including Active Directory objects, files and folders, printers, registry keys, processes, and threads.</span></span> <span data-ttu-id="1952d-285">Somente os estados não-configuradas e permitidos são suportados.</span><span class="sxs-lookup"><span data-stu-id="1952d-285">Only states NotConfigured and Allowed are supported.</span></span>|
|<span data-ttu-id="1952d-286">userRightsRegisterProcessAsService</span><span class="sxs-lookup"><span data-stu-id="1952d-286">userRightsRegisterProcessAsService</span></span>|[<span data-ttu-id="1952d-287">deviceManagementUserRightsSetting</span><span class="sxs-lookup"><span data-stu-id="1952d-287">deviceManagementUserRightsSetting</span></span>](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|<span data-ttu-id="1952d-288">Essa configuração de segurança determina quais contas de serviço são impedidas de registrar um processo como um serviço.</span><span class="sxs-lookup"><span data-stu-id="1952d-288">This security setting determines which service accounts are prevented from registering a process as a service.</span></span> <span data-ttu-id="1952d-289">Observação: Essa configuração de segurança não se aplica às contas de sistema, serviço Local ou serviço de rede.</span><span class="sxs-lookup"><span data-stu-id="1952d-289">Note: This security setting does not apply to the System, Local Service, or Network Service accounts.</span></span> <span data-ttu-id="1952d-290">Único estado bloqueado é suportado.</span><span class="sxs-lookup"><span data-stu-id="1952d-290">Only state Blocked is supported.</span></span>|
|<span data-ttu-id="1952d-291">xboxServicesEnableXboxGameSaveTask</span><span class="sxs-lookup"><span data-stu-id="1952d-291">xboxServicesEnableXboxGameSaveTask</span></span>|<span data-ttu-id="1952d-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-292">Boolean</span></span>|<span data-ttu-id="1952d-293">Essa configuração determina se salvar jogo do xbox está habilitado (1) ou desativada (0).</span><span class="sxs-lookup"><span data-stu-id="1952d-293">This setting determines whether xbox game save is enabled (1) or disabled (0).</span></span>|
|<span data-ttu-id="1952d-294">xboxServicesAccessoryManagementServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="1952d-294">xboxServicesAccessoryManagementServiceStartupMode</span></span>|[<span data-ttu-id="1952d-295">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="1952d-295">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="1952d-296">Essa configuração determina se o tipo de início do serviço de gerenciamento de acessório é Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="1952d-296">This setting determines whether the Accessory management service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="1952d-297">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="1952d-297">Default: Manual.</span></span> <span data-ttu-id="1952d-298">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1952d-298">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="1952d-299">xboxServicesLiveAuthManagerServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="1952d-299">xboxServicesLiveAuthManagerServiceStartupMode</span></span>|[<span data-ttu-id="1952d-300">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="1952d-300">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="1952d-301">Essa configuração determina se o tipo de início do serviço do Gerenciador de autenticação Live é Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="1952d-301">This setting determines whether Live Auth Manager service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="1952d-302">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="1952d-302">Default: Manual.</span></span> <span data-ttu-id="1952d-303">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1952d-303">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="1952d-304">xboxServicesLiveGameSaveServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="1952d-304">xboxServicesLiveGameSaveServiceStartupMode</span></span>|[<span data-ttu-id="1952d-305">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="1952d-305">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="1952d-306">Essa configuração determina se o jogo Live salvar o tipo de início do serviço é Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="1952d-306">This setting determines whether Live Game save service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="1952d-307">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="1952d-307">Default: Manual.</span></span> <span data-ttu-id="1952d-308">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1952d-308">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="1952d-309">xboxServicesLiveNetworkingServiceStartupMode</span><span class="sxs-lookup"><span data-stu-id="1952d-309">xboxServicesLiveNetworkingServiceStartupMode</span></span>|[<span data-ttu-id="1952d-310">serviceStartType</span><span class="sxs-lookup"><span data-stu-id="1952d-310">serviceStartType</span></span>](../resources/intune-deviceconfig-servicestarttype.md)|<span data-ttu-id="1952d-311">Essa configuração determina se o tipo de início do serviço de rede é Automatic(2), Manual(3), Disabled(4).</span><span class="sxs-lookup"><span data-stu-id="1952d-311">This setting determines whether Networking service's start type is Automatic(2), Manual(3), Disabled(4).</span></span> <span data-ttu-id="1952d-312">Padrão: Manual.</span><span class="sxs-lookup"><span data-stu-id="1952d-312">Default: Manual.</span></span> <span data-ttu-id="1952d-313">Os valores possíveis são: `manual`, `automatic`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1952d-313">Possible values are: `manual`, `automatic`, `disabled`.</span></span>|
|<span data-ttu-id="1952d-314">localSecurityOptionsBlockMicrosoftAccounts</span><span class="sxs-lookup"><span data-stu-id="1952d-314">localSecurityOptionsBlockMicrosoftAccounts</span></span>|<span data-ttu-id="1952d-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-315">Boolean</span></span>|<span data-ttu-id="1952d-316">Impedir que os usuários adicionem novas contas da Microsoft para este computador.</span><span class="sxs-lookup"><span data-stu-id="1952d-316">Prevent users from adding new Microsoft accounts to this computer.</span></span>|
|<span data-ttu-id="1952d-317">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span><span class="sxs-lookup"><span data-stu-id="1952d-317">localSecurityOptionsBlockRemoteLogonWithBlankPassword</span></span>|<span data-ttu-id="1952d-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-318">Boolean</span></span>|<span data-ttu-id="1952d-319">Habilite as contas locais que não são protegida para logon de locais que não seja o dispositivo físico de senha. É habilitada por padrão</span><span class="sxs-lookup"><span data-stu-id="1952d-319">Enable Local accounts that are not password protected to log on from locations other than the physical device.Default is enabled</span></span>|
|<span data-ttu-id="1952d-320">localSecurityOptionsEnableAdministratorAccount</span><span class="sxs-lookup"><span data-stu-id="1952d-320">localSecurityOptionsEnableAdministratorAccount</span></span>|<span data-ttu-id="1952d-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-321">Boolean</span></span>|<span data-ttu-id="1952d-322">Determina se a conta de Administrador Local está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="1952d-322">Determines whether the Local Administrator account is enabled or disabled.</span></span>|
|<span data-ttu-id="1952d-323">localSecurityOptionsAdministratorAccountName</span><span class="sxs-lookup"><span data-stu-id="1952d-323">localSecurityOptionsAdministratorAccountName</span></span>|<span data-ttu-id="1952d-324">String</span><span class="sxs-lookup"><span data-stu-id="1952d-324">String</span></span>|<span data-ttu-id="1952d-325">Defina um nome de conta diferente a ser associado com o identificador de segurança (SID) da conta "Administrador".</span><span class="sxs-lookup"><span data-stu-id="1952d-325">Define a different account name to be associated with the security identifier (SID) for the account “Administrator”.</span></span>|
|<span data-ttu-id="1952d-326">localSecurityOptionsEnableGuestAccount</span><span class="sxs-lookup"><span data-stu-id="1952d-326">localSecurityOptionsEnableGuestAccount</span></span>|<span data-ttu-id="1952d-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-327">Boolean</span></span>|<span data-ttu-id="1952d-328">Determina se a conta de convidado está habilitada ou desabilitada.</span><span class="sxs-lookup"><span data-stu-id="1952d-328">Determines if the Guest account is enabled or disabled.</span></span>|
|<span data-ttu-id="1952d-329">localSecurityOptionsGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="1952d-329">localSecurityOptionsGuestAccountName</span></span>|<span data-ttu-id="1952d-330">String</span><span class="sxs-lookup"><span data-stu-id="1952d-330">String</span></span>|<span data-ttu-id="1952d-331">Defina um nome de conta diferente a ser associado com o identificador de segurança (SID) da conta "Convidado".</span><span class="sxs-lookup"><span data-stu-id="1952d-331">Define a different account name to be associated with the security identifier (SID) for the account “Guest”.</span></span>|
|<span data-ttu-id="1952d-332">localSecurityOptionsAllowUndockWithoutHavingToLogon</span><span class="sxs-lookup"><span data-stu-id="1952d-332">localSecurityOptionsAllowUndockWithoutHavingToLogon</span></span>|<span data-ttu-id="1952d-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-333">Boolean</span></span>|<span data-ttu-id="1952d-334">Impedir que um computador portátil sendo não encaixado sem precisar fazer logon.</span><span class="sxs-lookup"><span data-stu-id="1952d-334">Prevent a portable computer from being undocked without having to log in.</span></span>|
|<span data-ttu-id="1952d-335">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span><span class="sxs-lookup"><span data-stu-id="1952d-335">localSecurityOptionsBlockUsersInstallingPrinterDrivers</span></span>|<span data-ttu-id="1952d-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-336">Boolean</span></span>|<span data-ttu-id="1952d-337">Restringir instalando drivers de impressora como parte da conexão a uma impressora compartilhada ao grupo Administradores apenas.</span><span class="sxs-lookup"><span data-stu-id="1952d-337">Restrict installing printer drivers as part of connecting to a shared printer to admins only.</span></span>|
|<span data-ttu-id="1952d-338">localSecurityOptionsBlockRemoteOpticalDriveAccess</span><span class="sxs-lookup"><span data-stu-id="1952d-338">localSecurityOptionsBlockRemoteOpticalDriveAccess</span></span>|<span data-ttu-id="1952d-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-339">Boolean</span></span>|<span data-ttu-id="1952d-340">A ativação dessa configuração permite que somente usuário conectado interativamente mídia de CD-ROM do access.</span><span class="sxs-lookup"><span data-stu-id="1952d-340">Enabling this settings allows only interactively logged on user to access CD-ROM media.</span></span>|
|<span data-ttu-id="1952d-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span><span class="sxs-lookup"><span data-stu-id="1952d-341">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser</span></span>|[<span data-ttu-id="1952d-342">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span><span class="sxs-lookup"><span data-stu-id="1952d-342">localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUserType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|<span data-ttu-id="1952d-343">Defina quem tem permissão para formatar e ejeção mídia NTFS removível.</span><span class="sxs-lookup"><span data-stu-id="1952d-343">Define who is allowed to format and eject removable NTFS media.</span></span> <span data-ttu-id="1952d-344">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="1952d-344">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="1952d-345">localSecurityOptionsMachineInactivityLimit</span><span class="sxs-lookup"><span data-stu-id="1952d-345">localSecurityOptionsMachineInactivityLimit</span></span>|<span data-ttu-id="1952d-346">Int32</span><span class="sxs-lookup"><span data-stu-id="1952d-346">Int32</span></span>|<span data-ttu-id="1952d-347">Defina o máximo de minutos de inatividade na tela de login da área de trabalho interativo até o protetor de tela é executado.</span><span class="sxs-lookup"><span data-stu-id="1952d-347">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="1952d-348">Valores válidos 0 e 9999</span><span class="sxs-lookup"><span data-stu-id="1952d-348">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="1952d-349">localSecurityOptionsMachineInactivityLimitInMinutes</span><span class="sxs-lookup"><span data-stu-id="1952d-349">localSecurityOptionsMachineInactivityLimitInMinutes</span></span>|<span data-ttu-id="1952d-350">Int32</span><span class="sxs-lookup"><span data-stu-id="1952d-350">Int32</span></span>|<span data-ttu-id="1952d-351">Defina o máximo de minutos de inatividade na tela de login da área de trabalho interativo até o protetor de tela é executado.</span><span class="sxs-lookup"><span data-stu-id="1952d-351">Define maximum minutes of inactivity on the interactive desktop’s login screen until the screen saver runs.</span></span> <span data-ttu-id="1952d-352">Valores válidos 0 e 9999</span><span class="sxs-lookup"><span data-stu-id="1952d-352">Valid values 0 to 9999</span></span>|
|<span data-ttu-id="1952d-353">localSecurityOptionsDoNotRequireCtrlAltDel</span><span class="sxs-lookup"><span data-stu-id="1952d-353">localSecurityOptionsDoNotRequireCtrlAltDel</span></span>|<span data-ttu-id="1952d-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-354">Boolean</span></span>|<span data-ttu-id="1952d-355">Exigir CTRL + ALT + DEL a ser pressionada para que um usuário possa fazer logon.</span><span class="sxs-lookup"><span data-stu-id="1952d-355">Require CTRL+ALT+DEL to be pressed before a user can log on.</span></span>|
|<span data-ttu-id="1952d-356">localSecurityOptionsHideLastSignedInUser</span><span class="sxs-lookup"><span data-stu-id="1952d-356">localSecurityOptionsHideLastSignedInUser</span></span>|<span data-ttu-id="1952d-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-357">Boolean</span></span>|<span data-ttu-id="1952d-358">Não exibe o nome de usuário da última pessoa que entraram nesse dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1952d-358">Do not display the username of the last person who signed in on this device.</span></span>|
|<span data-ttu-id="1952d-359">localSecurityOptionsHideUsernameAtSignIn</span><span class="sxs-lookup"><span data-stu-id="1952d-359">localSecurityOptionsHideUsernameAtSignIn</span></span>|<span data-ttu-id="1952d-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-360">Boolean</span></span>|<span data-ttu-id="1952d-361">Não exibe o nome de usuário da pessoa entrando para este dispositivo após credenciais são inseridas e antes de área de trabalho do dispositivo é mostrada.</span><span class="sxs-lookup"><span data-stu-id="1952d-361">Do not display the username of the person signing in to this device after credentials are entered and before the device’s desktop is shown.</span></span>|
|<span data-ttu-id="1952d-362">localSecurityOptionsLogOnMessageTitle</span><span class="sxs-lookup"><span data-stu-id="1952d-362">localSecurityOptionsLogOnMessageTitle</span></span>|<span data-ttu-id="1952d-363">String</span><span class="sxs-lookup"><span data-stu-id="1952d-363">String</span></span>|<span data-ttu-id="1952d-364">Defina o título da mensagem para usuários tentando fazer logon.</span><span class="sxs-lookup"><span data-stu-id="1952d-364">Set message title for users attempting to log in.</span></span>|
|<span data-ttu-id="1952d-365">localSecurityOptionsLogOnMessageText</span><span class="sxs-lookup"><span data-stu-id="1952d-365">localSecurityOptionsLogOnMessageText</span></span>|<span data-ttu-id="1952d-366">String</span><span class="sxs-lookup"><span data-stu-id="1952d-366">String</span></span>|<span data-ttu-id="1952d-367">Definir o texto da mensagem para os usuários que tentarem fazer logon.</span><span class="sxs-lookup"><span data-stu-id="1952d-367">Set message text for users attempting to log in.</span></span>|
|<span data-ttu-id="1952d-368">localSecurityOptionsAllowPKU2UAuthenticationRequests</span><span class="sxs-lookup"><span data-stu-id="1952d-368">localSecurityOptionsAllowPKU2UAuthenticationRequests</span></span>|<span data-ttu-id="1952d-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-369">Boolean</span></span>|<span data-ttu-id="1952d-370">Solicitações de autenticação de bloco PKU2U para este dispositivo usar identidades on-line.</span><span class="sxs-lookup"><span data-stu-id="1952d-370">Block PKU2U authentication requests to this device to use online identities.</span></span>|
|<span data-ttu-id="1952d-371">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span><span class="sxs-lookup"><span data-stu-id="1952d-371">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool</span></span>|<span data-ttu-id="1952d-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-372">Boolean</span></span>|<span data-ttu-id="1952d-373">Auxiliar da UI do boolean para entidade LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="1952d-373">UI helper boolean for LocalSecurityOptionsAllowRemoteCallsToSecurityAccountsManager entity</span></span>|
|<span data-ttu-id="1952d-374">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span><span class="sxs-lookup"><span data-stu-id="1952d-374">localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager</span></span>|<span data-ttu-id="1952d-375">String</span><span class="sxs-lookup"><span data-stu-id="1952d-375">String</span></span>|<span data-ttu-id="1952d-376">Edite a cadeia de caracteres de linguagem de definição de descritor de segurança padrão para permitir ou negar a usuários e grupos para fazer chamadas remotas para o SAM.</span><span class="sxs-lookup"><span data-stu-id="1952d-376">Edit the default Security Descriptor Definition Language string to allow or deny users and groups to make remote calls to the SAM.</span></span>|
|<span data-ttu-id="1952d-377">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span><span class="sxs-lookup"><span data-stu-id="1952d-377">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients</span></span>|[<span data-ttu-id="1952d-378">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="1952d-378">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="1952d-379">Essa configuração de segurança permite que um cliente exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="1952d-379">This security setting allows a client to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="1952d-380">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="1952d-380">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="1952d-381">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span><span class="sxs-lookup"><span data-stu-id="1952d-381">localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers</span></span>|[<span data-ttu-id="1952d-382">localSecurityOptionsMinimumSessionSecurity</span><span class="sxs-lookup"><span data-stu-id="1952d-382">localSecurityOptionsMinimumSessionSecurity</span></span>](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|<span data-ttu-id="1952d-383">Essa configuração de segurança permite que um servidor exija a negociação de criptografia de 128 bits e/ou segurança de sessão NTLMv2.</span><span class="sxs-lookup"><span data-stu-id="1952d-383">This security setting allows a server to require the negotiation of 128-bit encryption and/or NTLMv2 session security.</span></span> <span data-ttu-id="1952d-384">Os valores possíveis são: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span><span class="sxs-lookup"><span data-stu-id="1952d-384">Possible values are: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.</span></span>|
|<span data-ttu-id="1952d-385">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="1952d-385">lanManagerAuthenticationLevel</span></span>|[<span data-ttu-id="1952d-386">lanManagerAuthenticationLevel</span><span class="sxs-lookup"><span data-stu-id="1952d-386">lanManagerAuthenticationLevel</span></span>](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|<span data-ttu-id="1952d-387">Essa configuração de segurança determina qual protocolo de autenticação de desafio/resposta é usado para logons de rede.</span><span class="sxs-lookup"><span data-stu-id="1952d-387">This security setting determines which challenge/response authentication protocol is used for network logons.</span></span> <span data-ttu-id="1952d-388">Os possíveis valores são: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span><span class="sxs-lookup"><span data-stu-id="1952d-388">Possible values are: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.</span></span>|
|<span data-ttu-id="1952d-389">lanManagerWorkstationEnableInsecureGuestLogons</span><span class="sxs-lookup"><span data-stu-id="1952d-389">lanManagerWorkstationEnableInsecureGuestLogons</span></span>|<span data-ttu-id="1952d-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-390">Boolean</span></span>|<span data-ttu-id="1952d-391">Se for habilitada, o cliente SMB permitirá que os logons de convidado inseguros.</span><span class="sxs-lookup"><span data-stu-id="1952d-391">If enabled,the SMB client will allow insecure guest logons.</span></span> <span data-ttu-id="1952d-392">Se não estiver configurado, o cliente SMB rejeitará logons de convidado inseguros.</span><span class="sxs-lookup"><span data-stu-id="1952d-392">If not configured, the SMB client will reject insecure guest logons.</span></span>|
|<span data-ttu-id="1952d-393">localSecurityOptionsClearVirtualMemoryPageFile</span><span class="sxs-lookup"><span data-stu-id="1952d-393">localSecurityOptionsClearVirtualMemoryPageFile</span></span>|<span data-ttu-id="1952d-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-394">Boolean</span></span>|<span data-ttu-id="1952d-395">Essa configuração de segurança determina se o arquivo de paginação de memória virtual será limpo quando o sistema for desligado.</span><span class="sxs-lookup"><span data-stu-id="1952d-395">This security setting determines whether the virtual memory pagefile is cleared when the system is shut down.</span></span>|
|<span data-ttu-id="1952d-396">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span><span class="sxs-lookup"><span data-stu-id="1952d-396">localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn</span></span>|<span data-ttu-id="1952d-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-397">Boolean</span></span>|<span data-ttu-id="1952d-398">Essa configuração de segurança determina se um computador pode ser desligado sem precisar fazer logon no Windows.</span><span class="sxs-lookup"><span data-stu-id="1952d-398">This security setting determines whether a computer can be shut down without having to log on to Windows.</span></span>|
|<span data-ttu-id="1952d-399">localSecurityOptionsAllowUIAccessApplicationElevation</span><span class="sxs-lookup"><span data-stu-id="1952d-399">localSecurityOptionsAllowUIAccessApplicationElevation</span></span>|<span data-ttu-id="1952d-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-400">Boolean</span></span>|<span data-ttu-id="1952d-401">Permitir aplicativos UIAccess solicitar elevação sem usar a área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="1952d-401">Allow UIAccess apps to prompt for elevation without using the secure desktop.</span></span>|
|<span data-ttu-id="1952d-402">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span><span class="sxs-lookup"><span data-stu-id="1952d-402">localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations</span></span>|<span data-ttu-id="1952d-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-403">Boolean</span></span>|<span data-ttu-id="1952d-404">Virtualizar falhas de gravação de arquivo e registro a para por usuário locais</span><span class="sxs-lookup"><span data-stu-id="1952d-404">Virtualize file and registry write failures to per user locations</span></span>|
|<span data-ttu-id="1952d-405">localSecurityOptionsOnlyElevateSignedExecutables</span><span class="sxs-lookup"><span data-stu-id="1952d-405">localSecurityOptionsOnlyElevateSignedExecutables</span></span>|<span data-ttu-id="1952d-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-406">Boolean</span></span>|<span data-ttu-id="1952d-407">Impor a validação de caminho de certificação PKI para um determinado arquivo executável antes que ele tem permissão para executar.</span><span class="sxs-lookup"><span data-stu-id="1952d-407">Enforce PKI certification path validation for a given executable file before it is permitted to run.</span></span>|
|<span data-ttu-id="1952d-408">localSecurityOptionsAdministratorElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="1952d-408">localSecurityOptionsAdministratorElevationPromptBehavior</span></span>|[<span data-ttu-id="1952d-409">localSecurityOptionsAdministratorElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="1952d-409">localSecurityOptionsAdministratorElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|<span data-ttu-id="1952d-410">Defina o comportamento da solicitação de elevação para administradores no modo de aprovação de administrador.</span><span class="sxs-lookup"><span data-stu-id="1952d-410">Define the behavior of the elevation prompt for admins in Admin Approval Mode.</span></span> <span data-ttu-id="1952d-411">Os valores possíveis são: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span><span class="sxs-lookup"><span data-stu-id="1952d-411">Possible values are: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.</span></span>|
|<span data-ttu-id="1952d-412">localSecurityOptionsStandardUserElevationPromptBehavior</span><span class="sxs-lookup"><span data-stu-id="1952d-412">localSecurityOptionsStandardUserElevationPromptBehavior</span></span>|[<span data-ttu-id="1952d-413">localSecurityOptionsStandardUserElevationPromptBehaviorType</span><span class="sxs-lookup"><span data-stu-id="1952d-413">localSecurityOptionsStandardUserElevationPromptBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|<span data-ttu-id="1952d-414">Defina o comportamento da solicitação de elevação para usuários padrão.</span><span class="sxs-lookup"><span data-stu-id="1952d-414">Define the behavior of the elevation prompt for standard users.</span></span> <span data-ttu-id="1952d-415">Os valores possíveis são: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span><span class="sxs-lookup"><span data-stu-id="1952d-415">Possible values are: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.</span></span>|
|<span data-ttu-id="1952d-416">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span><span class="sxs-lookup"><span data-stu-id="1952d-416">localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation</span></span>|<span data-ttu-id="1952d-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-417">Boolean</span></span>|<span data-ttu-id="1952d-418">Habilite todas as solicitações de elevação ir para a área de trabalho do usuário interativa em vez de área de trabalho segura.</span><span class="sxs-lookup"><span data-stu-id="1952d-418">Enable all elevation requests to go to the interactive user's desktop rather than the secure desktop.</span></span> <span data-ttu-id="1952d-419">Configurações de diretiva de comportamento de solicitação para administradores e usuários padrão são usadas.</span><span class="sxs-lookup"><span data-stu-id="1952d-419">Prompt behavior policy settings for admins and standard users are used.</span></span>|
|<span data-ttu-id="1952d-420">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span><span class="sxs-lookup"><span data-stu-id="1952d-420">localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation</span></span>|<span data-ttu-id="1952d-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-421">Boolean</span></span>|<span data-ttu-id="1952d-422">Instalações de aplicativo exigir privilégios elevados vai solicitar credenciais de administrador. É habilitada por padrão</span><span class="sxs-lookup"><span data-stu-id="1952d-422">App installations requiring elevated privileges will prompt for admin credentials.Default is enabled</span></span>|
|<span data-ttu-id="1952d-423">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span><span class="sxs-lookup"><span data-stu-id="1952d-423">localSecurityOptionsAllowUIAccessApplicationsForSecureLocations</span></span>|<span data-ttu-id="1952d-424">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-424">Boolean</span></span>|<span data-ttu-id="1952d-425">Permitir aplicativos UIAccess solicitar elevação sem usar a área de trabalho segura. É habilitada por padrão</span><span class="sxs-lookup"><span data-stu-id="1952d-425">Allow UIAccess apps to prompt for elevation without using the secure desktop.Default is enabled</span></span>|
|<span data-ttu-id="1952d-426">localSecurityOptionsUseAdminApprovalMode</span><span class="sxs-lookup"><span data-stu-id="1952d-426">localSecurityOptionsUseAdminApprovalMode</span></span>|<span data-ttu-id="1952d-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-427">Boolean</span></span>|<span data-ttu-id="1952d-428">Define se a conta de administrador interna usa o modo de aprovação de administrador ou executa todos os aplicativos com privilégios de administrador completo. É habilitada por padrão</span><span class="sxs-lookup"><span data-stu-id="1952d-428">Defines whether the built-in admin account uses Admin Approval Mode or runs all apps with full admin privileges.Default is enabled</span></span>|
|<span data-ttu-id="1952d-429">localSecurityOptionsUseAdminApprovalModeForAdministrators</span><span class="sxs-lookup"><span data-stu-id="1952d-429">localSecurityOptionsUseAdminApprovalModeForAdministrators</span></span>|<span data-ttu-id="1952d-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-430">Boolean</span></span>|<span data-ttu-id="1952d-431">Defina se o modo de aprovação de administrador e todas as configurações de diretiva UAC estão habilitadas, é habilitada por padrão</span><span class="sxs-lookup"><span data-stu-id="1952d-431">Define whether Admin Approval Mode and all UAC policy settings are enabled, default is enabled</span></span>|
|<span data-ttu-id="1952d-432">localSecurityOptionsInformationShownOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="1952d-432">localSecurityOptionsInformationShownOnLockScreen</span></span>|[<span data-ttu-id="1952d-433">localSecurityOptionsInformationShownOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="1952d-433">localSecurityOptionsInformationShownOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|<span data-ttu-id="1952d-434">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1952d-434">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="1952d-435">Se não estiver configurado, username, domínio e nome de exibição do usuário são mostrados.</span><span class="sxs-lookup"><span data-stu-id="1952d-435">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="1952d-436">Os valores possíveis são: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span><span class="sxs-lookup"><span data-stu-id="1952d-436">Possible values are: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.</span></span>|
|<span data-ttu-id="1952d-437">localSecurityOptionsInformationDisplayedOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="1952d-437">localSecurityOptionsInformationDisplayedOnLockScreen</span></span>|[<span data-ttu-id="1952d-438">localSecurityOptionsInformationDisplayedOnLockScreenType</span><span class="sxs-lookup"><span data-stu-id="1952d-438">localSecurityOptionsInformationDisplayedOnLockScreenType</span></span>](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|<span data-ttu-id="1952d-439">Configure as informações do usuário que são exibidas quando a sessão está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1952d-439">Configure the user information that is displayed when the session is locked.</span></span> <span data-ttu-id="1952d-440">Se não estiver configurado, username, domínio e nome de exibição do usuário são mostrados.</span><span class="sxs-lookup"><span data-stu-id="1952d-440">If not configured, user display name, domain and username are shown.</span></span> <span data-ttu-id="1952d-441">Os valores possíveis são: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span><span class="sxs-lookup"><span data-stu-id="1952d-441">Possible values are: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.</span></span>|
|<span data-ttu-id="1952d-442">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span><span class="sxs-lookup"><span data-stu-id="1952d-442">localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees</span></span>|<span data-ttu-id="1952d-443">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-443">Boolean</span></span>|<span data-ttu-id="1952d-444">Essa configuração determina se o cliente SMB tentará negociar a assinatura de pacotes SMB.</span><span class="sxs-lookup"><span data-stu-id="1952d-444">This security setting determines whether the SMB client attempts to negotiate SMB packet signing.</span></span>|
|<span data-ttu-id="1952d-445">localSecurityOptionsClientDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="1952d-445">localSecurityOptionsClientDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="1952d-446">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-446">Boolean</span></span>|<span data-ttu-id="1952d-447">Essa configuração de segurança determina se a assinatura de pacotes é exigida pelo componente cliente do SMB.</span><span class="sxs-lookup"><span data-stu-id="1952d-447">This security setting determines whether packet signing is required by the SMB client component.</span></span>|
|<span data-ttu-id="1952d-448">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span><span class="sxs-lookup"><span data-stu-id="1952d-448">localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers</span></span>|<span data-ttu-id="1952d-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-449">Boolean</span></span>|<span data-ttu-id="1952d-450">Se essa configuração de segurança estiver habilitada, o redirecionador de bloco de mensagens do servidor (SMB) é permitido para enviar senhas de texto sem formatação para servidores SMB não Microsoft que não têm suporte para criptografia de senha durante a autenticação.</span><span class="sxs-lookup"><span data-stu-id="1952d-450">If this security setting is enabled, the Server Message Block (SMB) redirector is allowed to send plaintext passwords to non-Microsoft SMB servers that do not support password encryption during authentication.</span></span>|
|<span data-ttu-id="1952d-451">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span><span class="sxs-lookup"><span data-stu-id="1952d-451">localSecurityOptionsDisableServerDigitallySignCommunicationsAlways</span></span>|<span data-ttu-id="1952d-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-452">Boolean</span></span>|<span data-ttu-id="1952d-453">Essa configuração de segurança determina se a assinatura de pacotes é exigida pelo componente de servidor SMB.</span><span class="sxs-lookup"><span data-stu-id="1952d-453">This security setting determines whether packet signing is required by the SMB server component.</span></span>|
|<span data-ttu-id="1952d-454">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span><span class="sxs-lookup"><span data-stu-id="1952d-454">localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees</span></span>|<span data-ttu-id="1952d-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-455">Boolean</span></span>|<span data-ttu-id="1952d-456">Essa configuração de segurança determina se o servidor SMB irá negociar assinatura com clientes que solicitarem de pacotes SMB.</span><span class="sxs-lookup"><span data-stu-id="1952d-456">This security setting determines whether the SMB server will negotiate SMB packet signing with clients that request it.</span></span>|
|<span data-ttu-id="1952d-457">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span><span class="sxs-lookup"><span data-stu-id="1952d-457">localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares</span></span>|<span data-ttu-id="1952d-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-458">Boolean</span></span>|<span data-ttu-id="1952d-459">Por padrão, essa configuração de segurança restringe o acesso anônimo a compartilhamentos e pipes para as configurações de pipes nomeados que podem ser acessados anonimamente e compartilhamentos que podem ser acessados anonimamente</span><span class="sxs-lookup"><span data-stu-id="1952d-459">By default, this security setting restricts anonymous access to shares and pipes to the settings for named pipes that can be accessed anonymously and Shares that can be accessed anonymously</span></span>|
|<span data-ttu-id="1952d-460">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span><span class="sxs-lookup"><span data-stu-id="1952d-460">localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts</span></span>|<span data-ttu-id="1952d-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-461">Boolean</span></span>|<span data-ttu-id="1952d-462">Essa configuração de segurança determina quais permissões adicionais serão concedidas para conexões anônimas ao computador.</span><span class="sxs-lookup"><span data-stu-id="1952d-462">This security setting determines what additional permissions will be granted for anonymous connections to the computer.</span></span>|
|<span data-ttu-id="1952d-463">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span><span class="sxs-lookup"><span data-stu-id="1952d-463">localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares</span></span>|<span data-ttu-id="1952d-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-464">Boolean</span></span>|<span data-ttu-id="1952d-465">Essa configuração de segurança determina se deve ser permite que usuários anônimos executem determinadas atividades, como enumeração de nomes de contas de domínio e compartilhamentos de rede.</span><span class="sxs-lookup"><span data-stu-id="1952d-465">This security setting determines whether to allows anonymous users to perform certain activities, such as enumerating the names of domain accounts and network shares.</span></span>|
|<span data-ttu-id="1952d-466">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span><span class="sxs-lookup"><span data-stu-id="1952d-466">localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange</span></span>|<span data-ttu-id="1952d-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-467">Boolean</span></span>|<span data-ttu-id="1952d-468">Essa configuração de segurança determina se, na próxima alteração de senha, o valor de hash do LM (LAN Manager) para a nova senha é armazenado.</span><span class="sxs-lookup"><span data-stu-id="1952d-468">This security setting determines if, at the next password change, the LAN Manager (LM) hash value for the new password is stored.</span></span> <span data-ttu-id="1952d-469">Ele não é armazenado por padrão.</span><span class="sxs-lookup"><span data-stu-id="1952d-469">It’s not stored by default.</span></span>|
|<span data-ttu-id="1952d-470">localSecurityOptionsSmartCardRemovalBehavior</span><span class="sxs-lookup"><span data-stu-id="1952d-470">localSecurityOptionsSmartCardRemovalBehavior</span></span>|[<span data-ttu-id="1952d-471">localSecurityOptionsSmartCardRemovalBehaviorType</span><span class="sxs-lookup"><span data-stu-id="1952d-471">localSecurityOptionsSmartCardRemovalBehaviorType</span></span>](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md)|<span data-ttu-id="1952d-472">Essa configuração de segurança determina o que acontece quando o cartão inteligente de um usuário conectado é removido do leitor de cartão inteligente.</span><span class="sxs-lookup"><span data-stu-id="1952d-472">This security setting determines what happens when the smart card for a logged-on user is removed from the smart card reader.</span></span> <span data-ttu-id="1952d-473">Os valores possíveis são: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span><span class="sxs-lookup"><span data-stu-id="1952d-473">Possible values are: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.</span></span>|
|<span data-ttu-id="1952d-474">defenderSecurityCenterDisableAppBrowserUI</span><span class="sxs-lookup"><span data-stu-id="1952d-474">defenderSecurityCenterDisableAppBrowserUI</span></span>|<span data-ttu-id="1952d-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-475">Boolean</span></span>|<span data-ttu-id="1952d-476">Usada para desabilitar a exibição da área de proteção de aplicativo e de navegador.</span><span class="sxs-lookup"><span data-stu-id="1952d-476">Used to disable the display of the app and browser protection area.</span></span>|
|<span data-ttu-id="1952d-477">defenderSecurityCenterDisableFamilyUI</span><span class="sxs-lookup"><span data-stu-id="1952d-477">defenderSecurityCenterDisableFamilyUI</span></span>|<span data-ttu-id="1952d-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-478">Boolean</span></span>|<span data-ttu-id="1952d-479">Usada para desabilitar a exibição da área de opções da família.</span><span class="sxs-lookup"><span data-stu-id="1952d-479">Used to disable the display of the family options area.</span></span>|
|<span data-ttu-id="1952d-480">defenderSecurityCenterDisableHealthUI</span><span class="sxs-lookup"><span data-stu-id="1952d-480">defenderSecurityCenterDisableHealthUI</span></span>|<span data-ttu-id="1952d-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-481">Boolean</span></span>|<span data-ttu-id="1952d-482">Usada para desabilitar a exibição da área de integridade e desempenho do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1952d-482">Used to disable the display of the device performance and health area.</span></span>|
|<span data-ttu-id="1952d-483">defenderSecurityCenterDisableNetworkUI</span><span class="sxs-lookup"><span data-stu-id="1952d-483">defenderSecurityCenterDisableNetworkUI</span></span>|<span data-ttu-id="1952d-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-484">Boolean</span></span>|<span data-ttu-id="1952d-485">Usada para desabilitar a exibição da área de proteção de rede e de firewall.</span><span class="sxs-lookup"><span data-stu-id="1952d-485">Used to disable the display of the firewall and network protection area.</span></span>|
|<span data-ttu-id="1952d-486">defenderSecurityCenterDisableVirusUI</span><span class="sxs-lookup"><span data-stu-id="1952d-486">defenderSecurityCenterDisableVirusUI</span></span>|<span data-ttu-id="1952d-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-487">Boolean</span></span>|<span data-ttu-id="1952d-488">Usada para desabilitar a exibição da área de proteção de vírus e ameaças.</span><span class="sxs-lookup"><span data-stu-id="1952d-488">Used to disable the display of the virus and threat protection area.</span></span>|
|<span data-ttu-id="1952d-489">defenderSecurityCenterDisableAccountUI</span><span class="sxs-lookup"><span data-stu-id="1952d-489">defenderSecurityCenterDisableAccountUI</span></span>|<span data-ttu-id="1952d-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-490">Boolean</span></span>|<span data-ttu-id="1952d-491">Usada para desabilitar a exibição da área de proteção de conta.</span><span class="sxs-lookup"><span data-stu-id="1952d-491">Used to disable the display of the account protection area.</span></span>|
|<span data-ttu-id="1952d-492">defenderSecurityCenterDisableHardwareUI</span><span class="sxs-lookup"><span data-stu-id="1952d-492">defenderSecurityCenterDisableHardwareUI</span></span>|<span data-ttu-id="1952d-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-493">Boolean</span></span>|<span data-ttu-id="1952d-494">Usada para desabilitar a exibição da área de proteção de hardware.</span><span class="sxs-lookup"><span data-stu-id="1952d-494">Used to disable the display of the hardware protection area.</span></span>|
|<span data-ttu-id="1952d-495">defenderSecurityCenterDisableRansomwareUI</span><span class="sxs-lookup"><span data-stu-id="1952d-495">defenderSecurityCenterDisableRansomwareUI</span></span>|<span data-ttu-id="1952d-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-496">Boolean</span></span>|<span data-ttu-id="1952d-497">Usada para desabilitar a exibição da área de proteção do ransomware.</span><span class="sxs-lookup"><span data-stu-id="1952d-497">Used to disable the display of the ransomware protection area.</span></span> |
|<span data-ttu-id="1952d-498">defenderSecurityCenterDisableSecureBootUI</span><span class="sxs-lookup"><span data-stu-id="1952d-498">defenderSecurityCenterDisableSecureBootUI</span></span>|<span data-ttu-id="1952d-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-499">Boolean</span></span>|<span data-ttu-id="1952d-500">Usada para desabilitar a exibição da área de inicialização segura em segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1952d-500">Used to disable the display of the secure boot area under Device security.</span></span>|
|<span data-ttu-id="1952d-501">defenderSecurityCenterDisableTroubleshootingUI</span><span class="sxs-lookup"><span data-stu-id="1952d-501">defenderSecurityCenterDisableTroubleshootingUI</span></span>|<span data-ttu-id="1952d-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-502">Boolean</span></span>|<span data-ttu-id="1952d-503">Usada para desabilitar a exibição do processo de segurança, a solução de problemas em segurança de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1952d-503">Used to disable the display of the security process troubleshooting under Device security.</span></span>|
|<span data-ttu-id="1952d-504">defenderSecurityCenterOrganizationDisplayName</span><span class="sxs-lookup"><span data-stu-id="1952d-504">defenderSecurityCenterOrganizationDisplayName</span></span>|<span data-ttu-id="1952d-505">String</span><span class="sxs-lookup"><span data-stu-id="1952d-505">String</span></span>|<span data-ttu-id="1952d-506">O nome de empresa que é exibido para os usuários.</span><span class="sxs-lookup"><span data-stu-id="1952d-506">The company name that is displayed to the users.</span></span>|
|<span data-ttu-id="1952d-507">defenderSecurityCenterHelpEmail</span><span class="sxs-lookup"><span data-stu-id="1952d-507">defenderSecurityCenterHelpEmail</span></span>|<span data-ttu-id="1952d-508">String</span><span class="sxs-lookup"><span data-stu-id="1952d-508">String</span></span>|<span data-ttu-id="1952d-509">O endereço de email que será exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="1952d-509">The email address that is displayed to users.</span></span>|
|<span data-ttu-id="1952d-510">defenderSecurityCenterHelpPhone</span><span class="sxs-lookup"><span data-stu-id="1952d-510">defenderSecurityCenterHelpPhone</span></span>|<span data-ttu-id="1952d-511">String</span><span class="sxs-lookup"><span data-stu-id="1952d-511">String</span></span>|<span data-ttu-id="1952d-512">O número de telefone ou o ID do Skype que será exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="1952d-512">The phone number or Skype ID that is displayed to users.</span></span>|
|<span data-ttu-id="1952d-513">defenderSecurityCenterHelpURL</span><span class="sxs-lookup"><span data-stu-id="1952d-513">defenderSecurityCenterHelpURL</span></span>|<span data-ttu-id="1952d-514">String</span><span class="sxs-lookup"><span data-stu-id="1952d-514">String</span></span>|<span data-ttu-id="1952d-515">Portal da Ajuda URL isso será exibido aos usuários.</span><span class="sxs-lookup"><span data-stu-id="1952d-515">The help portal URL this is displayed to users.</span></span>|
|<span data-ttu-id="1952d-516">defenderSecurityCenterNotificationsFromApp</span><span class="sxs-lookup"><span data-stu-id="1952d-516">defenderSecurityCenterNotificationsFromApp</span></span>|[<span data-ttu-id="1952d-517">defenderSecurityCenterNotificationsFromAppType</span><span class="sxs-lookup"><span data-stu-id="1952d-517">defenderSecurityCenterNotificationsFromAppType</span></span>](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|<span data-ttu-id="1952d-518">Notificações para mostrar de exibido áreas de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1952d-518">Notifications to show from the displayed areas of app.</span></span> <span data-ttu-id="1952d-519">Os valores possíveis são: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span><span class="sxs-lookup"><span data-stu-id="1952d-519">Possible values are: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.</span></span>|
|<span data-ttu-id="1952d-520">defenderSecurityCenterITContactDisplay</span><span class="sxs-lookup"><span data-stu-id="1952d-520">defenderSecurityCenterITContactDisplay</span></span>|[<span data-ttu-id="1952d-521">defenderSecurityCenterITContactDisplayType</span><span class="sxs-lookup"><span data-stu-id="1952d-521">defenderSecurityCenterITContactDisplayType</span></span>](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|<span data-ttu-id="1952d-522">Configurar onde exibir contato de TI informações aos usuários finais.</span><span class="sxs-lookup"><span data-stu-id="1952d-522">Configure where to display IT contact information to end users.</span></span> <span data-ttu-id="1952d-523">Os valores possíveis são: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span><span class="sxs-lookup"><span data-stu-id="1952d-523">Possible values are: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.</span></span>|
|<span data-ttu-id="1952d-524">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="1952d-524">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="1952d-525">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-525">Boolean</span></span>|<span data-ttu-id="1952d-526">Bloqueia conexões de FTP com estado ao dispositivo</span><span class="sxs-lookup"><span data-stu-id="1952d-526">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="1952d-527">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="1952d-527">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="1952d-528">Int32</span><span class="sxs-lookup"><span data-stu-id="1952d-528">Int32</span></span>|<span data-ttu-id="1952d-529">Configura o tempo limite ocioso das associações de segurança, em segundos, de 300 para 3.600, inclusive.</span><span class="sxs-lookup"><span data-stu-id="1952d-529">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="1952d-530">Após esse período, as associações de segurança expirarão e serão excluídas.</span><span class="sxs-lookup"><span data-stu-id="1952d-530">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="1952d-531">Valores válidos de 300 a 3.600</span><span class="sxs-lookup"><span data-stu-id="1952d-531">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="1952d-532">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="1952d-532">firewallPreSharedKeyEncodingMethod</span></span>|[<span data-ttu-id="1952d-533">firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="1952d-533">firewallPreSharedKeyEncodingMethodType</span></span>](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|<span data-ttu-id="1952d-534">Selecione a chave pré compartilhada codificação a ser usada.</span><span class="sxs-lookup"><span data-stu-id="1952d-534">Select the preshared key encoding to be used.</span></span> <span data-ttu-id="1952d-535">Os valores possíveis são: `deviceDefault`, `none`, `utF8`.</span><span class="sxs-lookup"><span data-stu-id="1952d-535">Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="1952d-536">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="1952d-536">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="1952d-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-537">Boolean</span></span>|<span data-ttu-id="1952d-538">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de vizinhos</span><span class="sxs-lookup"><span data-stu-id="1952d-538">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="1952d-539">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="1952d-539">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="1952d-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-540">Boolean</span></span>|<span data-ttu-id="1952d-541">Configura isenções IPSec para permitir ICMP</span><span class="sxs-lookup"><span data-stu-id="1952d-541">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="1952d-542">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="1952d-542">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="1952d-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-543">Boolean</span></span>|<span data-ttu-id="1952d-544">Configura isenções IPSec para permitir códigos do tipo ICMP IPv6 de descoberta de roteadores</span><span class="sxs-lookup"><span data-stu-id="1952d-544">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="1952d-545">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="1952d-545">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="1952d-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-546">Boolean</span></span>|<span data-ttu-id="1952d-547">Configura isenções IPSec para permitir tráfego DHCP de IPv4 e IPv6</span><span class="sxs-lookup"><span data-stu-id="1952d-547">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="1952d-548">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="1952d-548">firewallCertificateRevocationListCheckMethod</span></span>|[<span data-ttu-id="1952d-549">firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="1952d-549">firewallCertificateRevocationListCheckMethodType</span></span>](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|<span data-ttu-id="1952d-550">Especifique como a lista de revogação de certificado deve ser impostas.</span><span class="sxs-lookup"><span data-stu-id="1952d-550">Specify how the certificate revocation list is to be enforced.</span></span> <span data-ttu-id="1952d-551">Os valores possíveis são: `deviceDefault`, `none`, `attempt`, `require`.</span><span class="sxs-lookup"><span data-stu-id="1952d-551">Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="1952d-552">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="1952d-552">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="1952d-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-553">Boolean</span></span>|<span data-ttu-id="1952d-554">Se um conjunto de autenticação não for totalmente suportado por um módulo de chave, direcione o módulo para ignorar apenas pacotes de autenticação não compatíveis, em vez de todo o conjunto</span><span class="sxs-lookup"><span data-stu-id="1952d-554">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="1952d-555">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="1952d-555">firewallPacketQueueingMethod</span></span>|[<span data-ttu-id="1952d-556">firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="1952d-556">firewallPacketQueueingMethodType</span></span>](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|<span data-ttu-id="1952d-557">Configura como queueing pacotes deve ser aplicada no cenário túnel gateway.</span><span class="sxs-lookup"><span data-stu-id="1952d-557">Configures how packet queueing should be applied in the tunnel gateway scenario.</span></span> <span data-ttu-id="1952d-558">Os valores possíveis são: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span><span class="sxs-lookup"><span data-stu-id="1952d-558">Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="1952d-559">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="1952d-559">firewallProfileDomain</span></span>|[<span data-ttu-id="1952d-560">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1952d-560">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="1952d-561">Define as configurações de perfil de firewall das redes do domínio</span><span class="sxs-lookup"><span data-stu-id="1952d-561">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="1952d-562">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="1952d-562">firewallProfilePublic</span></span>|[<span data-ttu-id="1952d-563">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1952d-563">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="1952d-564">Define as configurações de perfil de firewall das redes públicas</span><span class="sxs-lookup"><span data-stu-id="1952d-564">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="1952d-565">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="1952d-565">firewallProfilePrivate</span></span>|[<span data-ttu-id="1952d-566">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1952d-566">windowsFirewallNetworkProfile</span></span>](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|<span data-ttu-id="1952d-567">Define as configurações de perfil de firewall das redes privadas</span><span class="sxs-lookup"><span data-stu-id="1952d-567">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="1952d-568">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="1952d-568">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="1952d-569">String collection</span><span class="sxs-lookup"><span data-stu-id="1952d-569">String collection</span></span>|<span data-ttu-id="1952d-570">Lista de arquivos executáveis e pastas a serem excluídos das regras de redução de superfície de ataque</span><span class="sxs-lookup"><span data-stu-id="1952d-570">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="1952d-571">defenderOfficeAppsOtherProcessInjectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-571">defenderOfficeAppsOtherProcessInjectionType</span></span>|[<span data-ttu-id="1952d-572">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1952d-572">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1952d-573">Valor que indica o comportamento dos aplicativos do Office injeção aos outros processos.</span><span class="sxs-lookup"><span data-stu-id="1952d-573">Value indicating the behavior of Office applications injecting into other processes.</span></span> <span data-ttu-id="1952d-574">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-574">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-575">defenderOfficeAppsOtherProcessInjection</span><span class="sxs-lookup"><span data-stu-id="1952d-575">defenderOfficeAppsOtherProcessInjection</span></span>|[<span data-ttu-id="1952d-576">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-576">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-577">Valor que indica o comportamento dos aplicativos do Office injeção aos outros processos.</span><span class="sxs-lookup"><span data-stu-id="1952d-577">Value indicating the behavior of  Office applications injecting into other processes.</span></span> <span data-ttu-id="1952d-578">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-578">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-579">defenderOfficeAppsExecutableContentCreationOrLaunchType</span><span class="sxs-lookup"><span data-stu-id="1952d-579">defenderOfficeAppsExecutableContentCreationOrLaunchType</span></span>|[<span data-ttu-id="1952d-580">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1952d-580">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1952d-581">Valor que indica o comportamento de macros aplicativos/Office criando ou launching conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="1952d-581">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="1952d-582">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-582">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-583">defenderOfficeAppsExecutableContentCreationOrLaunch</span><span class="sxs-lookup"><span data-stu-id="1952d-583">defenderOfficeAppsExecutableContentCreationOrLaunch</span></span>|[<span data-ttu-id="1952d-584">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-584">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-585">Valor que indica o comportamento de macros aplicativos/Office criando ou launching conteúdo executável.</span><span class="sxs-lookup"><span data-stu-id="1952d-585">Value indicating the behavior of Office applications/macros creating or launching executable content.</span></span> <span data-ttu-id="1952d-586">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-586">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-587">defenderOfficeAppsLaunchChildProcessType</span><span class="sxs-lookup"><span data-stu-id="1952d-587">defenderOfficeAppsLaunchChildProcessType</span></span>|[<span data-ttu-id="1952d-588">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1952d-588">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1952d-589">Valor que indica o comportamento do aplicativo Office launching processos filho.</span><span class="sxs-lookup"><span data-stu-id="1952d-589">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="1952d-590">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-590">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-591">defenderOfficeAppsLaunchChildProcess</span><span class="sxs-lookup"><span data-stu-id="1952d-591">defenderOfficeAppsLaunchChildProcess</span></span>|[<span data-ttu-id="1952d-592">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-592">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-593">Valor que indica o comportamento do aplicativo Office launching processos filho.</span><span class="sxs-lookup"><span data-stu-id="1952d-593">Value indicating the behavior of Office application launching child processes.</span></span> <span data-ttu-id="1952d-594">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-594">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-595">defenderOfficeMacroCodeAllowWin32ImportsType</span><span class="sxs-lookup"><span data-stu-id="1952d-595">defenderOfficeMacroCodeAllowWin32ImportsType</span></span>|[<span data-ttu-id="1952d-596">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1952d-596">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1952d-597">O valor que indica que o comportamento do Win32 importa do código de Macro no Office.</span><span class="sxs-lookup"><span data-stu-id="1952d-597">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="1952d-598">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-598">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-599">defenderOfficeMacroCodeAllowWin32Imports</span><span class="sxs-lookup"><span data-stu-id="1952d-599">defenderOfficeMacroCodeAllowWin32Imports</span></span>|[<span data-ttu-id="1952d-600">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-600">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-601">O valor que indica que o comportamento do Win32 importa do código de Macro no Office.</span><span class="sxs-lookup"><span data-stu-id="1952d-601">Value indicating the behavior of Win32 imports from Macro code in Office.</span></span> <span data-ttu-id="1952d-602">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-602">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-603">defenderScriptObfuscatedMacroCodeType</span><span class="sxs-lookup"><span data-stu-id="1952d-603">defenderScriptObfuscatedMacroCodeType</span></span>|[<span data-ttu-id="1952d-604">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1952d-604">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1952d-605">Valor que indica o comportamento do código de js/vbs/ps/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="1952d-605">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="1952d-606">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-606">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-607">defenderScriptObfuscatedMacroCode</span><span class="sxs-lookup"><span data-stu-id="1952d-607">defenderScriptObfuscatedMacroCode</span></span>|[<span data-ttu-id="1952d-608">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-608">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-609">Valor que indica o comportamento do código de js/vbs/ps/macro ofuscado.</span><span class="sxs-lookup"><span data-stu-id="1952d-609">Value indicating the behavior of obfuscated js/vbs/ps/macro code.</span></span> <span data-ttu-id="1952d-610">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-610">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-611">defenderScriptDownloadedPayloadExecutionType</span><span class="sxs-lookup"><span data-stu-id="1952d-611">defenderScriptDownloadedPayloadExecutionType</span></span>|[<span data-ttu-id="1952d-612">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1952d-612">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1952d-613">Valor que indica o comportamento do js/vbs executá-lo carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="1952d-613">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="1952d-614">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-614">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-615">defenderScriptDownloadedPayloadExecution</span><span class="sxs-lookup"><span data-stu-id="1952d-615">defenderScriptDownloadedPayloadExecution</span></span>|[<span data-ttu-id="1952d-616">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-616">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-617">Valor que indica o comportamento do js/vbs executá-lo carga baixada da Internet.</span><span class="sxs-lookup"><span data-stu-id="1952d-617">Value indicating the behavior of js/vbs executing payload downloaded from Internet.</span></span> <span data-ttu-id="1952d-618">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-618">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-619">defenderPreventCredentialStealingType</span><span class="sxs-lookup"><span data-stu-id="1952d-619">defenderPreventCredentialStealingType</span></span>|[<span data-ttu-id="1952d-620">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-620">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-621">Valor que indica se a credencial roubar do subsistema de autoridade de segurança local do Windows será permitida.</span><span class="sxs-lookup"><span data-stu-id="1952d-621">Value indicating if credential stealing from the Windows local security authority subsystem is permitted.</span></span> <span data-ttu-id="1952d-622">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-622">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-623">defenderProcessCreationType</span><span class="sxs-lookup"><span data-stu-id="1952d-623">defenderProcessCreationType</span></span>|[<span data-ttu-id="1952d-624">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1952d-624">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1952d-625">O valor de resposta indica a criações de processo provenientes de comandos PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="1952d-625">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="1952d-626">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-626">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-627">defenderProcessCreation</span><span class="sxs-lookup"><span data-stu-id="1952d-627">defenderProcessCreation</span></span>|[<span data-ttu-id="1952d-628">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-628">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-629">O valor de resposta indica a criações de processo provenientes de comandos PSExec e WMI.</span><span class="sxs-lookup"><span data-stu-id="1952d-629">Value indicating response to process creations originating from PSExec and WMI commands.</span></span> <span data-ttu-id="1952d-630">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-630">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-631">defenderUntrustedUSBProcessType</span><span class="sxs-lookup"><span data-stu-id="1952d-631">defenderUntrustedUSBProcessType</span></span>|[<span data-ttu-id="1952d-632">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1952d-632">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1952d-633">Valor que indica a resposta para processos assinados e não confiáveis que executam o USB.</span><span class="sxs-lookup"><span data-stu-id="1952d-633">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="1952d-634">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-634">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-635">defenderUntrustedUSBProcess</span><span class="sxs-lookup"><span data-stu-id="1952d-635">defenderUntrustedUSBProcess</span></span>|[<span data-ttu-id="1952d-636">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-636">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-637">Valor que indica a resposta para processos assinados e não confiáveis que executam o USB.</span><span class="sxs-lookup"><span data-stu-id="1952d-637">Value indicating response to untrusted and unsigned processes that run from USB.</span></span> <span data-ttu-id="1952d-638">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-638">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-639">defenderUntrustedExecutableType</span><span class="sxs-lookup"><span data-stu-id="1952d-639">defenderUntrustedExecutableType</span></span>|[<span data-ttu-id="1952d-640">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1952d-640">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1952d-641">Valor que indica a resposta para executáveis que não atendem a uma chamadas, idade ou lista de confiável critérios.</span><span class="sxs-lookup"><span data-stu-id="1952d-641">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="1952d-642">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-642">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-643">defenderUntrustedExecutable</span><span class="sxs-lookup"><span data-stu-id="1952d-643">defenderUntrustedExecutable</span></span>|[<span data-ttu-id="1952d-644">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-644">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-645">Valor que indica a resposta para executáveis que não atendem a uma chamadas, idade ou lista de confiável critérios.</span><span class="sxs-lookup"><span data-stu-id="1952d-645">Value indicating response to executables that don't meet a prevalence, age, or trusted list criteria.</span></span> <span data-ttu-id="1952d-646">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-646">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-647">defenderEmailContentExecutionType</span><span class="sxs-lookup"><span data-stu-id="1952d-647">defenderEmailContentExecutionType</span></span>|[<span data-ttu-id="1952d-648">defenderAttackSurfaceType</span><span class="sxs-lookup"><span data-stu-id="1952d-648">defenderAttackSurfaceType</span></span>](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|<span data-ttu-id="1952d-649">Valor que indica se a execução de conteúdo executável (exe, dll, ps, js, vbs, etc.) deve ser retirada da email (email/webmail-cliente).</span><span class="sxs-lookup"><span data-stu-id="1952d-649">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="1952d-650">Os valores possíveis são: `userDefined`, `block`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-650">Possible values are: `userDefined`, `block`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-651">defenderEmailContentExecution</span><span class="sxs-lookup"><span data-stu-id="1952d-651">defenderEmailContentExecution</span></span>|[<span data-ttu-id="1952d-652">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-652">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-653">Valor que indica se a execução de conteúdo executável (exe, dll, ps, js, vbs, etc.) deve ser retirada da email (email/webmail-cliente).</span><span class="sxs-lookup"><span data-stu-id="1952d-653">Value indicating if execution of executable content (exe, dll, ps, js, vbs, etc) should be dropped from email (webmail/mail-client).</span></span> <span data-ttu-id="1952d-654">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-654">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-655">defenderAdvancedRansomewareProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-655">defenderAdvancedRansomewareProtectionType</span></span>|[<span data-ttu-id="1952d-656">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-656">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-657">Valor que indica o uso de proteção avançada contra ransomeware.</span><span class="sxs-lookup"><span data-stu-id="1952d-657">Value indicating use of advanced protection against ransomeware.</span></span> <span data-ttu-id="1952d-658">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-658">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-659">defenderGuardMyFoldersType</span><span class="sxs-lookup"><span data-stu-id="1952d-659">defenderGuardMyFoldersType</span></span>|[<span data-ttu-id="1952d-660">folderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-660">folderProtectionType</span></span>](../resources/intune-deviceconfig-folderprotectiontype.md)|<span data-ttu-id="1952d-661">Valor que indica o comportamento de pastas protegidas.</span><span class="sxs-lookup"><span data-stu-id="1952d-661">Value indicating the behavior of protected folders.</span></span> <span data-ttu-id="1952d-662">Os valores possíveis são: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span><span class="sxs-lookup"><span data-stu-id="1952d-662">Possible values are: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.</span></span>|
|<span data-ttu-id="1952d-663">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="1952d-663">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="1952d-664">String collection</span><span class="sxs-lookup"><span data-stu-id="1952d-664">String collection</span></span>|<span data-ttu-id="1952d-665">Lista de caminhos para execução com permissão para acessar as pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="1952d-665">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="1952d-666">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="1952d-666">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="1952d-667">String collection</span><span class="sxs-lookup"><span data-stu-id="1952d-667">String collection</span></span>|<span data-ttu-id="1952d-668">Lista de caminhos de pasta a serem adicionados à lista de pastas protegidas</span><span class="sxs-lookup"><span data-stu-id="1952d-668">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="1952d-669">defenderNetworkProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-669">defenderNetworkProtectionType</span></span>|[<span data-ttu-id="1952d-670">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="1952d-670">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="1952d-671">Valor que indica o comportamento do NetworkProtection.</span><span class="sxs-lookup"><span data-stu-id="1952d-671">Value indicating the behavior of NetworkProtection.</span></span> <span data-ttu-id="1952d-672">Os valores possíveis são: `userDefined`, `enable`, `auditMode`.</span><span class="sxs-lookup"><span data-stu-id="1952d-672">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="1952d-673">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="1952d-673">defenderExploitProtectionXml</span></span>|<span data-ttu-id="1952d-674">Binária</span><span class="sxs-lookup"><span data-stu-id="1952d-674">Binary</span></span>|<span data-ttu-id="1952d-675">Conteúdo XML com informações sobre a proteção contra vulnerabilidades.</span><span class="sxs-lookup"><span data-stu-id="1952d-675">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="1952d-676">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="1952d-676">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="1952d-677">String</span><span class="sxs-lookup"><span data-stu-id="1952d-677">String</span></span>|<span data-ttu-id="1952d-678">Nome do arquivo do qual DefenderExploitProtectionXml foi obtido.</span><span class="sxs-lookup"><span data-stu-id="1952d-678">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="1952d-679">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="1952d-679">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="1952d-680">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-680">Boolean</span></span>|<span data-ttu-id="1952d-681">Indica se o usuário será ou não impedido de substituir as configurações de Exploit Protection.</span><span class="sxs-lookup"><span data-stu-id="1952d-681">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="1952d-682">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="1952d-682">appLockerApplicationControl</span></span>|[<span data-ttu-id="1952d-683">appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="1952d-683">appLockerApplicationControlType</span></span>](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|<span data-ttu-id="1952d-684">Permite que o administrador escolha quais tipos de aplicativo permitir nos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1952d-684">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="1952d-685">Os valores possíveis são: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span><span class="sxs-lookup"><span data-stu-id="1952d-685">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="1952d-686">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span><span class="sxs-lookup"><span data-stu-id="1952d-686">deviceGuardLocalSystemAuthorityCredentialGuardSettings</span></span>|[<span data-ttu-id="1952d-687">deviceGuardLocalSystemAuthorityCredentialGuardType</span><span class="sxs-lookup"><span data-stu-id="1952d-687">deviceGuardLocalSystemAuthorityCredentialGuardType</span></span>](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|<span data-ttu-id="1952d-688">Ative o protetor de credencial quando o nível de segurança de plataforma com inicialização seguro e virtualização com base em segurança estão habilitadas.</span><span class="sxs-lookup"><span data-stu-id="1952d-688">Turn on Credential Guard when Platform Security Level with Secure Boot and Virtualization Based Security are both enabled.</span></span> <span data-ttu-id="1952d-689">Os valores possíveis são: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span><span class="sxs-lookup"><span data-stu-id="1952d-689">Possible values are: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.</span></span>|
|<span data-ttu-id="1952d-690">deviceGuardEnableVirtualizationBasedSecurity</span><span class="sxs-lookup"><span data-stu-id="1952d-690">deviceGuardEnableVirtualizationBasedSecurity</span></span>|<span data-ttu-id="1952d-691">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-691">Boolean</span></span>|<span data-ttu-id="1952d-692">Ativa as teclas de virtualização com base em Security(VBS).</span><span class="sxs-lookup"><span data-stu-id="1952d-692">Turns On Virtualization Based Security(VBS).</span></span>|
|<span data-ttu-id="1952d-693">deviceGuardEnableSecureBootWithDMA</span><span class="sxs-lookup"><span data-stu-id="1952d-693">deviceGuardEnableSecureBootWithDMA</span></span>|<span data-ttu-id="1952d-694">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-694">Boolean</span></span>|<span data-ttu-id="1952d-695">Especifica se o nível de segurança de plataforma está habilitado na próxima reinicialização.</span><span class="sxs-lookup"><span data-stu-id="1952d-695">Specifies whether Platform Security Level is enabled at next reboot.</span></span>|
|<span data-ttu-id="1952d-696">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="1952d-696">smartScreenEnableInShell</span></span>|<span data-ttu-id="1952d-697">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-697">Boolean</span></span>|<span data-ttu-id="1952d-698">Permite que os administradores de TI configurem SmartScreen para Windows.</span><span class="sxs-lookup"><span data-stu-id="1952d-698">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="1952d-699">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="1952d-699">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="1952d-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-700">Boolean</span></span>|<span data-ttu-id="1952d-701">Permite que administradores de TI controlem se os usuários podem ignorar avisos do SmartScreen e executar arquivos maliciosos.</span><span class="sxs-lookup"><span data-stu-id="1952d-701">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="1952d-702">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="1952d-702">applicationGuardEnabled</span></span>|<span data-ttu-id="1952d-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-703">Boolean</span></span>|<span data-ttu-id="1952d-704">Habilitar o Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="1952d-704">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="1952d-705">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="1952d-705">applicationGuardEnabledOptions</span></span>|[<span data-ttu-id="1952d-706">applicationGuardEnabledOptions</span><span class="sxs-lookup"><span data-stu-id="1952d-706">applicationGuardEnabledOptions</span></span>](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|<span data-ttu-id="1952d-707">Habilite o protetor de aplicativo do Windows Defender para versões mais recentes do Windows.</span><span class="sxs-lookup"><span data-stu-id="1952d-707">Enable Windows Defender Application Guard for newer Windows builds.</span></span> <span data-ttu-id="1952d-708">Os valores possíveis são: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span><span class="sxs-lookup"><span data-stu-id="1952d-708">Possible values are: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.</span></span>|
|<span data-ttu-id="1952d-709">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="1952d-709">applicationGuardBlockFileTransfer</span></span>|[<span data-ttu-id="1952d-710">applicationGuardBlockFileTransferType</span><span class="sxs-lookup"><span data-stu-id="1952d-710">applicationGuardBlockFileTransferType</span></span>](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|<span data-ttu-id="1952d-711">Área de transferência de bloqueio para um arquivo de imagem de transferência, arquivo de texto ou nenhum deles.</span><span class="sxs-lookup"><span data-stu-id="1952d-711">Block clipboard to transfer image file, text file or neither of them.</span></span> <span data-ttu-id="1952d-712">Os valores possíveis são: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span><span class="sxs-lookup"><span data-stu-id="1952d-712">Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="1952d-713">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="1952d-713">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="1952d-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-714">Boolean</span></span>|<span data-ttu-id="1952d-715">Impedir sites corporativos de carregar conteúdos que não sejam da empresa, como plug-ins de terceiros</span><span class="sxs-lookup"><span data-stu-id="1952d-715">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="1952d-716">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="1952d-716">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="1952d-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-717">Boolean</span></span>|<span data-ttu-id="1952d-718">Permitir dados persistentes gerados por usuários dentro do contêiner do App Guard (favoritos, cookies, senhas da Web, etc.)</span><span class="sxs-lookup"><span data-stu-id="1952d-718">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="1952d-719">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="1952d-719">applicationGuardForceAuditing</span></span>|<span data-ttu-id="1952d-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-720">Boolean</span></span>|<span data-ttu-id="1952d-721">A auditoria forçada manterá logs e eventos do Windows para atender aos critérios de segurança/conformidade (exemplos de evento são logon e logoff do usuário, uso de direitos de privilégios, instalação de software, as alterações do sistema, etc.)
</span><span class="sxs-lookup"><span data-stu-id="1952d-721">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="1952d-722">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="1952d-722">applicationGuardBlockClipboardSharing</span></span>|[<span data-ttu-id="1952d-723">applicationGuardBlockClipboardSharingType</span><span class="sxs-lookup"><span data-stu-id="1952d-723">applicationGuardBlockClipboardSharingType</span></span>](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|<span data-ttu-id="1952d-724">Impedir a área de transferência de compartilhar dados do Host para o Contêiner, do Contêiner para o Host ou em ambas as direções.</span><span class="sxs-lookup"><span data-stu-id="1952d-724">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="1952d-725">Os valores possíveis são: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span><span class="sxs-lookup"><span data-stu-id="1952d-725">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="1952d-726">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="1952d-726">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="1952d-727">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-727">Boolean</span></span>|<span data-ttu-id="1952d-728">Permitir a impressão em PDF pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="1952d-728">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="1952d-729">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="1952d-729">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="1952d-730">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-730">Boolean</span></span>|<span data-ttu-id="1952d-731">Permitir a impressão em XPS pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="1952d-731">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="1952d-732">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="1952d-732">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="1952d-733">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-733">Boolean</span></span>|<span data-ttu-id="1952d-734">Permitir a impressão em Impressoras Locais pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="1952d-734">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="1952d-735">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="1952d-735">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="1952d-736">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-736">Boolean</span></span>|<span data-ttu-id="1952d-737">Permitir a impressão em Impressoras da Rede pelo contêiner</span><span class="sxs-lookup"><span data-stu-id="1952d-737">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="1952d-738">applicationGuardAllowVirtualGPU</span><span class="sxs-lookup"><span data-stu-id="1952d-738">applicationGuardAllowVirtualGPU</span></span>|<span data-ttu-id="1952d-739">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-739">Boolean</span></span>|<span data-ttu-id="1952d-740">Permitir guard aplicativo usar GPU virtual</span><span class="sxs-lookup"><span data-stu-id="1952d-740">Allow application guard to use virtual GPU</span></span>|
|<span data-ttu-id="1952d-741">applicationGuardAllowFileSaveOnHost</span><span class="sxs-lookup"><span data-stu-id="1952d-741">applicationGuardAllowFileSaveOnHost</span></span>|<span data-ttu-id="1952d-742">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-742">Boolean</span></span>|<span data-ttu-id="1952d-743">Permitir que os usuários baixem arquivos de borda no contêiner do protetor de aplicativo e salvá-los no host do sistema de arquivos</span><span class="sxs-lookup"><span data-stu-id="1952d-743">Allow users to download files from Edge in the application guard container and save them on the host file system</span></span>|
|<span data-ttu-id="1952d-744">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="1952d-744">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="1952d-745">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-745">Boolean</span></span>|<span data-ttu-id="1952d-746">Permite que o administrador desabilite o aviso de outras criptografias de disco nas máquinas dos usuários.</span><span class="sxs-lookup"><span data-stu-id="1952d-746">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="1952d-747">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="1952d-747">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="1952d-748">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-748">Boolean</span></span>|<span data-ttu-id="1952d-749">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="1952d-749">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="1952d-750">Essa política é válida apenas para uma SKU móvel.</span><span class="sxs-lookup"><span data-stu-id="1952d-750">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="1952d-751">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="1952d-751">bitLockerEncryptDevice</span></span>|<span data-ttu-id="1952d-752">Boolean</span><span class="sxs-lookup"><span data-stu-id="1952d-752">Boolean</span></span>|<span data-ttu-id="1952d-753">Permite que o administrador exija que a criptografia seja ativada usando BitLocker.</span><span class="sxs-lookup"><span data-stu-id="1952d-753">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="1952d-754">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1952d-754">bitLockerSystemDrivePolicy</span></span>|[<span data-ttu-id="1952d-755">bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1952d-755">bitLockerSystemDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|<span data-ttu-id="1952d-756">Política de unidade de disco BitLocker sistema.</span><span class="sxs-lookup"><span data-stu-id="1952d-756">BitLocker System Drive Policy.</span></span>|
|<span data-ttu-id="1952d-757">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1952d-757">bitLockerFixedDrivePolicy</span></span>|[<span data-ttu-id="1952d-758">bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1952d-758">bitLockerFixedDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md)|<span data-ttu-id="1952d-759">O BitLocker fixa direcionar a política.</span><span class="sxs-lookup"><span data-stu-id="1952d-759">BitLocker Fixed Drive Policy.</span></span>|
|<span data-ttu-id="1952d-760">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1952d-760">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="1952d-761">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1952d-761">bitLockerRemovableDrivePolicy</span></span>](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|<span data-ttu-id="1952d-762">Política da unidade removível do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="1952d-762">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="1952d-763">Resposta</span><span class="sxs-lookup"><span data-stu-id="1952d-763">Response</span></span>
<span data-ttu-id="1952d-764">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1952d-764">If successful, this method returns a `201 Created` response code and a [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1952d-765">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1952d-765">Example</span></span>
### <a name="request"></a><span data-ttu-id="1952d-766">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1952d-766">Request</span></span>
<span data-ttu-id="1952d-767">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1952d-767">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 26391

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
  "localSecurityOptionsEnableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsEnableGuestAccount": true,
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
  "lanManagerWorkstationEnableInsecureGuestLogons": true,
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

### <a name="response"></a><span data-ttu-id="1952d-768">Resposta</span><span class="sxs-lookup"><span data-stu-id="1952d-768">Response</span></span>
<span data-ttu-id="1952d-p194">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1952d-p194">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 26499

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
  "localSecurityOptionsEnableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "Local Security Options Administrator Account Name value",
  "localSecurityOptionsEnableGuestAccount": true,
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
  "lanManagerWorkstationEnableInsecureGuestLogons": true,
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





