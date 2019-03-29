---
title: Criar androidEasEmailProfileConfiguration
description: Criar um novo objeto androidEasEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6288feb32a616a3ba0636ce3f6fb61a6585ad2f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964273"
---
# <a name="create-androideasemailprofileconfiguration"></a><span data-ttu-id="31d18-103">Criar androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="31d18-103">Create androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="31d18-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="31d18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31d18-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31d18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31d18-106">Criar um novo objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="31d18-106">Create a new [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31d18-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="31d18-107">Prerequisites</span></span>
<span data-ttu-id="31d18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31d18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31d18-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31d18-110">Permission type</span></span>|<span data-ttu-id="31d18-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="31d18-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31d18-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31d18-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31d18-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31d18-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31d18-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31d18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31d18-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31d18-115">Not supported.</span></span>|
|<span data-ttu-id="31d18-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31d18-116">Application</span></span>|<span data-ttu-id="31d18-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31d18-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31d18-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31d18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="31d18-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31d18-119">Request headers</span></span>
|<span data-ttu-id="31d18-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="31d18-120">Header</span></span>|<span data-ttu-id="31d18-121">Valor</span><span class="sxs-lookup"><span data-stu-id="31d18-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31d18-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="31d18-122">Authorization</span></span>|<span data-ttu-id="31d18-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31d18-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31d18-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="31d18-124">Accept</span></span>|<span data-ttu-id="31d18-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31d18-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31d18-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31d18-126">Request body</span></span>
<span data-ttu-id="31d18-127">No corpo da solicitação, forneça uma representação JSON do objeto androidEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="31d18-127">In the request body, supply a JSON representation for the androidEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="31d18-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="31d18-128">The following table shows the properties that are required when you create the androidEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="31d18-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31d18-129">Property</span></span>|<span data-ttu-id="31d18-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="31d18-130">Type</span></span>|<span data-ttu-id="31d18-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="31d18-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31d18-132">id</span><span class="sxs-lookup"><span data-stu-id="31d18-132">id</span></span>|<span data-ttu-id="31d18-133">String</span><span class="sxs-lookup"><span data-stu-id="31d18-133">String</span></span>|<span data-ttu-id="31d18-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="31d18-134">Key of the entity.</span></span> <span data-ttu-id="31d18-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31d18-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31d18-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31d18-136">lastModifiedDateTime</span></span>|<span data-ttu-id="31d18-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31d18-137">DateTimeOffset</span></span>|<span data-ttu-id="31d18-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="31d18-138">DateTime the object was last modified.</span></span> <span data-ttu-id="31d18-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31d18-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31d18-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="31d18-140">roleScopeTagIds</span></span>|<span data-ttu-id="31d18-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="31d18-141">String collection</span></span>|<span data-ttu-id="31d18-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="31d18-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="31d18-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31d18-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31d18-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="31d18-144">supportsScopeTags</span></span>|<span data-ttu-id="31d18-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="31d18-145">Boolean</span></span>|<span data-ttu-id="31d18-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="31d18-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="31d18-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="31d18-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="31d18-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="31d18-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="31d18-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31d18-149">This property is read-only.</span></span> <span data-ttu-id="31d18-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31d18-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31d18-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31d18-151">createdDateTime</span></span>|<span data-ttu-id="31d18-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31d18-152">DateTimeOffset</span></span>|<span data-ttu-id="31d18-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="31d18-153">DateTime the object was created.</span></span> <span data-ttu-id="31d18-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31d18-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31d18-155">descrição</span><span class="sxs-lookup"><span data-stu-id="31d18-155">description</span></span>|<span data-ttu-id="31d18-156">String</span><span class="sxs-lookup"><span data-stu-id="31d18-156">String</span></span>|<span data-ttu-id="31d18-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31d18-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="31d18-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31d18-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31d18-159">displayName</span><span class="sxs-lookup"><span data-stu-id="31d18-159">displayName</span></span>|<span data-ttu-id="31d18-160">String</span><span class="sxs-lookup"><span data-stu-id="31d18-160">String</span></span>|<span data-ttu-id="31d18-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31d18-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="31d18-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31d18-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31d18-163">versão</span><span class="sxs-lookup"><span data-stu-id="31d18-163">version</span></span>|<span data-ttu-id="31d18-164">Int32</span><span class="sxs-lookup"><span data-stu-id="31d18-164">Int32</span></span>|<span data-ttu-id="31d18-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31d18-165">Version of the device configuration.</span></span> <span data-ttu-id="31d18-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31d18-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31d18-167">accountName</span><span class="sxs-lookup"><span data-stu-id="31d18-167">accountName</span></span>|<span data-ttu-id="31d18-168">String</span><span class="sxs-lookup"><span data-stu-id="31d18-168">String</span></span>|<span data-ttu-id="31d18-169">Nome da conta do Exchange ActiveSync, exibido para os usuários como o nome do perfil EAS (este).</span><span class="sxs-lookup"><span data-stu-id="31d18-169">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="31d18-170">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="31d18-170">authenticationMethod</span></span>|[<span data-ttu-id="31d18-171">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="31d18-171">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="31d18-172">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="31d18-172">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="31d18-173">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="31d18-173">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="31d18-174">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="31d18-174">syncCalendar</span></span>|<span data-ttu-id="31d18-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="31d18-175">Boolean</span></span>|<span data-ttu-id="31d18-176">Alterna a sincronização do calendário.</span><span class="sxs-lookup"><span data-stu-id="31d18-176">Toggles syncing the calendar.</span></span> <span data-ttu-id="31d18-177">Se definido como falso, o calendário será desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31d18-177">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="31d18-178">syncContacts</span><span class="sxs-lookup"><span data-stu-id="31d18-178">syncContacts</span></span>|<span data-ttu-id="31d18-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="31d18-179">Boolean</span></span>|<span data-ttu-id="31d18-180">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="31d18-180">Toggles syncing contacts.</span></span> <span data-ttu-id="31d18-181">Se definido como falso, os contatos serão desativados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31d18-181">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="31d18-182">syncTasks</span><span class="sxs-lookup"><span data-stu-id="31d18-182">syncTasks</span></span>|<span data-ttu-id="31d18-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="31d18-183">Boolean</span></span>|<span data-ttu-id="31d18-184">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="31d18-184">Toggles syncing tasks.</span></span> <span data-ttu-id="31d18-185">Se definido como falso, as tarefas serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31d18-185">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="31d18-186">syncNotes</span><span class="sxs-lookup"><span data-stu-id="31d18-186">syncNotes</span></span>|<span data-ttu-id="31d18-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="31d18-187">Boolean</span></span>|<span data-ttu-id="31d18-188">Alterna a sincronização das anotações.</span><span class="sxs-lookup"><span data-stu-id="31d18-188">Toggles syncing notes.</span></span> <span data-ttu-id="31d18-189">Se definido como false, as anotações serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31d18-189">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="31d18-190">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="31d18-190">durationOfEmailToSync</span></span>|[<span data-ttu-id="31d18-191">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="31d18-191">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="31d18-192">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="31d18-192">Duration of time email should be synced to.</span></span> <span data-ttu-id="31d18-193">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="31d18-193">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="31d18-194">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="31d18-194">emailAddressSource</span></span>|[<span data-ttu-id="31d18-195">userEmail</span><span class="sxs-lookup"><span data-stu-id="31d18-195">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="31d18-196">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31d18-196">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="31d18-197">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="31d18-197">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="31d18-198">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="31d18-198">emailSyncSchedule</span></span>|[<span data-ttu-id="31d18-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="31d18-199">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="31d18-200">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="31d18-200">Email sync schedule.</span></span> <span data-ttu-id="31d18-201">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="31d18-201">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="31d18-202">hostName</span><span class="sxs-lookup"><span data-stu-id="31d18-202">hostName</span></span>|<span data-ttu-id="31d18-203">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31d18-203">String</span></span>|<span data-ttu-id="31d18-204">Local do Exchange (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="31d18-204">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="31d18-205">requireSmime</span><span class="sxs-lookup"><span data-stu-id="31d18-205">requireSmime</span></span>|<span data-ttu-id="31d18-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="31d18-206">Boolean</span></span>|<span data-ttu-id="31d18-207">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="31d18-207">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="31d18-208">requireSsl</span><span class="sxs-lookup"><span data-stu-id="31d18-208">requireSsl</span></span>|<span data-ttu-id="31d18-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="31d18-209">Boolean</span></span>|<span data-ttu-id="31d18-210">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="31d18-210">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="31d18-211">usernameSource</span><span class="sxs-lookup"><span data-stu-id="31d18-211">usernameSource</span></span>|[<span data-ttu-id="31d18-212">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="31d18-212">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="31d18-213">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31d18-213">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="31d18-214">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="31d18-214">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="31d18-215">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="31d18-215">userDomainNameSource</span></span>|[<span data-ttu-id="31d18-216">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="31d18-216">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="31d18-217">Atributo userDomainname que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31d18-217">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="31d18-218">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="31d18-218">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="31d18-219">customDomainName</span><span class="sxs-lookup"><span data-stu-id="31d18-219">customDomainName</span></span>|<span data-ttu-id="31d18-220">String</span><span class="sxs-lookup"><span data-stu-id="31d18-220">String</span></span>|<span data-ttu-id="31d18-221">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="31d18-221">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="31d18-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="31d18-222">Response</span></span>
<span data-ttu-id="31d18-223">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31d18-223">If successful, this method returns a `201 Created` response code and a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31d18-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="31d18-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="31d18-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31d18-225">Request</span></span>
<span data-ttu-id="31d18-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="31d18-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="31d18-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="31d18-227">Response</span></span>
<span data-ttu-id="31d18-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31d18-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




