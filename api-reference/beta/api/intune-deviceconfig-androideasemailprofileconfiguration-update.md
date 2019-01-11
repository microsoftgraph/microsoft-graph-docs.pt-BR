---
title: Atualizar androidEasEmailProfileConfiguration
description: Atualize as propriedades de um objeto androidEasEmailProfileConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 58542198f24cb39f77a12a3e447de3c416f82215
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828375"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="f9b5d-103">Atualizar androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9b5d-103">Update androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="f9b5d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9b5d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f9b5d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9b5d-107">Atualize as propriedades de um objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f9b5d-107">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9b5d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f9b5d-108">Prerequisites</span></span>
<span data-ttu-id="f9b5d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9b5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9b5d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9b5d-111">Permission type</span></span>|<span data-ttu-id="f9b5d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f9b5d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9b5d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9b5d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f9b5d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9b5d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9b5d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9b5d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9b5d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-116">Not supported.</span></span>|
|<span data-ttu-id="f9b5d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9b5d-117">Application</span></span>|<span data-ttu-id="f9b5d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9b5d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9b5d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f9b5d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b5d-120">Request headers</span></span>
|<span data-ttu-id="f9b5d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f9b5d-121">Header</span></span>|<span data-ttu-id="f9b5d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f9b5d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9b5d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9b5d-123">Authorization</span></span>|<span data-ttu-id="f9b5d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9b5d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f9b5d-125">Accept</span></span>|<span data-ttu-id="f9b5d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f9b5d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9b5d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b5d-127">Request body</span></span>
<span data-ttu-id="f9b5d-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f9b5d-128">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="f9b5d-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f9b5d-129">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="f9b5d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9b5d-130">Property</span></span>|<span data-ttu-id="f9b5d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9b5d-131">Type</span></span>|<span data-ttu-id="f9b5d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9b5d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9b5d-133">id</span><span class="sxs-lookup"><span data-stu-id="f9b5d-133">id</span></span>|<span data-ttu-id="f9b5d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9b5d-134">String</span></span>|<span data-ttu-id="f9b5d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-135">Key of the entity.</span></span> <span data-ttu-id="f9b5d-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9b5d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9b5d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9b5d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f9b5d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9b5d-138">DateTimeOffset</span></span>|<span data-ttu-id="f9b5d-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f9b5d-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9b5d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9b5d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f9b5d-141">roleScopeTagIds</span></span>|<span data-ttu-id="f9b5d-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f9b5d-142">String collection</span></span>|<span data-ttu-id="f9b5d-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f9b5d-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9b5d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9b5d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f9b5d-145">supportsScopeTags</span></span>|<span data-ttu-id="f9b5d-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9b5d-146">Boolean</span></span>|<span data-ttu-id="f9b5d-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f9b5d-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f9b5d-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f9b5d-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-150">This property is read-only.</span></span> <span data-ttu-id="f9b5d-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9b5d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9b5d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9b5d-152">createdDateTime</span></span>|<span data-ttu-id="f9b5d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9b5d-153">DateTimeOffset</span></span>|<span data-ttu-id="f9b5d-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-154">DateTime the object was created.</span></span> <span data-ttu-id="f9b5d-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9b5d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9b5d-156">description</span><span class="sxs-lookup"><span data-stu-id="f9b5d-156">description</span></span>|<span data-ttu-id="f9b5d-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9b5d-157">String</span></span>|<span data-ttu-id="f9b5d-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f9b5d-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9b5d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9b5d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f9b5d-160">displayName</span></span>|<span data-ttu-id="f9b5d-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9b5d-161">String</span></span>|<span data-ttu-id="f9b5d-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f9b5d-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9b5d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9b5d-164">version</span><span class="sxs-lookup"><span data-stu-id="f9b5d-164">version</span></span>|<span data-ttu-id="f9b5d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f9b5d-165">Int32</span></span>|<span data-ttu-id="f9b5d-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-166">Version of the device configuration.</span></span> <span data-ttu-id="f9b5d-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9b5d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9b5d-168">accountName</span><span class="sxs-lookup"><span data-stu-id="f9b5d-168">accountName</span></span>|<span data-ttu-id="f9b5d-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9b5d-169">String</span></span>|<span data-ttu-id="f9b5d-170">Nome da conta do Exchange ActiveSync, exibido aos usuários como o nome do perfil EAS (this).</span><span class="sxs-lookup"><span data-stu-id="f9b5d-170">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="f9b5d-171">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f9b5d-171">authenticationMethod</span></span>|[<span data-ttu-id="f9b5d-172">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f9b5d-172">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="f9b5d-173">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-173">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="f9b5d-174">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-174">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="f9b5d-175">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="f9b5d-175">syncCalendar</span></span>|<span data-ttu-id="f9b5d-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9b5d-176">Boolean</span></span>|<span data-ttu-id="f9b5d-177">Alterna o calendário está sincronizando.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-177">Toggles syncing the calendar.</span></span> <span data-ttu-id="f9b5d-178">Se definido como false calendário está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-178">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="f9b5d-179">syncContacts</span><span class="sxs-lookup"><span data-stu-id="f9b5d-179">syncContacts</span></span>|<span data-ttu-id="f9b5d-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9b5d-180">Boolean</span></span>|<span data-ttu-id="f9b5d-181">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-181">Toggles syncing contacts.</span></span> <span data-ttu-id="f9b5d-182">Se definido como falsos contatos está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-182">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="f9b5d-183">syncTasks</span><span class="sxs-lookup"><span data-stu-id="f9b5d-183">syncTasks</span></span>|<span data-ttu-id="f9b5d-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9b5d-184">Boolean</span></span>|<span data-ttu-id="f9b5d-185">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-185">Toggles syncing tasks.</span></span> <span data-ttu-id="f9b5d-186">Se definido como falsos tarefas está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-186">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="f9b5d-187">syncNotes</span><span class="sxs-lookup"><span data-stu-id="f9b5d-187">syncNotes</span></span>|<span data-ttu-id="f9b5d-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9b5d-188">Boolean</span></span>|<span data-ttu-id="f9b5d-189">Alterna a sincronização de notas.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-189">Toggles syncing notes.</span></span> <span data-ttu-id="f9b5d-190">Se definido como falsos anotações está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-190">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="f9b5d-191">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="f9b5d-191">durationOfEmailToSync</span></span>|[<span data-ttu-id="f9b5d-192">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="f9b5d-192">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="f9b5d-193">Duração de email de tempo deve ser sincronizada para.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-193">Duration of time email should be synced to.</span></span> <span data-ttu-id="f9b5d-194">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-194">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="f9b5d-195">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="f9b5d-195">emailAddressSource</span></span>|[<span data-ttu-id="f9b5d-196">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="f9b5d-196">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="f9b5d-197">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-197">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f9b5d-198">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-198">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="f9b5d-199">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="f9b5d-199">emailSyncSchedule</span></span>|[<span data-ttu-id="f9b5d-200">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="f9b5d-200">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="f9b5d-201">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-201">Email sync schedule.</span></span> <span data-ttu-id="f9b5d-202">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-202">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="f9b5d-203">hostName</span><span class="sxs-lookup"><span data-stu-id="f9b5d-203">hostName</span></span>|<span data-ttu-id="f9b5d-204">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9b5d-204">String</span></span>|<span data-ttu-id="f9b5d-205">Exchange local (URL) que o aplicativo de email nativo se conecta ao.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-205">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="f9b5d-206">requireSmime</span><span class="sxs-lookup"><span data-stu-id="f9b5d-206">requireSmime</span></span>|<span data-ttu-id="f9b5d-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9b5d-207">Boolean</span></span>|<span data-ttu-id="f9b5d-208">Indica se deve ou não usar certificados S/MIME.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-208">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="f9b5d-209">requireSsl</span><span class="sxs-lookup"><span data-stu-id="f9b5d-209">requireSsl</span></span>|<span data-ttu-id="f9b5d-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="f9b5d-210">Boolean</span></span>|<span data-ttu-id="f9b5d-211">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-211">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="f9b5d-212">usernameSource</span><span class="sxs-lookup"><span data-stu-id="f9b5d-212">usernameSource</span></span>|[<span data-ttu-id="f9b5d-213">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="f9b5d-213">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="f9b5d-214">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-214">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f9b5d-215">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-215">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="f9b5d-216">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="f9b5d-216">userDomainNameSource</span></span>|[<span data-ttu-id="f9b5d-217">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="f9b5d-217">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="f9b5d-218">Atributo nome_do_domínio que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-218">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="f9b5d-219">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-219">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="f9b5d-220">customDomainName</span><span class="sxs-lookup"><span data-stu-id="f9b5d-220">customDomainName</span></span>|<span data-ttu-id="f9b5d-221">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f9b5d-221">String</span></span>|<span data-ttu-id="f9b5d-222">Valor de nome de domínio personalizado usado ao gerar um perfil de email antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-222">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="f9b5d-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9b5d-223">Response</span></span>
<span data-ttu-id="f9b5d-224">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-224">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9b5d-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9b5d-225">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9b5d-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9b5d-226">Request</span></span>
<span data-ttu-id="f9b5d-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 783

{
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

### <a name="response"></a><span data-ttu-id="f9b5d-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9b5d-228">Response</span></span>
<span data-ttu-id="f9b5d-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9b5d-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





