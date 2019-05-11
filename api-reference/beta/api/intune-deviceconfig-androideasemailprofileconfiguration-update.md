---
title: Atualizar androidEasEmailProfileConfiguration
description: Atualiza as propriedades de um objeto androidEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1bf87238d42b9520544380225f985479e9d05bf5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933057"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="2c8da-103">Atualizar androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c8da-103">Update androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="2c8da-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2c8da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c8da-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c8da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c8da-106">Atualiza as propriedades de um objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2c8da-106">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c8da-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2c8da-107">Prerequisites</span></span>
<span data-ttu-id="2c8da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c8da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c8da-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c8da-110">Permission type</span></span>|<span data-ttu-id="2c8da-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2c8da-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c8da-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c8da-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2c8da-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c8da-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2c8da-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c8da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c8da-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c8da-115">Not supported.</span></span>|
|<span data-ttu-id="2c8da-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c8da-116">Application</span></span>|<span data-ttu-id="2c8da-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c8da-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c8da-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c8da-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2c8da-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c8da-119">Request headers</span></span>
|<span data-ttu-id="2c8da-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c8da-120">Header</span></span>|<span data-ttu-id="2c8da-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2c8da-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2c8da-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c8da-122">Authorization</span></span>|<span data-ttu-id="2c8da-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c8da-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2c8da-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2c8da-124">Accept</span></span>|<span data-ttu-id="2c8da-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2c8da-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c8da-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c8da-126">Request body</span></span>
<span data-ttu-id="2c8da-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2c8da-127">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="2c8da-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2c8da-128">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="2c8da-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c8da-129">Property</span></span>|<span data-ttu-id="2c8da-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c8da-130">Type</span></span>|<span data-ttu-id="2c8da-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c8da-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c8da-132">id</span><span class="sxs-lookup"><span data-stu-id="2c8da-132">id</span></span>|<span data-ttu-id="2c8da-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c8da-133">String</span></span>|<span data-ttu-id="2c8da-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2c8da-134">Key of the entity.</span></span> <span data-ttu-id="2c8da-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c8da-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c8da-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c8da-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2c8da-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c8da-137">DateTimeOffset</span></span>|<span data-ttu-id="2c8da-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2c8da-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2c8da-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c8da-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c8da-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2c8da-140">roleScopeTagIds</span></span>|<span data-ttu-id="2c8da-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c8da-141">String collection</span></span>|<span data-ttu-id="2c8da-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2c8da-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2c8da-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c8da-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c8da-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2c8da-144">supportsScopeTags</span></span>|<span data-ttu-id="2c8da-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="2c8da-145">Boolean</span></span>|<span data-ttu-id="2c8da-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2c8da-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2c8da-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="2c8da-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2c8da-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c8da-149">This property is read-only.</span></span> <span data-ttu-id="2c8da-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c8da-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c8da-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2c8da-151">createdDateTime</span></span>|<span data-ttu-id="2c8da-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2c8da-152">DateTimeOffset</span></span>|<span data-ttu-id="2c8da-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2c8da-153">DateTime the object was created.</span></span> <span data-ttu-id="2c8da-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c8da-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c8da-155">description</span><span class="sxs-lookup"><span data-stu-id="2c8da-155">description</span></span>|<span data-ttu-id="2c8da-156">String</span><span class="sxs-lookup"><span data-stu-id="2c8da-156">String</span></span>|<span data-ttu-id="2c8da-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2c8da-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c8da-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c8da-159">displayName</span><span class="sxs-lookup"><span data-stu-id="2c8da-159">displayName</span></span>|<span data-ttu-id="2c8da-160">String</span><span class="sxs-lookup"><span data-stu-id="2c8da-160">String</span></span>|<span data-ttu-id="2c8da-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2c8da-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c8da-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c8da-163">versão</span><span class="sxs-lookup"><span data-stu-id="2c8da-163">version</span></span>|<span data-ttu-id="2c8da-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2c8da-164">Int32</span></span>|<span data-ttu-id="2c8da-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-165">Version of the device configuration.</span></span> <span data-ttu-id="2c8da-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2c8da-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2c8da-167">accountName</span><span class="sxs-lookup"><span data-stu-id="2c8da-167">accountName</span></span>|<span data-ttu-id="2c8da-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c8da-168">String</span></span>|<span data-ttu-id="2c8da-169">Nome da conta do Exchange ActiveSync, exibido para os usuários como o nome do perfil EAS (este).</span><span class="sxs-lookup"><span data-stu-id="2c8da-169">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="2c8da-170">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2c8da-170">authenticationMethod</span></span>|[<span data-ttu-id="2c8da-171">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2c8da-171">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="2c8da-172">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="2c8da-172">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="2c8da-173">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="2c8da-173">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="2c8da-174">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="2c8da-174">syncCalendar</span></span>|<span data-ttu-id="2c8da-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="2c8da-175">Boolean</span></span>|<span data-ttu-id="2c8da-176">Alterna a sincronização do calendário.</span><span class="sxs-lookup"><span data-stu-id="2c8da-176">Toggles syncing the calendar.</span></span> <span data-ttu-id="2c8da-177">Se definido como falso, o calendário será desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-177">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="2c8da-178">syncContacts</span><span class="sxs-lookup"><span data-stu-id="2c8da-178">syncContacts</span></span>|<span data-ttu-id="2c8da-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="2c8da-179">Boolean</span></span>|<span data-ttu-id="2c8da-180">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="2c8da-180">Toggles syncing contacts.</span></span> <span data-ttu-id="2c8da-181">Se definido como falso, os contatos serão desativados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-181">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="2c8da-182">syncTasks</span><span class="sxs-lookup"><span data-stu-id="2c8da-182">syncTasks</span></span>|<span data-ttu-id="2c8da-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="2c8da-183">Boolean</span></span>|<span data-ttu-id="2c8da-184">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="2c8da-184">Toggles syncing tasks.</span></span> <span data-ttu-id="2c8da-185">Se definido como falso, as tarefas serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-185">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="2c8da-186">syncNotes</span><span class="sxs-lookup"><span data-stu-id="2c8da-186">syncNotes</span></span>|<span data-ttu-id="2c8da-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="2c8da-187">Boolean</span></span>|<span data-ttu-id="2c8da-188">Alterna a sincronização das anotações.</span><span class="sxs-lookup"><span data-stu-id="2c8da-188">Toggles syncing notes.</span></span> <span data-ttu-id="2c8da-189">Se definido como false, as anotações serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-189">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="2c8da-190">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="2c8da-190">durationOfEmailToSync</span></span>|[<span data-ttu-id="2c8da-191">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="2c8da-191">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="2c8da-192">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="2c8da-192">Duration of time email should be synced to.</span></span> <span data-ttu-id="2c8da-193">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="2c8da-193">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="2c8da-194">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="2c8da-194">emailAddressSource</span></span>|[<span data-ttu-id="2c8da-195">UserEmail</span><span class="sxs-lookup"><span data-stu-id="2c8da-195">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="2c8da-196">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-196">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2c8da-197">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="2c8da-197">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2c8da-198">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="2c8da-198">emailSyncSchedule</span></span>|[<span data-ttu-id="2c8da-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="2c8da-199">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="2c8da-200">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="2c8da-200">Email sync schedule.</span></span> <span data-ttu-id="2c8da-201">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="2c8da-201">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="2c8da-202">hostName</span><span class="sxs-lookup"><span data-stu-id="2c8da-202">hostName</span></span>|<span data-ttu-id="2c8da-203">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c8da-203">String</span></span>|<span data-ttu-id="2c8da-204">Local do Exchange (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="2c8da-204">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="2c8da-205">requireSmime</span><span class="sxs-lookup"><span data-stu-id="2c8da-205">requireSmime</span></span>|<span data-ttu-id="2c8da-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="2c8da-206">Boolean</span></span>|<span data-ttu-id="2c8da-207">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="2c8da-207">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="2c8da-208">requireSsl</span><span class="sxs-lookup"><span data-stu-id="2c8da-208">requireSsl</span></span>|<span data-ttu-id="2c8da-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="2c8da-209">Boolean</span></span>|<span data-ttu-id="2c8da-210">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="2c8da-210">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="2c8da-211">usernameSource</span><span class="sxs-lookup"><span data-stu-id="2c8da-211">usernameSource</span></span>|[<span data-ttu-id="2c8da-212">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="2c8da-212">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="2c8da-213">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-213">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2c8da-214">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="2c8da-214">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="2c8da-215">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="2c8da-215">userDomainNameSource</span></span>|[<span data-ttu-id="2c8da-216">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="2c8da-216">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="2c8da-217">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-217">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="2c8da-218">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="2c8da-218">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="2c8da-219">customDomainName</span><span class="sxs-lookup"><span data-stu-id="2c8da-219">customDomainName</span></span>|<span data-ttu-id="2c8da-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c8da-220">String</span></span>|<span data-ttu-id="2c8da-221">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2c8da-221">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="2c8da-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c8da-222">Response</span></span>
<span data-ttu-id="2c8da-223">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c8da-223">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c8da-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c8da-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c8da-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c8da-225">Request</span></span>
<span data-ttu-id="2c8da-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c8da-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 793

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="2c8da-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c8da-227">Response</span></span>
<span data-ttu-id="2c8da-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c8da-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 965

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```




