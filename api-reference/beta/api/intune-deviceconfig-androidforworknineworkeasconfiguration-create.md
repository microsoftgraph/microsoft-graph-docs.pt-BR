---
title: Criar androidForWorkNineWorkEasConfiguration
description: Criar um novo objeto androidForWorkNineWorkEasConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f8f9b00660a88f2111f1f88d53e42750089561d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933463"
---
# <a name="create-androidforworknineworkeasconfiguration"></a><span data-ttu-id="40365-103">Criar androidForWorkNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="40365-103">Create androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="40365-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40365-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40365-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40365-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40365-106">Criar um novo objeto [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="40365-106">Create a new [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40365-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40365-107">Prerequisites</span></span>
<span data-ttu-id="40365-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40365-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40365-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40365-110">Permission type</span></span>|<span data-ttu-id="40365-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40365-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40365-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40365-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40365-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40365-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="40365-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40365-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40365-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40365-115">Not supported.</span></span>|
|<span data-ttu-id="40365-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40365-116">Application</span></span>|<span data-ttu-id="40365-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40365-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40365-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40365-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="40365-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40365-119">Request headers</span></span>
|<span data-ttu-id="40365-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40365-120">Header</span></span>|<span data-ttu-id="40365-121">Valor</span><span class="sxs-lookup"><span data-stu-id="40365-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40365-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="40365-122">Authorization</span></span>|<span data-ttu-id="40365-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40365-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40365-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40365-124">Accept</span></span>|<span data-ttu-id="40365-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40365-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40365-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40365-126">Request body</span></span>
<span data-ttu-id="40365-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="40365-127">In the request body, supply a JSON representation for the androidForWorkNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="40365-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="40365-128">The following table shows the properties that are required when you create the androidForWorkNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="40365-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40365-129">Property</span></span>|<span data-ttu-id="40365-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="40365-130">Type</span></span>|<span data-ttu-id="40365-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="40365-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40365-132">id</span><span class="sxs-lookup"><span data-stu-id="40365-132">id</span></span>|<span data-ttu-id="40365-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40365-133">String</span></span>|<span data-ttu-id="40365-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="40365-134">Key of the entity.</span></span> <span data-ttu-id="40365-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40365-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40365-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40365-136">lastModifiedDateTime</span></span>|<span data-ttu-id="40365-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40365-137">DateTimeOffset</span></span>|<span data-ttu-id="40365-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="40365-138">DateTime the object was last modified.</span></span> <span data-ttu-id="40365-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40365-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40365-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="40365-140">roleScopeTagIds</span></span>|<span data-ttu-id="40365-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="40365-141">String collection</span></span>|<span data-ttu-id="40365-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="40365-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="40365-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40365-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40365-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="40365-144">supportsScopeTags</span></span>|<span data-ttu-id="40365-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="40365-145">Boolean</span></span>|<span data-ttu-id="40365-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="40365-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="40365-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="40365-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="40365-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="40365-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="40365-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40365-149">This property is read-only.</span></span> <span data-ttu-id="40365-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40365-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40365-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40365-151">createdDateTime</span></span>|<span data-ttu-id="40365-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40365-152">DateTimeOffset</span></span>|<span data-ttu-id="40365-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="40365-153">DateTime the object was created.</span></span> <span data-ttu-id="40365-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40365-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40365-155">description</span><span class="sxs-lookup"><span data-stu-id="40365-155">description</span></span>|<span data-ttu-id="40365-156">String</span><span class="sxs-lookup"><span data-stu-id="40365-156">String</span></span>|<span data-ttu-id="40365-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40365-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="40365-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40365-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40365-159">displayName</span><span class="sxs-lookup"><span data-stu-id="40365-159">displayName</span></span>|<span data-ttu-id="40365-160">String</span><span class="sxs-lookup"><span data-stu-id="40365-160">String</span></span>|<span data-ttu-id="40365-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40365-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="40365-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40365-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40365-163">versão</span><span class="sxs-lookup"><span data-stu-id="40365-163">version</span></span>|<span data-ttu-id="40365-164">Int32</span><span class="sxs-lookup"><span data-stu-id="40365-164">Int32</span></span>|<span data-ttu-id="40365-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40365-165">Version of the device configuration.</span></span> <span data-ttu-id="40365-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="40365-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="40365-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="40365-167">authenticationMethod</span></span>|[<span data-ttu-id="40365-168">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="40365-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="40365-169">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="40365-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="40365-170">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="40365-170">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="40365-171">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="40365-171">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="40365-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="40365-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="40365-173">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="40365-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="40365-174">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="40365-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="40365-175">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="40365-175">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="40365-176">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="40365-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="40365-177">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="40365-177">emailAddressSource</span></span>|[<span data-ttu-id="40365-178">UserEmail</span><span class="sxs-lookup"><span data-stu-id="40365-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="40365-179">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40365-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="40365-180">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="40365-180">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="40365-181">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="40365-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="40365-182">hostName</span><span class="sxs-lookup"><span data-stu-id="40365-182">hostName</span></span>|<span data-ttu-id="40365-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40365-183">String</span></span>|<span data-ttu-id="40365-184">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="40365-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="40365-185">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="40365-185">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="40365-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="40365-186">requireSsl</span></span>|<span data-ttu-id="40365-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="40365-187">Boolean</span></span>|<span data-ttu-id="40365-188">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="40365-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="40365-189">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="40365-189">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="40365-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="40365-190">usernameSource</span></span>|[<span data-ttu-id="40365-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="40365-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="40365-192">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40365-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="40365-193">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="40365-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="40365-194">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="40365-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="40365-195">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="40365-195">syncCalendar</span></span>|<span data-ttu-id="40365-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="40365-196">Boolean</span></span>|<span data-ttu-id="40365-197">Alterna a sincronização do calendário.</span><span class="sxs-lookup"><span data-stu-id="40365-197">Toggles syncing the calendar.</span></span> <span data-ttu-id="40365-198">Se definido como falso, o calendário será desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40365-198">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="40365-199">syncContacts</span><span class="sxs-lookup"><span data-stu-id="40365-199">syncContacts</span></span>|<span data-ttu-id="40365-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="40365-200">Boolean</span></span>|<span data-ttu-id="40365-201">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="40365-201">Toggles syncing contacts.</span></span> <span data-ttu-id="40365-202">Se definido como falso, os contatos serão desativados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40365-202">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="40365-203">syncTasks</span><span class="sxs-lookup"><span data-stu-id="40365-203">syncTasks</span></span>|<span data-ttu-id="40365-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="40365-204">Boolean</span></span>|<span data-ttu-id="40365-205">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="40365-205">Toggles syncing tasks.</span></span> <span data-ttu-id="40365-206">Se definido como falso, as tarefas serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40365-206">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="40365-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="40365-207">Response</span></span>
<span data-ttu-id="40365-208">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40365-208">If successful, this method returns a `201 Created` response code and a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40365-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40365-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="40365-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40365-210">Request</span></span>
<span data-ttu-id="40365-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40365-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 566

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="40365-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="40365-212">Response</span></span>
<span data-ttu-id="40365-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40365-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 738

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "id": "f8ef19e0-19e0-f8ef-e019-eff8e019eff8",
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




