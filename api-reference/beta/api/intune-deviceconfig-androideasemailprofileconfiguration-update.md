---
title: Atualizar androidEasEmailProfileConfiguration
description: Atualize as propriedades de um objeto androidEasEmailProfileConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9b1cb423ebe3cf5424151f665be3ca682aff5fb3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406987"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="97017-103">Atualizar androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="97017-103">Update androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="97017-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="97017-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="97017-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="97017-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97017-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="97017-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97017-107">Atualize as propriedades de um objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="97017-107">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97017-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97017-108">Prerequisites</span></span>
<span data-ttu-id="97017-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="97017-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="97017-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97017-111">Permission type</span></span>|<span data-ttu-id="97017-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="97017-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97017-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97017-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97017-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97017-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="97017-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97017-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97017-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97017-116">Not supported.</span></span>|
|<span data-ttu-id="97017-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97017-117">Application</span></span>|<span data-ttu-id="97017-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97017-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97017-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97017-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="97017-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97017-120">Request headers</span></span>
|<span data-ttu-id="97017-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="97017-121">Header</span></span>|<span data-ttu-id="97017-122">Valor</span><span class="sxs-lookup"><span data-stu-id="97017-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97017-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97017-123">Authorization</span></span>|<span data-ttu-id="97017-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97017-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97017-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="97017-125">Accept</span></span>|<span data-ttu-id="97017-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97017-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97017-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97017-127">Request body</span></span>
<span data-ttu-id="97017-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="97017-128">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="97017-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="97017-129">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="97017-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97017-130">Property</span></span>|<span data-ttu-id="97017-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="97017-131">Type</span></span>|<span data-ttu-id="97017-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="97017-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97017-133">id</span><span class="sxs-lookup"><span data-stu-id="97017-133">id</span></span>|<span data-ttu-id="97017-134">String</span><span class="sxs-lookup"><span data-stu-id="97017-134">String</span></span>|<span data-ttu-id="97017-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="97017-135">Key of the entity.</span></span> <span data-ttu-id="97017-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97017-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97017-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97017-137">lastModifiedDateTime</span></span>|<span data-ttu-id="97017-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97017-138">DateTimeOffset</span></span>|<span data-ttu-id="97017-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="97017-139">DateTime the object was last modified.</span></span> <span data-ttu-id="97017-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97017-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97017-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="97017-141">roleScopeTagIds</span></span>|<span data-ttu-id="97017-142">String collection</span><span class="sxs-lookup"><span data-stu-id="97017-142">String collection</span></span>|<span data-ttu-id="97017-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="97017-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="97017-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97017-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97017-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="97017-145">supportsScopeTags</span></span>|<span data-ttu-id="97017-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="97017-146">Boolean</span></span>|<span data-ttu-id="97017-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="97017-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="97017-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="97017-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="97017-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="97017-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="97017-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97017-150">This property is read-only.</span></span> <span data-ttu-id="97017-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97017-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97017-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97017-152">createdDateTime</span></span>|<span data-ttu-id="97017-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97017-153">DateTimeOffset</span></span>|<span data-ttu-id="97017-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="97017-154">DateTime the object was created.</span></span> <span data-ttu-id="97017-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97017-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97017-156">description</span><span class="sxs-lookup"><span data-stu-id="97017-156">description</span></span>|<span data-ttu-id="97017-157">String</span><span class="sxs-lookup"><span data-stu-id="97017-157">String</span></span>|<span data-ttu-id="97017-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97017-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="97017-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97017-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97017-160">displayName</span><span class="sxs-lookup"><span data-stu-id="97017-160">displayName</span></span>|<span data-ttu-id="97017-161">String</span><span class="sxs-lookup"><span data-stu-id="97017-161">String</span></span>|<span data-ttu-id="97017-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97017-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="97017-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97017-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97017-164">version</span><span class="sxs-lookup"><span data-stu-id="97017-164">version</span></span>|<span data-ttu-id="97017-165">Int32</span><span class="sxs-lookup"><span data-stu-id="97017-165">Int32</span></span>|<span data-ttu-id="97017-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97017-166">Version of the device configuration.</span></span> <span data-ttu-id="97017-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="97017-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="97017-168">accountName</span><span class="sxs-lookup"><span data-stu-id="97017-168">accountName</span></span>|<span data-ttu-id="97017-169">String</span><span class="sxs-lookup"><span data-stu-id="97017-169">String</span></span>|<span data-ttu-id="97017-170">Nome da conta do Exchange ActiveSync, exibido aos usuários como o nome do perfil EAS (this).</span><span class="sxs-lookup"><span data-stu-id="97017-170">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="97017-171">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="97017-171">authenticationMethod</span></span>|[<span data-ttu-id="97017-172">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="97017-172">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="97017-173">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="97017-173">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="97017-174">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="97017-174">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="97017-175">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="97017-175">syncCalendar</span></span>|<span data-ttu-id="97017-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="97017-176">Boolean</span></span>|<span data-ttu-id="97017-177">Alterna o calendário está sincronizando.</span><span class="sxs-lookup"><span data-stu-id="97017-177">Toggles syncing the calendar.</span></span> <span data-ttu-id="97017-178">Se definido como false calendário está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97017-178">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="97017-179">syncContacts</span><span class="sxs-lookup"><span data-stu-id="97017-179">syncContacts</span></span>|<span data-ttu-id="97017-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="97017-180">Boolean</span></span>|<span data-ttu-id="97017-181">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="97017-181">Toggles syncing contacts.</span></span> <span data-ttu-id="97017-182">Se definido como falsos contatos está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97017-182">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="97017-183">syncTasks</span><span class="sxs-lookup"><span data-stu-id="97017-183">syncTasks</span></span>|<span data-ttu-id="97017-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="97017-184">Boolean</span></span>|<span data-ttu-id="97017-185">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="97017-185">Toggles syncing tasks.</span></span> <span data-ttu-id="97017-186">Se definido como falsos tarefas está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97017-186">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="97017-187">syncNotes</span><span class="sxs-lookup"><span data-stu-id="97017-187">syncNotes</span></span>|<span data-ttu-id="97017-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="97017-188">Boolean</span></span>|<span data-ttu-id="97017-189">Alterna a sincronização de notas.</span><span class="sxs-lookup"><span data-stu-id="97017-189">Toggles syncing notes.</span></span> <span data-ttu-id="97017-190">Se definido como falsos anotações está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97017-190">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="97017-191">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="97017-191">durationOfEmailToSync</span></span>|[<span data-ttu-id="97017-192">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="97017-192">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="97017-193">Duração de email de tempo deve ser sincronizada para.</span><span class="sxs-lookup"><span data-stu-id="97017-193">Duration of time email should be synced to.</span></span> <span data-ttu-id="97017-194">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="97017-194">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="97017-195">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="97017-195">emailAddressSource</span></span>|[<span data-ttu-id="97017-196">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="97017-196">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="97017-197">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97017-197">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="97017-198">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="97017-198">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="97017-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="97017-199">emailSyncSchedule</span></span>|[<span data-ttu-id="97017-200">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="97017-200">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="97017-201">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="97017-201">Email sync schedule.</span></span> <span data-ttu-id="97017-202">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="97017-202">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="97017-203">hostName</span><span class="sxs-lookup"><span data-stu-id="97017-203">hostName</span></span>|<span data-ttu-id="97017-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97017-204">String</span></span>|<span data-ttu-id="97017-205">Exchange local (URL) que o aplicativo de email nativo se conecta ao.</span><span class="sxs-lookup"><span data-stu-id="97017-205">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="97017-206">requireSmime</span><span class="sxs-lookup"><span data-stu-id="97017-206">requireSmime</span></span>|<span data-ttu-id="97017-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="97017-207">Boolean</span></span>|<span data-ttu-id="97017-208">Indica se deve ou não usar certificados S/MIME.</span><span class="sxs-lookup"><span data-stu-id="97017-208">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="97017-209">requireSsl</span><span class="sxs-lookup"><span data-stu-id="97017-209">requireSsl</span></span>|<span data-ttu-id="97017-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="97017-210">Boolean</span></span>|<span data-ttu-id="97017-211">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="97017-211">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="97017-212">usernameSource</span><span class="sxs-lookup"><span data-stu-id="97017-212">usernameSource</span></span>|[<span data-ttu-id="97017-213">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="97017-213">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="97017-214">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97017-214">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="97017-215">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="97017-215">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="97017-216">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="97017-216">userDomainNameSource</span></span>|[<span data-ttu-id="97017-217">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="97017-217">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="97017-218">Atributo nome_do_domínio que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97017-218">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="97017-219">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="97017-219">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="97017-220">customDomainName</span><span class="sxs-lookup"><span data-stu-id="97017-220">customDomainName</span></span>|<span data-ttu-id="97017-221">String</span><span class="sxs-lookup"><span data-stu-id="97017-221">String</span></span>|<span data-ttu-id="97017-222">Valor de nome de domínio personalizado usado ao gerar um perfil de email antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="97017-222">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="97017-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="97017-223">Response</span></span>
<span data-ttu-id="97017-224">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97017-224">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97017-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97017-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="97017-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97017-226">Request</span></span>
<span data-ttu-id="97017-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97017-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="97017-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="97017-228">Response</span></span>
<span data-ttu-id="97017-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97017-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




