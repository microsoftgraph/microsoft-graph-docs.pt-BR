---
title: Criar androidForWorkGmailEasConfiguration
description: Criar um novo objeto androidForWorkGmailEasConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 96f537de719a0dff891673e92dc56f25b435fa70
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154464"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="94352-103">Criar androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="94352-103">Create androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="94352-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94352-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94352-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94352-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94352-106">Criar um novo objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="94352-106">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94352-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94352-107">Prerequisites</span></span>
<span data-ttu-id="94352-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="94352-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="94352-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94352-110">Permission type</span></span>|<span data-ttu-id="94352-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94352-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94352-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94352-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94352-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94352-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="94352-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94352-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94352-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94352-115">Not supported.</span></span>|
|<span data-ttu-id="94352-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94352-116">Application</span></span>|<span data-ttu-id="94352-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94352-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94352-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94352-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="94352-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94352-119">Request headers</span></span>
|<span data-ttu-id="94352-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94352-120">Header</span></span>|<span data-ttu-id="94352-121">Valor</span><span class="sxs-lookup"><span data-stu-id="94352-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94352-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94352-122">Authorization</span></span>|<span data-ttu-id="94352-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94352-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94352-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94352-124">Accept</span></span>|<span data-ttu-id="94352-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94352-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94352-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94352-126">Request body</span></span>
<span data-ttu-id="94352-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="94352-127">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="94352-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="94352-128">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="94352-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94352-129">Property</span></span>|<span data-ttu-id="94352-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="94352-130">Type</span></span>|<span data-ttu-id="94352-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="94352-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94352-132">id</span><span class="sxs-lookup"><span data-stu-id="94352-132">id</span></span>|<span data-ttu-id="94352-133">String</span><span class="sxs-lookup"><span data-stu-id="94352-133">String</span></span>|<span data-ttu-id="94352-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="94352-134">Key of the entity.</span></span> <span data-ttu-id="94352-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94352-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94352-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94352-136">lastModifiedDateTime</span></span>|<span data-ttu-id="94352-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94352-137">DateTimeOffset</span></span>|<span data-ttu-id="94352-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="94352-138">DateTime the object was last modified.</span></span> <span data-ttu-id="94352-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94352-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94352-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="94352-140">roleScopeTagIds</span></span>|<span data-ttu-id="94352-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="94352-141">String collection</span></span>|<span data-ttu-id="94352-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="94352-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="94352-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94352-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94352-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="94352-144">supportsScopeTags</span></span>|<span data-ttu-id="94352-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="94352-145">Boolean</span></span>|<span data-ttu-id="94352-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="94352-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="94352-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="94352-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="94352-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="94352-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="94352-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="94352-149">This property is read-only.</span></span> <span data-ttu-id="94352-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94352-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94352-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="94352-151">createdDateTime</span></span>|<span data-ttu-id="94352-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94352-152">DateTimeOffset</span></span>|<span data-ttu-id="94352-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="94352-153">DateTime the object was created.</span></span> <span data-ttu-id="94352-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94352-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94352-155">description</span><span class="sxs-lookup"><span data-stu-id="94352-155">description</span></span>|<span data-ttu-id="94352-156">String</span><span class="sxs-lookup"><span data-stu-id="94352-156">String</span></span>|<span data-ttu-id="94352-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94352-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="94352-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94352-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94352-159">displayName</span><span class="sxs-lookup"><span data-stu-id="94352-159">displayName</span></span>|<span data-ttu-id="94352-160">String</span><span class="sxs-lookup"><span data-stu-id="94352-160">String</span></span>|<span data-ttu-id="94352-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94352-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="94352-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94352-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94352-163">version</span><span class="sxs-lookup"><span data-stu-id="94352-163">version</span></span>|<span data-ttu-id="94352-164">Int32</span><span class="sxs-lookup"><span data-stu-id="94352-164">Int32</span></span>|<span data-ttu-id="94352-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94352-165">Version of the device configuration.</span></span> <span data-ttu-id="94352-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="94352-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="94352-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="94352-167">authenticationMethod</span></span>|[<span data-ttu-id="94352-168">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="94352-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="94352-169">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="94352-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="94352-170">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="94352-170">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="94352-171">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="94352-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="94352-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="94352-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="94352-173">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="94352-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="94352-174">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="94352-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="94352-175">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="94352-175">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="94352-176">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="94352-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="94352-177">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="94352-177">emailAddressSource</span></span>|[<span data-ttu-id="94352-178">userEmail</span><span class="sxs-lookup"><span data-stu-id="94352-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="94352-179">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94352-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="94352-180">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="94352-180">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="94352-181">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="94352-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="94352-182">hostName</span><span class="sxs-lookup"><span data-stu-id="94352-182">hostName</span></span>|<span data-ttu-id="94352-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94352-183">String</span></span>|<span data-ttu-id="94352-184">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="94352-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="94352-185">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="94352-185">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="94352-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="94352-186">requireSsl</span></span>|<span data-ttu-id="94352-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="94352-187">Boolean</span></span>|<span data-ttu-id="94352-188">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="94352-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="94352-189">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="94352-189">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="94352-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="94352-190">usernameSource</span></span>|[<span data-ttu-id="94352-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="94352-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="94352-192">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94352-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="94352-193">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="94352-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="94352-194">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="94352-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="94352-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="94352-195">Response</span></span>
<span data-ttu-id="94352-196">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94352-196">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94352-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94352-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="94352-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94352-198">Request</span></span>
<span data-ttu-id="94352-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94352-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 491

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="94352-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="94352-200">Response</span></span>
<span data-ttu-id="94352-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94352-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 663

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
  "id": "2bafc891-c891-2baf-91c8-af2b91c8af2b",
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




