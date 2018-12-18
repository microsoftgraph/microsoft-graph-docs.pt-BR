---
title: Atualizar androidForWorkGmailEasConfiguration
description: Atualize as propriedades de um objeto androidForWorkGmailEasConfiguration.
author: tfitzmac
ms.openlocfilehash: 9da99cb4ecb0d466a8367e2d7b5ad3902956e1c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317791"
---
# <a name="update-androidforworkgmaileasconfiguration"></a><span data-ttu-id="0f048-103">Atualizar androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f048-103">Update androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="0f048-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0f048-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f048-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0f048-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f048-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0f048-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f048-107">Atualize as propriedades de um objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0f048-107">Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f048-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f048-108">Prerequisites</span></span>
<span data-ttu-id="0f048-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f048-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f048-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f048-111">Permission type</span></span>|<span data-ttu-id="0f048-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f048-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f048-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f048-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f048-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f048-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f048-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f048-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f048-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f048-116">Not supported.</span></span>|
|<span data-ttu-id="0f048-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f048-117">Application</span></span>|<span data-ttu-id="0f048-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f048-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f048-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f048-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0f048-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f048-120">Request headers</span></span>
|<span data-ttu-id="0f048-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f048-121">Header</span></span>|<span data-ttu-id="0f048-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0f048-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f048-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f048-123">Authorization</span></span>|<span data-ttu-id="0f048-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f048-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f048-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0f048-125">Accept</span></span>|<span data-ttu-id="0f048-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f048-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f048-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f048-127">Request body</span></span>
<span data-ttu-id="0f048-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0f048-128">In the request body, supply a JSON representation for the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="0f048-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f048-129">The following table shows the properties that are required when you create the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>

|<span data-ttu-id="0f048-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f048-130">Property</span></span>|<span data-ttu-id="0f048-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f048-131">Type</span></span>|<span data-ttu-id="0f048-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f048-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f048-133">id</span><span class="sxs-lookup"><span data-stu-id="0f048-133">id</span></span>|<span data-ttu-id="0f048-134">String</span><span class="sxs-lookup"><span data-stu-id="0f048-134">String</span></span>|<span data-ttu-id="0f048-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f048-135">Key of the entity.</span></span> <span data-ttu-id="0f048-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f048-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f048-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f048-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0f048-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f048-138">DateTimeOffset</span></span>|<span data-ttu-id="0f048-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0f048-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0f048-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f048-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f048-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f048-141">roleScopeTagIds</span></span>|<span data-ttu-id="0f048-142">String collection</span><span class="sxs-lookup"><span data-stu-id="0f048-142">String collection</span></span>|<span data-ttu-id="0f048-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f048-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0f048-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f048-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f048-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0f048-145">supportsScopeTags</span></span>|<span data-ttu-id="0f048-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f048-146">Boolean</span></span>|<span data-ttu-id="0f048-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0f048-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0f048-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0f048-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0f048-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="0f048-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0f048-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0f048-150">This property is read-only.</span></span> <span data-ttu-id="0f048-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f048-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f048-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f048-152">createdDateTime</span></span>|<span data-ttu-id="0f048-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f048-153">DateTimeOffset</span></span>|<span data-ttu-id="0f048-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0f048-154">DateTime the object was created.</span></span> <span data-ttu-id="0f048-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f048-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f048-156">description</span><span class="sxs-lookup"><span data-stu-id="0f048-156">description</span></span>|<span data-ttu-id="0f048-157">String</span><span class="sxs-lookup"><span data-stu-id="0f048-157">String</span></span>|<span data-ttu-id="0f048-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0f048-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0f048-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f048-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f048-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0f048-160">displayName</span></span>|<span data-ttu-id="0f048-161">String</span><span class="sxs-lookup"><span data-stu-id="0f048-161">String</span></span>|<span data-ttu-id="0f048-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0f048-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0f048-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f048-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f048-164">version</span><span class="sxs-lookup"><span data-stu-id="0f048-164">version</span></span>|<span data-ttu-id="0f048-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0f048-165">Int32</span></span>|<span data-ttu-id="0f048-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0f048-166">Version of the device configuration.</span></span> <span data-ttu-id="0f048-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f048-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f048-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0f048-168">authenticationMethod</span></span>|[<span data-ttu-id="0f048-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0f048-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="0f048-170">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="0f048-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="0f048-171">Herdada do [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0f048-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="0f048-172">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="0f048-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="0f048-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="0f048-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="0f048-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="0f048-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="0f048-175">Duração de email de tempo deve ser sincronizada para.</span><span class="sxs-lookup"><span data-stu-id="0f048-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="0f048-176">Herdada do [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0f048-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="0f048-177">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="0f048-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="0f048-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="0f048-178">emailAddressSource</span></span>|[<span data-ttu-id="0f048-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="0f048-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0f048-180">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0f048-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0f048-181">Herdada do [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0f048-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="0f048-182">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0f048-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0f048-183">hostName</span><span class="sxs-lookup"><span data-stu-id="0f048-183">hostName</span></span>|<span data-ttu-id="0f048-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f048-184">String</span></span>|<span data-ttu-id="0f048-185">Exchange local (URL) que conecta-se para o aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="0f048-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="0f048-186">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0f048-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="0f048-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="0f048-187">requireSsl</span></span>|<span data-ttu-id="0f048-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f048-188">Boolean</span></span>|<span data-ttu-id="0f048-189">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="0f048-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="0f048-190">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0f048-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="0f048-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="0f048-191">usernameSource</span></span>|[<span data-ttu-id="0f048-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="0f048-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="0f048-193">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0f048-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0f048-194">Herdada do [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0f048-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="0f048-195">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0f048-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="0f048-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f048-196">Response</span></span>
<span data-ttu-id="0f048-197">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f048-197">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f048-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f048-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f048-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f048-199">Request</span></span>
<span data-ttu-id="0f048-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f048-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 481

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
  "usernameSource": "userPrincipalName"
}
```

### <a name="response"></a><span data-ttu-id="0f048-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f048-201">Response</span></span>
<span data-ttu-id="0f048-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f048-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





