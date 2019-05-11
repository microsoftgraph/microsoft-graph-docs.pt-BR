---
title: Atualizar androidWorkProfileGmailEasConfiguration
description: Atualiza as propriedades de um objeto androidWorkProfileGmailEasConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12ee3f51dbfbc62f82a586feb20a8e89317e1634
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928415"
---
# <a name="update-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="fbe12-103">Atualizar androidWorkProfileGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="fbe12-103">Update androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="fbe12-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fbe12-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbe12-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbe12-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbe12-106">Atualiza as propriedades de um objeto [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fbe12-106">Update the properties of a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbe12-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fbe12-107">Prerequisites</span></span>
<span data-ttu-id="fbe12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbe12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbe12-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbe12-110">Permission type</span></span>|<span data-ttu-id="fbe12-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fbe12-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbe12-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbe12-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fbe12-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbe12-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fbe12-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbe12-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbe12-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbe12-115">Not supported.</span></span>|
|<span data-ttu-id="fbe12-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbe12-116">Application</span></span>|<span data-ttu-id="fbe12-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fbe12-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbe12-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbe12-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fbe12-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbe12-119">Request headers</span></span>
|<span data-ttu-id="fbe12-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbe12-120">Header</span></span>|<span data-ttu-id="fbe12-121">Valor</span><span class="sxs-lookup"><span data-stu-id="fbe12-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbe12-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbe12-122">Authorization</span></span>|<span data-ttu-id="fbe12-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbe12-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbe12-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fbe12-124">Accept</span></span>|<span data-ttu-id="fbe12-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fbe12-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbe12-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbe12-126">Request body</span></span>
<span data-ttu-id="fbe12-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fbe12-127">In the request body, supply a JSON representation for the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="fbe12-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fbe12-128">The following table shows the properties that are required when you create the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span></span>

|<span data-ttu-id="fbe12-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbe12-129">Property</span></span>|<span data-ttu-id="fbe12-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbe12-130">Type</span></span>|<span data-ttu-id="fbe12-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbe12-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbe12-132">id</span><span class="sxs-lookup"><span data-stu-id="fbe12-132">id</span></span>|<span data-ttu-id="fbe12-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbe12-133">String</span></span>|<span data-ttu-id="fbe12-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fbe12-134">Key of the entity.</span></span> <span data-ttu-id="fbe12-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbe12-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbe12-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbe12-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fbe12-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbe12-137">DateTimeOffset</span></span>|<span data-ttu-id="fbe12-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="fbe12-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fbe12-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbe12-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbe12-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fbe12-140">roleScopeTagIds</span></span>|<span data-ttu-id="fbe12-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbe12-141">String collection</span></span>|<span data-ttu-id="fbe12-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="fbe12-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fbe12-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbe12-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbe12-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fbe12-144">supportsScopeTags</span></span>|<span data-ttu-id="fbe12-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="fbe12-145">Boolean</span></span>|<span data-ttu-id="fbe12-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="fbe12-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fbe12-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="fbe12-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fbe12-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="fbe12-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fbe12-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbe12-149">This property is read-only.</span></span> <span data-ttu-id="fbe12-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbe12-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbe12-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbe12-151">createdDateTime</span></span>|<span data-ttu-id="fbe12-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbe12-152">DateTimeOffset</span></span>|<span data-ttu-id="fbe12-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fbe12-153">DateTime the object was created.</span></span> <span data-ttu-id="fbe12-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbe12-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbe12-155">description</span><span class="sxs-lookup"><span data-stu-id="fbe12-155">description</span></span>|<span data-ttu-id="fbe12-156">String</span><span class="sxs-lookup"><span data-stu-id="fbe12-156">String</span></span>|<span data-ttu-id="fbe12-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbe12-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fbe12-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbe12-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbe12-159">displayName</span><span class="sxs-lookup"><span data-stu-id="fbe12-159">displayName</span></span>|<span data-ttu-id="fbe12-160">String</span><span class="sxs-lookup"><span data-stu-id="fbe12-160">String</span></span>|<span data-ttu-id="fbe12-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbe12-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fbe12-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbe12-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbe12-163">versão</span><span class="sxs-lookup"><span data-stu-id="fbe12-163">version</span></span>|<span data-ttu-id="fbe12-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fbe12-164">Int32</span></span>|<span data-ttu-id="fbe12-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbe12-165">Version of the device configuration.</span></span> <span data-ttu-id="fbe12-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fbe12-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fbe12-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fbe12-167">authenticationMethod</span></span>|[<span data-ttu-id="fbe12-168">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fbe12-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="fbe12-169">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="fbe12-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="fbe12-170">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fbe12-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="fbe12-171">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="fbe12-171">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="fbe12-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="fbe12-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="fbe12-173">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="fbe12-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="fbe12-174">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="fbe12-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="fbe12-175">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fbe12-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="fbe12-176">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="fbe12-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="fbe12-177">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="fbe12-177">emailAddressSource</span></span>|[<span data-ttu-id="fbe12-178">UserEmail</span><span class="sxs-lookup"><span data-stu-id="fbe12-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="fbe12-179">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbe12-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="fbe12-180">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fbe12-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="fbe12-181">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="fbe12-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="fbe12-182">hostName</span><span class="sxs-lookup"><span data-stu-id="fbe12-182">hostName</span></span>|<span data-ttu-id="fbe12-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbe12-183">String</span></span>|<span data-ttu-id="fbe12-184">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="fbe12-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="fbe12-185">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fbe12-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="fbe12-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="fbe12-186">requireSsl</span></span>|<span data-ttu-id="fbe12-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="fbe12-187">Boolean</span></span>|<span data-ttu-id="fbe12-188">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="fbe12-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="fbe12-189">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fbe12-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="fbe12-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="fbe12-190">usernameSource</span></span>|[<span data-ttu-id="fbe12-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="fbe12-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="fbe12-192">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fbe12-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="fbe12-193">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fbe12-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="fbe12-194">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="fbe12-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="fbe12-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbe12-195">Response</span></span>
<span data-ttu-id="fbe12-196">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbe12-196">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbe12-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbe12-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbe12-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbe12-198">Request</span></span>
<span data-ttu-id="fbe12-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbe12-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 495

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
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
  "usernameSource": "userPrincipalName"
}
```

### <a name="response"></a><span data-ttu-id="fbe12-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbe12-200">Response</span></span>
<span data-ttu-id="fbe12-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbe12-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 667

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "id": "a4a44bb5-4bb5-a4a4-b54b-a4a4b54ba4a4",
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
  "usernameSource": "userPrincipalName"
}
```




