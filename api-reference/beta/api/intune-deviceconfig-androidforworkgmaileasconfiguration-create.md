---
title: Criar androidForWorkGmailEasConfiguration
description: Criar um novo objeto androidForWorkGmailEasConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10a53f08d3f0af5bb54d84655e6d735d3d2cd5d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32478998"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="a0632-103">Criar androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0632-103">Create androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="a0632-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0632-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0632-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0632-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0632-106">Criar um novo objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a0632-106">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0632-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0632-107">Prerequisites</span></span>
<span data-ttu-id="a0632-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0632-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0632-110">Permission type</span></span>|<span data-ttu-id="a0632-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0632-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0632-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0632-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0632-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0632-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0632-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0632-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0632-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0632-115">Not supported.</span></span>|
|<span data-ttu-id="a0632-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0632-116">Application</span></span>|<span data-ttu-id="a0632-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0632-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0632-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0632-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0632-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0632-119">Request headers</span></span>
|<span data-ttu-id="a0632-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0632-120">Header</span></span>|<span data-ttu-id="a0632-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a0632-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0632-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0632-122">Authorization</span></span>|<span data-ttu-id="a0632-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0632-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0632-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0632-124">Accept</span></span>|<span data-ttu-id="a0632-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0632-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0632-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0632-126">Request body</span></span>
<span data-ttu-id="a0632-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0632-127">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="a0632-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0632-128">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="a0632-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0632-129">Property</span></span>|<span data-ttu-id="a0632-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0632-130">Type</span></span>|<span data-ttu-id="a0632-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0632-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0632-132">id</span><span class="sxs-lookup"><span data-stu-id="a0632-132">id</span></span>|<span data-ttu-id="a0632-133">String</span><span class="sxs-lookup"><span data-stu-id="a0632-133">String</span></span>|<span data-ttu-id="a0632-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a0632-134">Key of the entity.</span></span> <span data-ttu-id="a0632-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0632-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0632-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0632-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a0632-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0632-137">DateTimeOffset</span></span>|<span data-ttu-id="a0632-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a0632-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a0632-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0632-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0632-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0632-140">roleScopeTagIds</span></span>|<span data-ttu-id="a0632-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0632-141">String collection</span></span>|<span data-ttu-id="a0632-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a0632-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a0632-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0632-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0632-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a0632-144">supportsScopeTags</span></span>|<span data-ttu-id="a0632-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="a0632-145">Boolean</span></span>|<span data-ttu-id="a0632-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a0632-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a0632-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a0632-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a0632-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a0632-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a0632-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a0632-149">This property is read-only.</span></span> <span data-ttu-id="a0632-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0632-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0632-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0632-151">createdDateTime</span></span>|<span data-ttu-id="a0632-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0632-152">DateTimeOffset</span></span>|<span data-ttu-id="a0632-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a0632-153">DateTime the object was created.</span></span> <span data-ttu-id="a0632-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0632-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0632-155">description</span><span class="sxs-lookup"><span data-stu-id="a0632-155">description</span></span>|<span data-ttu-id="a0632-156">String</span><span class="sxs-lookup"><span data-stu-id="a0632-156">String</span></span>|<span data-ttu-id="a0632-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0632-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a0632-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0632-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0632-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a0632-159">displayName</span></span>|<span data-ttu-id="a0632-160">String</span><span class="sxs-lookup"><span data-stu-id="a0632-160">String</span></span>|<span data-ttu-id="a0632-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0632-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a0632-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0632-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0632-163">versão</span><span class="sxs-lookup"><span data-stu-id="a0632-163">version</span></span>|<span data-ttu-id="a0632-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a0632-164">Int32</span></span>|<span data-ttu-id="a0632-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0632-165">Version of the device configuration.</span></span> <span data-ttu-id="a0632-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0632-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0632-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a0632-167">authenticationMethod</span></span>|[<span data-ttu-id="a0632-168">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a0632-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="a0632-169">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="a0632-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="a0632-170">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0632-170">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="a0632-171">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="a0632-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="a0632-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="a0632-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="a0632-173">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="a0632-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="a0632-174">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="a0632-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="a0632-175">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0632-175">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="a0632-176">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="a0632-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="a0632-177">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="a0632-177">emailAddressSource</span></span>|[<span data-ttu-id="a0632-178">userEmail</span><span class="sxs-lookup"><span data-stu-id="a0632-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a0632-179">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0632-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a0632-180">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0632-180">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="a0632-181">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a0632-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a0632-182">hostName</span><span class="sxs-lookup"><span data-stu-id="a0632-182">hostName</span></span>|<span data-ttu-id="a0632-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0632-183">String</span></span>|<span data-ttu-id="a0632-184">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="a0632-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="a0632-185">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0632-185">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="a0632-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="a0632-186">requireSsl</span></span>|<span data-ttu-id="a0632-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="a0632-187">Boolean</span></span>|<span data-ttu-id="a0632-188">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="a0632-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="a0632-189">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0632-189">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="a0632-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a0632-190">usernameSource</span></span>|[<span data-ttu-id="a0632-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="a0632-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="a0632-192">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0632-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a0632-193">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0632-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="a0632-194">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a0632-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="a0632-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0632-195">Response</span></span>
<span data-ttu-id="a0632-196">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0632-196">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0632-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0632-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0632-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0632-198">Request</span></span>
<span data-ttu-id="a0632-199">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0632-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0632-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0632-200">Response</span></span>
<span data-ttu-id="a0632-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0632-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





