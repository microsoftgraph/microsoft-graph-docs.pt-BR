---
title: Criar androidForWorkGmailEasConfiguration
description: Crie um novo objeto de androidForWorkGmailEasConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fd125237e6f2557fece7dc98920e936fcd4d59c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424865"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="45a6c-103">Criar androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="45a6c-103">Create androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="45a6c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="45a6c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="45a6c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="45a6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45a6c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="45a6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45a6c-107">Crie um novo objeto de [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="45a6c-107">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45a6c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45a6c-108">Prerequisites</span></span>
<span data-ttu-id="45a6c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="45a6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="45a6c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45a6c-111">Permission type</span></span>|<span data-ttu-id="45a6c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45a6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45a6c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45a6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45a6c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45a6c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45a6c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45a6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45a6c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45a6c-116">Not supported.</span></span>|
|<span data-ttu-id="45a6c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45a6c-117">Application</span></span>|<span data-ttu-id="45a6c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45a6c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45a6c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45a6c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="45a6c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45a6c-120">Request headers</span></span>
|<span data-ttu-id="45a6c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45a6c-121">Header</span></span>|<span data-ttu-id="45a6c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45a6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45a6c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45a6c-123">Authorization</span></span>|<span data-ttu-id="45a6c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45a6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45a6c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="45a6c-125">Accept</span></span>|<span data-ttu-id="45a6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45a6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45a6c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45a6c-127">Request body</span></span>
<span data-ttu-id="45a6c-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="45a6c-128">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="45a6c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="45a6c-129">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="45a6c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45a6c-130">Property</span></span>|<span data-ttu-id="45a6c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="45a6c-131">Type</span></span>|<span data-ttu-id="45a6c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="45a6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45a6c-133">id</span><span class="sxs-lookup"><span data-stu-id="45a6c-133">id</span></span>|<span data-ttu-id="45a6c-134">String</span><span class="sxs-lookup"><span data-stu-id="45a6c-134">String</span></span>|<span data-ttu-id="45a6c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="45a6c-135">Key of the entity.</span></span> <span data-ttu-id="45a6c-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45a6c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45a6c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45a6c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="45a6c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45a6c-138">DateTimeOffset</span></span>|<span data-ttu-id="45a6c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="45a6c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="45a6c-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45a6c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45a6c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="45a6c-141">roleScopeTagIds</span></span>|<span data-ttu-id="45a6c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="45a6c-142">String collection</span></span>|<span data-ttu-id="45a6c-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="45a6c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="45a6c-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45a6c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45a6c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="45a6c-145">supportsScopeTags</span></span>|<span data-ttu-id="45a6c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="45a6c-146">Boolean</span></span>|<span data-ttu-id="45a6c-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="45a6c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="45a6c-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="45a6c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="45a6c-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="45a6c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="45a6c-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="45a6c-150">This property is read-only.</span></span> <span data-ttu-id="45a6c-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45a6c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45a6c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45a6c-152">createdDateTime</span></span>|<span data-ttu-id="45a6c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45a6c-153">DateTimeOffset</span></span>|<span data-ttu-id="45a6c-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="45a6c-154">DateTime the object was created.</span></span> <span data-ttu-id="45a6c-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45a6c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45a6c-156">description</span><span class="sxs-lookup"><span data-stu-id="45a6c-156">description</span></span>|<span data-ttu-id="45a6c-157">String</span><span class="sxs-lookup"><span data-stu-id="45a6c-157">String</span></span>|<span data-ttu-id="45a6c-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45a6c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="45a6c-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45a6c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45a6c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="45a6c-160">displayName</span></span>|<span data-ttu-id="45a6c-161">String</span><span class="sxs-lookup"><span data-stu-id="45a6c-161">String</span></span>|<span data-ttu-id="45a6c-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45a6c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="45a6c-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45a6c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45a6c-164">version</span><span class="sxs-lookup"><span data-stu-id="45a6c-164">version</span></span>|<span data-ttu-id="45a6c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="45a6c-165">Int32</span></span>|<span data-ttu-id="45a6c-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45a6c-166">Version of the device configuration.</span></span> <span data-ttu-id="45a6c-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="45a6c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="45a6c-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="45a6c-168">authenticationMethod</span></span>|[<span data-ttu-id="45a6c-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="45a6c-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="45a6c-170">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="45a6c-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="45a6c-171">Herdada do [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45a6c-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="45a6c-172">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="45a6c-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="45a6c-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="45a6c-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="45a6c-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="45a6c-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="45a6c-175">Duração de email de tempo deve ser sincronizada para.</span><span class="sxs-lookup"><span data-stu-id="45a6c-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="45a6c-176">Herdada do [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45a6c-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="45a6c-177">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="45a6c-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="45a6c-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="45a6c-178">emailAddressSource</span></span>|[<span data-ttu-id="45a6c-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="45a6c-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="45a6c-180">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45a6c-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="45a6c-181">Herdada do [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45a6c-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="45a6c-182">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="45a6c-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="45a6c-183">hostName</span><span class="sxs-lookup"><span data-stu-id="45a6c-183">hostName</span></span>|<span data-ttu-id="45a6c-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45a6c-184">String</span></span>|<span data-ttu-id="45a6c-185">Exchange local (URL) que conecta-se para o aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="45a6c-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="45a6c-186">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45a6c-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="45a6c-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="45a6c-187">requireSsl</span></span>|<span data-ttu-id="45a6c-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="45a6c-188">Boolean</span></span>|<span data-ttu-id="45a6c-189">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="45a6c-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="45a6c-190">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="45a6c-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="45a6c-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="45a6c-191">usernameSource</span></span>|[<span data-ttu-id="45a6c-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="45a6c-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="45a6c-193">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="45a6c-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="45a6c-194">Herdada do [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="45a6c-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="45a6c-195">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="45a6c-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="45a6c-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a6c-196">Response</span></span>
<span data-ttu-id="45a6c-197">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45a6c-197">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45a6c-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45a6c-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="45a6c-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45a6c-199">Request</span></span>
<span data-ttu-id="45a6c-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45a6c-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45a6c-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a6c-201">Response</span></span>
<span data-ttu-id="45a6c-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45a6c-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




