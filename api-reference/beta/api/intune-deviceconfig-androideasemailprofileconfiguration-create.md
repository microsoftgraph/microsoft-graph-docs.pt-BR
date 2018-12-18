---
title: Criar androidEasEmailProfileConfiguration
description: Crie um novo objeto de androidEasEmailProfileConfiguration.
author: tfitzmac
ms.openlocfilehash: 38e4e36917ac1679420261746713205f77693b73
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361968"
---
# <a name="create-androideasemailprofileconfiguration"></a><span data-ttu-id="15fad-103">Criar androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="15fad-103">Create androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="15fad-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="15fad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15fad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="15fad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15fad-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="15fad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15fad-107">Crie um novo objeto de [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="15fad-107">Create a new [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="15fad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15fad-108">Prerequisites</span></span>
<span data-ttu-id="15fad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15fad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15fad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15fad-111">Permission type</span></span>|<span data-ttu-id="15fad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15fad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15fad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15fad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15fad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15fad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15fad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15fad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15fad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15fad-116">Not supported.</span></span>|
|<span data-ttu-id="15fad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15fad-117">Application</span></span>|<span data-ttu-id="15fad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15fad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15fad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15fad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="15fad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15fad-120">Request headers</span></span>
|<span data-ttu-id="15fad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15fad-121">Header</span></span>|<span data-ttu-id="15fad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="15fad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15fad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="15fad-123">Authorization</span></span>|<span data-ttu-id="15fad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15fad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15fad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15fad-125">Accept</span></span>|<span data-ttu-id="15fad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15fad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15fad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15fad-127">Request body</span></span>
<span data-ttu-id="15fad-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="15fad-128">In the request body, supply a JSON representation for the androidEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="15fad-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="15fad-129">The following table shows the properties that are required when you create the androidEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="15fad-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15fad-130">Property</span></span>|<span data-ttu-id="15fad-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="15fad-131">Type</span></span>|<span data-ttu-id="15fad-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="15fad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15fad-133">id</span><span class="sxs-lookup"><span data-stu-id="15fad-133">id</span></span>|<span data-ttu-id="15fad-134">String</span><span class="sxs-lookup"><span data-stu-id="15fad-134">String</span></span>|<span data-ttu-id="15fad-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="15fad-135">Key of the entity.</span></span> <span data-ttu-id="15fad-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15fad-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15fad-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15fad-137">lastModifiedDateTime</span></span>|<span data-ttu-id="15fad-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15fad-138">DateTimeOffset</span></span>|<span data-ttu-id="15fad-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="15fad-139">DateTime the object was last modified.</span></span> <span data-ttu-id="15fad-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15fad-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15fad-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="15fad-141">roleScopeTagIds</span></span>|<span data-ttu-id="15fad-142">String collection</span><span class="sxs-lookup"><span data-stu-id="15fad-142">String collection</span></span>|<span data-ttu-id="15fad-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="15fad-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="15fad-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15fad-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15fad-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="15fad-145">supportsScopeTags</span></span>|<span data-ttu-id="15fad-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="15fad-146">Boolean</span></span>|<span data-ttu-id="15fad-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="15fad-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="15fad-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="15fad-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="15fad-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="15fad-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="15fad-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="15fad-150">This property is read-only.</span></span> <span data-ttu-id="15fad-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15fad-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15fad-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15fad-152">createdDateTime</span></span>|<span data-ttu-id="15fad-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15fad-153">DateTimeOffset</span></span>|<span data-ttu-id="15fad-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="15fad-154">DateTime the object was created.</span></span> <span data-ttu-id="15fad-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15fad-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15fad-156">description</span><span class="sxs-lookup"><span data-stu-id="15fad-156">description</span></span>|<span data-ttu-id="15fad-157">String</span><span class="sxs-lookup"><span data-stu-id="15fad-157">String</span></span>|<span data-ttu-id="15fad-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15fad-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="15fad-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15fad-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15fad-160">displayName</span><span class="sxs-lookup"><span data-stu-id="15fad-160">displayName</span></span>|<span data-ttu-id="15fad-161">String</span><span class="sxs-lookup"><span data-stu-id="15fad-161">String</span></span>|<span data-ttu-id="15fad-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15fad-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="15fad-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15fad-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15fad-164">version</span><span class="sxs-lookup"><span data-stu-id="15fad-164">version</span></span>|<span data-ttu-id="15fad-165">Int32</span><span class="sxs-lookup"><span data-stu-id="15fad-165">Int32</span></span>|<span data-ttu-id="15fad-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15fad-166">Version of the device configuration.</span></span> <span data-ttu-id="15fad-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15fad-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15fad-168">accountName</span><span class="sxs-lookup"><span data-stu-id="15fad-168">accountName</span></span>|<span data-ttu-id="15fad-169">String</span><span class="sxs-lookup"><span data-stu-id="15fad-169">String</span></span>|<span data-ttu-id="15fad-170">Nome da conta do Exchange ActiveSync, exibido aos usuários como o nome do perfil EAS (this).</span><span class="sxs-lookup"><span data-stu-id="15fad-170">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="15fad-171">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="15fad-171">authenticationMethod</span></span>|[<span data-ttu-id="15fad-172">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="15fad-172">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="15fad-173">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="15fad-173">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="15fad-174">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="15fad-174">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="15fad-175">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="15fad-175">syncCalendar</span></span>|<span data-ttu-id="15fad-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="15fad-176">Boolean</span></span>|<span data-ttu-id="15fad-177">Alterna o calendário está sincronizando.</span><span class="sxs-lookup"><span data-stu-id="15fad-177">Toggles syncing the calendar.</span></span> <span data-ttu-id="15fad-178">Se definido como false calendário está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15fad-178">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="15fad-179">syncContacts</span><span class="sxs-lookup"><span data-stu-id="15fad-179">syncContacts</span></span>|<span data-ttu-id="15fad-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="15fad-180">Boolean</span></span>|<span data-ttu-id="15fad-181">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="15fad-181">Toggles syncing contacts.</span></span> <span data-ttu-id="15fad-182">Se definido como falsos contatos está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15fad-182">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="15fad-183">syncTasks</span><span class="sxs-lookup"><span data-stu-id="15fad-183">syncTasks</span></span>|<span data-ttu-id="15fad-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="15fad-184">Boolean</span></span>|<span data-ttu-id="15fad-185">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="15fad-185">Toggles syncing tasks.</span></span> <span data-ttu-id="15fad-186">Se definido como falsos tarefas está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15fad-186">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="15fad-187">syncNotes</span><span class="sxs-lookup"><span data-stu-id="15fad-187">syncNotes</span></span>|<span data-ttu-id="15fad-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="15fad-188">Boolean</span></span>|<span data-ttu-id="15fad-189">Alterna a sincronização de notas.</span><span class="sxs-lookup"><span data-stu-id="15fad-189">Toggles syncing notes.</span></span> <span data-ttu-id="15fad-190">Se definido como falsos anotações está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15fad-190">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="15fad-191">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="15fad-191">durationOfEmailToSync</span></span>|[<span data-ttu-id="15fad-192">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="15fad-192">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="15fad-193">Duração de email de tempo deve ser sincronizada para.</span><span class="sxs-lookup"><span data-stu-id="15fad-193">Duration of time email should be synced to.</span></span> <span data-ttu-id="15fad-194">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="15fad-194">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="15fad-195">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="15fad-195">emailAddressSource</span></span>|[<span data-ttu-id="15fad-196">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="15fad-196">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="15fad-197">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15fad-197">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="15fad-198">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="15fad-198">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="15fad-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="15fad-199">emailSyncSchedule</span></span>|[<span data-ttu-id="15fad-200">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="15fad-200">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="15fad-201">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="15fad-201">Email sync schedule.</span></span> <span data-ttu-id="15fad-202">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="15fad-202">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="15fad-203">hostName</span><span class="sxs-lookup"><span data-stu-id="15fad-203">hostName</span></span>|<span data-ttu-id="15fad-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15fad-204">String</span></span>|<span data-ttu-id="15fad-205">Exchange local (URL) que o aplicativo de email nativo se conecta ao.</span><span class="sxs-lookup"><span data-stu-id="15fad-205">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="15fad-206">requireSmime</span><span class="sxs-lookup"><span data-stu-id="15fad-206">requireSmime</span></span>|<span data-ttu-id="15fad-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="15fad-207">Boolean</span></span>|<span data-ttu-id="15fad-208">Indica se deve ou não usar certificados S/MIME.</span><span class="sxs-lookup"><span data-stu-id="15fad-208">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="15fad-209">requireSsl</span><span class="sxs-lookup"><span data-stu-id="15fad-209">requireSsl</span></span>|<span data-ttu-id="15fad-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="15fad-210">Boolean</span></span>|<span data-ttu-id="15fad-211">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="15fad-211">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="15fad-212">usernameSource</span><span class="sxs-lookup"><span data-stu-id="15fad-212">usernameSource</span></span>|[<span data-ttu-id="15fad-213">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="15fad-213">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="15fad-214">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15fad-214">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="15fad-215">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="15fad-215">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="15fad-216">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="15fad-216">userDomainNameSource</span></span>|[<span data-ttu-id="15fad-217">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="15fad-217">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="15fad-218">Atributo nome_do_domínio que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15fad-218">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="15fad-219">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="15fad-219">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="15fad-220">customDomainName</span><span class="sxs-lookup"><span data-stu-id="15fad-220">customDomainName</span></span>|<span data-ttu-id="15fad-221">String</span><span class="sxs-lookup"><span data-stu-id="15fad-221">String</span></span>|<span data-ttu-id="15fad-222">Valor de nome de domínio personalizado usado ao gerar um perfil de email antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15fad-222">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="15fad-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="15fad-223">Response</span></span>
<span data-ttu-id="15fad-224">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15fad-224">If successful, this method returns a `201 Created` response code and a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15fad-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15fad-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="15fad-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15fad-226">Request</span></span>
<span data-ttu-id="15fad-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15fad-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 857

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="15fad-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="15fad-228">Response</span></span>
<span data-ttu-id="15fad-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15fad-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





