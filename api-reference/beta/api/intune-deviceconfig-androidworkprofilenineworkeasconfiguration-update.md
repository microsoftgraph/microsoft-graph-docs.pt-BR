---
title: Atualizar androidWorkProfileNineWorkEasConfiguration
description: Atualize as propriedades de um objeto androidWorkProfileNineWorkEasConfiguration.
ms.openlocfilehash: dcf17a25a61eb11e9ec8eacf469513cd2e831d9c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037665"
---
# <a name="update-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="58b2c-103">Atualizar androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="58b2c-103">Update androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="58b2c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="58b2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="58b2c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="58b2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58b2c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="58b2c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="58b2c-107">Atualize as propriedades de um objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="58b2c-107">Update the properties of a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="58b2c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58b2c-108">Prerequisites</span></span>
<span data-ttu-id="58b2c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58b2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58b2c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58b2c-111">Permission type</span></span>|<span data-ttu-id="58b2c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58b2c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58b2c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58b2c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58b2c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58b2c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58b2c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58b2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58b2c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58b2c-116">Not supported.</span></span>|
|<span data-ttu-id="58b2c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58b2c-117">Application</span></span>|<span data-ttu-id="58b2c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58b2c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58b2c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58b2c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="58b2c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58b2c-120">Request headers</span></span>
|<span data-ttu-id="58b2c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58b2c-121">Header</span></span>|<span data-ttu-id="58b2c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="58b2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58b2c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="58b2c-123">Authorization</span></span>|<span data-ttu-id="58b2c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58b2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58b2c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58b2c-125">Accept</span></span>|<span data-ttu-id="58b2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58b2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58b2c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58b2c-127">Request body</span></span>
<span data-ttu-id="58b2c-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="58b2c-128">In the request body, supply a JSON representation for the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="58b2c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58b2c-129">The following table shows the properties that are required when you create the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="58b2c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58b2c-130">Property</span></span>|<span data-ttu-id="58b2c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="58b2c-131">Type</span></span>|<span data-ttu-id="58b2c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="58b2c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58b2c-133">id</span><span class="sxs-lookup"><span data-stu-id="58b2c-133">id</span></span>|<span data-ttu-id="58b2c-134">String</span><span class="sxs-lookup"><span data-stu-id="58b2c-134">String</span></span>|<span data-ttu-id="58b2c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="58b2c-135">Key of the entity.</span></span> <span data-ttu-id="58b2c-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58b2c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58b2c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58b2c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="58b2c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58b2c-138">DateTimeOffset</span></span>|<span data-ttu-id="58b2c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="58b2c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="58b2c-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58b2c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58b2c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="58b2c-141">roleScopeTagIds</span></span>|<span data-ttu-id="58b2c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="58b2c-142">String collection</span></span>|<span data-ttu-id="58b2c-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="58b2c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="58b2c-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58b2c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58b2c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="58b2c-145">supportsScopeTags</span></span>|<span data-ttu-id="58b2c-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="58b2c-146">Boolean</span></span>|<span data-ttu-id="58b2c-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="58b2c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="58b2c-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="58b2c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="58b2c-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="58b2c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="58b2c-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="58b2c-150">This property is read-only.</span></span> <span data-ttu-id="58b2c-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58b2c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58b2c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58b2c-152">createdDateTime</span></span>|<span data-ttu-id="58b2c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58b2c-153">DateTimeOffset</span></span>|<span data-ttu-id="58b2c-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="58b2c-154">DateTime the object was created.</span></span> <span data-ttu-id="58b2c-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58b2c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58b2c-156">description</span><span class="sxs-lookup"><span data-stu-id="58b2c-156">description</span></span>|<span data-ttu-id="58b2c-157">String</span><span class="sxs-lookup"><span data-stu-id="58b2c-157">String</span></span>|<span data-ttu-id="58b2c-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="58b2c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="58b2c-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58b2c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58b2c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="58b2c-160">displayName</span></span>|<span data-ttu-id="58b2c-161">String</span><span class="sxs-lookup"><span data-stu-id="58b2c-161">String</span></span>|<span data-ttu-id="58b2c-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="58b2c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="58b2c-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58b2c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58b2c-164">version</span><span class="sxs-lookup"><span data-stu-id="58b2c-164">version</span></span>|<span data-ttu-id="58b2c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="58b2c-165">Int32</span></span>|<span data-ttu-id="58b2c-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="58b2c-166">Version of the device configuration.</span></span> <span data-ttu-id="58b2c-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="58b2c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58b2c-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="58b2c-168">authenticationMethod</span></span>|[<span data-ttu-id="58b2c-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="58b2c-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="58b2c-170">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="58b2c-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="58b2c-171">Herdada do [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="58b2c-171">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="58b2c-172">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="58b2c-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="58b2c-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="58b2c-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="58b2c-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="58b2c-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="58b2c-175">Duração de email de tempo deve ser sincronizada para.</span><span class="sxs-lookup"><span data-stu-id="58b2c-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="58b2c-176">Herdada do [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="58b2c-176">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="58b2c-177">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="58b2c-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="58b2c-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="58b2c-178">emailAddressSource</span></span>|[<span data-ttu-id="58b2c-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="58b2c-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="58b2c-180">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="58b2c-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="58b2c-181">Herdada do [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="58b2c-181">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="58b2c-182">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="58b2c-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="58b2c-183">hostName</span><span class="sxs-lookup"><span data-stu-id="58b2c-183">hostName</span></span>|<span data-ttu-id="58b2c-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58b2c-184">String</span></span>|<span data-ttu-id="58b2c-185">Exchange local (URL) que conecta-se para o aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="58b2c-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="58b2c-186">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="58b2c-186">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="58b2c-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="58b2c-187">requireSsl</span></span>|<span data-ttu-id="58b2c-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="58b2c-188">Boolean</span></span>|<span data-ttu-id="58b2c-189">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="58b2c-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="58b2c-190">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="58b2c-190">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="58b2c-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="58b2c-191">usernameSource</span></span>|[<span data-ttu-id="58b2c-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="58b2c-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="58b2c-193">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="58b2c-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="58b2c-194">Herdada do [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="58b2c-194">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="58b2c-195">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="58b2c-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="58b2c-196">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="58b2c-196">syncCalendar</span></span>|<span data-ttu-id="58b2c-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="58b2c-197">Boolean</span></span>|<span data-ttu-id="58b2c-198">Alterna o calendário está sincronizando.</span><span class="sxs-lookup"><span data-stu-id="58b2c-198">Toggles syncing the calendar.</span></span> <span data-ttu-id="58b2c-199">Se definido como falso, o calendário está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="58b2c-199">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="58b2c-200">syncContacts</span><span class="sxs-lookup"><span data-stu-id="58b2c-200">syncContacts</span></span>|<span data-ttu-id="58b2c-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="58b2c-201">Boolean</span></span>|<span data-ttu-id="58b2c-202">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="58b2c-202">Toggles syncing contacts.</span></span> <span data-ttu-id="58b2c-203">Se definido como falsos contatos está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="58b2c-203">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="58b2c-204">syncTasks</span><span class="sxs-lookup"><span data-stu-id="58b2c-204">syncTasks</span></span>|<span data-ttu-id="58b2c-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="58b2c-205">Boolean</span></span>|<span data-ttu-id="58b2c-206">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="58b2c-206">Toggles syncing tasks.</span></span> <span data-ttu-id="58b2c-207">Se definido como falsos tarefas está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="58b2c-207">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="58b2c-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="58b2c-208">Response</span></span>
<span data-ttu-id="58b2c-209">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58b2c-209">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58b2c-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58b2c-210">Example</span></span>
### <a name="request"></a><span data-ttu-id="58b2c-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58b2c-211">Request</span></span>
<span data-ttu-id="58b2c-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58b2c-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 553

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```

### <a name="response"></a><span data-ttu-id="58b2c-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="58b2c-213">Response</span></span>
<span data-ttu-id="58b2c-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58b2c-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 742

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```





