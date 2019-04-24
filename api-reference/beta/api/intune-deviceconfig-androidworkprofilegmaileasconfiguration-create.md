---
title: Criar androidWorkProfileGmailEasConfiguration
description: Criar um novo objeto androidWorkProfileGmailEasConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2948e8942dbc14c9810669120921ffae13a941e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32474448"
---
# <a name="create-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="d77b3-103">Criar androidWorkProfileGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="d77b3-103">Create androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="d77b3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d77b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d77b3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d77b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d77b3-106">Criar um novo objeto [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d77b3-106">Create a new [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d77b3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d77b3-107">Prerequisites</span></span>
<span data-ttu-id="d77b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d77b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d77b3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d77b3-110">Permission type</span></span>|<span data-ttu-id="d77b3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d77b3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d77b3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d77b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d77b3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d77b3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d77b3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d77b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d77b3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d77b3-115">Not supported.</span></span>|
|<span data-ttu-id="d77b3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d77b3-116">Application</span></span>|<span data-ttu-id="d77b3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d77b3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d77b3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d77b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d77b3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d77b3-119">Request headers</span></span>
|<span data-ttu-id="d77b3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d77b3-120">Header</span></span>|<span data-ttu-id="d77b3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d77b3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d77b3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d77b3-122">Authorization</span></span>|<span data-ttu-id="d77b3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d77b3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d77b3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d77b3-124">Accept</span></span>|<span data-ttu-id="d77b3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d77b3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d77b3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d77b3-126">Request body</span></span>
<span data-ttu-id="d77b3-127">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d77b3-127">In the request body, supply a JSON representation for the androidWorkProfileGmailEasConfiguration object.</span></span>

<span data-ttu-id="d77b3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d77b3-128">The following table shows the properties that are required when you create the androidWorkProfileGmailEasConfiguration.</span></span>

|<span data-ttu-id="d77b3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d77b3-129">Property</span></span>|<span data-ttu-id="d77b3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d77b3-130">Type</span></span>|<span data-ttu-id="d77b3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d77b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d77b3-132">id</span><span class="sxs-lookup"><span data-stu-id="d77b3-132">id</span></span>|<span data-ttu-id="d77b3-133">String</span><span class="sxs-lookup"><span data-stu-id="d77b3-133">String</span></span>|<span data-ttu-id="d77b3-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d77b3-134">Key of the entity.</span></span> <span data-ttu-id="d77b3-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d77b3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d77b3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d77b3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d77b3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d77b3-137">DateTimeOffset</span></span>|<span data-ttu-id="d77b3-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d77b3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d77b3-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d77b3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d77b3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d77b3-140">roleScopeTagIds</span></span>|<span data-ttu-id="d77b3-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d77b3-141">String collection</span></span>|<span data-ttu-id="d77b3-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d77b3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d77b3-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d77b3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d77b3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d77b3-144">supportsScopeTags</span></span>|<span data-ttu-id="d77b3-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="d77b3-145">Boolean</span></span>|<span data-ttu-id="d77b3-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d77b3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d77b3-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d77b3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d77b3-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d77b3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d77b3-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d77b3-149">This property is read-only.</span></span> <span data-ttu-id="d77b3-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d77b3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d77b3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d77b3-151">createdDateTime</span></span>|<span data-ttu-id="d77b3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d77b3-152">DateTimeOffset</span></span>|<span data-ttu-id="d77b3-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d77b3-153">DateTime the object was created.</span></span> <span data-ttu-id="d77b3-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d77b3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d77b3-155">description</span><span class="sxs-lookup"><span data-stu-id="d77b3-155">description</span></span>|<span data-ttu-id="d77b3-156">String</span><span class="sxs-lookup"><span data-stu-id="d77b3-156">String</span></span>|<span data-ttu-id="d77b3-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d77b3-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d77b3-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d77b3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d77b3-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d77b3-159">displayName</span></span>|<span data-ttu-id="d77b3-160">String</span><span class="sxs-lookup"><span data-stu-id="d77b3-160">String</span></span>|<span data-ttu-id="d77b3-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d77b3-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d77b3-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d77b3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d77b3-163">versão</span><span class="sxs-lookup"><span data-stu-id="d77b3-163">version</span></span>|<span data-ttu-id="d77b3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d77b3-164">Int32</span></span>|<span data-ttu-id="d77b3-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d77b3-165">Version of the device configuration.</span></span> <span data-ttu-id="d77b3-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d77b3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d77b3-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d77b3-167">authenticationMethod</span></span>|[<span data-ttu-id="d77b3-168">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d77b3-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="d77b3-169">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="d77b3-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="d77b3-170">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d77b3-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d77b3-171">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="d77b3-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="d77b3-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="d77b3-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="d77b3-173">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="d77b3-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="d77b3-174">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="d77b3-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="d77b3-175">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d77b3-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d77b3-176">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="d77b3-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="d77b3-177">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="d77b3-177">emailAddressSource</span></span>|[<span data-ttu-id="d77b3-178">userEmail</span><span class="sxs-lookup"><span data-stu-id="d77b3-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d77b3-179">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d77b3-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d77b3-180">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d77b3-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d77b3-181">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d77b3-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d77b3-182">hostName</span><span class="sxs-lookup"><span data-stu-id="d77b3-182">hostName</span></span>|<span data-ttu-id="d77b3-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d77b3-183">String</span></span>|<span data-ttu-id="d77b3-184">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="d77b3-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="d77b3-185">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d77b3-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="d77b3-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="d77b3-186">requireSsl</span></span>|<span data-ttu-id="d77b3-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="d77b3-187">Boolean</span></span>|<span data-ttu-id="d77b3-188">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="d77b3-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="d77b3-189">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d77b3-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="d77b3-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d77b3-190">usernameSource</span></span>|[<span data-ttu-id="d77b3-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="d77b3-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="d77b3-192">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d77b3-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d77b3-193">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d77b3-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="d77b3-194">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d77b3-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="d77b3-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="d77b3-195">Response</span></span>
<span data-ttu-id="d77b3-196">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d77b3-196">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d77b3-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d77b3-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="d77b3-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d77b3-198">Request</span></span>
<span data-ttu-id="d77b3-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d77b3-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d77b3-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="d77b3-200">Response</span></span>
<span data-ttu-id="d77b3-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d77b3-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





