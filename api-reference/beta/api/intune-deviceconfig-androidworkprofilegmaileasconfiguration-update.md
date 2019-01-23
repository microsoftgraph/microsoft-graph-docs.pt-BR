---
title: Atualizar androidWorkProfileGmailEasConfiguration
description: Atualize as propriedades de um objeto androidWorkProfileGmailEasConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 381cadea135bf1c09fb70250283ae829d0c0c65f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394233"
---
# <a name="update-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="db181-103">Atualizar androidWorkProfileGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="db181-103">Update androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="db181-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="db181-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="db181-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="db181-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db181-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="db181-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db181-107">Atualize as propriedades de um objeto [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="db181-107">Update the properties of a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db181-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db181-108">Prerequisites</span></span>
<span data-ttu-id="db181-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="db181-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="db181-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db181-111">Permission type</span></span>|<span data-ttu-id="db181-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="db181-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db181-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db181-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db181-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db181-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db181-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db181-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db181-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db181-116">Not supported.</span></span>|
|<span data-ttu-id="db181-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db181-117">Application</span></span>|<span data-ttu-id="db181-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db181-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db181-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db181-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="db181-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db181-120">Request headers</span></span>
|<span data-ttu-id="db181-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db181-121">Header</span></span>|<span data-ttu-id="db181-122">Valor</span><span class="sxs-lookup"><span data-stu-id="db181-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db181-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="db181-123">Authorization</span></span>|<span data-ttu-id="db181-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db181-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db181-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db181-125">Accept</span></span>|<span data-ttu-id="db181-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db181-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db181-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db181-127">Request body</span></span>
<span data-ttu-id="db181-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="db181-128">In the request body, supply a JSON representation for the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="db181-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="db181-129">The following table shows the properties that are required when you create the [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md).</span></span>

|<span data-ttu-id="db181-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db181-130">Property</span></span>|<span data-ttu-id="db181-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="db181-131">Type</span></span>|<span data-ttu-id="db181-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="db181-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db181-133">id</span><span class="sxs-lookup"><span data-stu-id="db181-133">id</span></span>|<span data-ttu-id="db181-134">String</span><span class="sxs-lookup"><span data-stu-id="db181-134">String</span></span>|<span data-ttu-id="db181-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="db181-135">Key of the entity.</span></span> <span data-ttu-id="db181-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db181-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db181-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db181-137">lastModifiedDateTime</span></span>|<span data-ttu-id="db181-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db181-138">DateTimeOffset</span></span>|<span data-ttu-id="db181-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="db181-139">DateTime the object was last modified.</span></span> <span data-ttu-id="db181-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db181-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db181-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="db181-141">roleScopeTagIds</span></span>|<span data-ttu-id="db181-142">String collection</span><span class="sxs-lookup"><span data-stu-id="db181-142">String collection</span></span>|<span data-ttu-id="db181-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="db181-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="db181-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db181-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db181-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="db181-145">supportsScopeTags</span></span>|<span data-ttu-id="db181-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="db181-146">Boolean</span></span>|<span data-ttu-id="db181-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="db181-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="db181-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="db181-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="db181-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="db181-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="db181-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="db181-150">This property is read-only.</span></span> <span data-ttu-id="db181-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db181-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db181-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db181-152">createdDateTime</span></span>|<span data-ttu-id="db181-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db181-153">DateTimeOffset</span></span>|<span data-ttu-id="db181-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="db181-154">DateTime the object was created.</span></span> <span data-ttu-id="db181-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db181-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db181-156">description</span><span class="sxs-lookup"><span data-stu-id="db181-156">description</span></span>|<span data-ttu-id="db181-157">String</span><span class="sxs-lookup"><span data-stu-id="db181-157">String</span></span>|<span data-ttu-id="db181-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db181-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="db181-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db181-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db181-160">displayName</span><span class="sxs-lookup"><span data-stu-id="db181-160">displayName</span></span>|<span data-ttu-id="db181-161">String</span><span class="sxs-lookup"><span data-stu-id="db181-161">String</span></span>|<span data-ttu-id="db181-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db181-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="db181-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db181-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db181-164">version</span><span class="sxs-lookup"><span data-stu-id="db181-164">version</span></span>|<span data-ttu-id="db181-165">Int32</span><span class="sxs-lookup"><span data-stu-id="db181-165">Int32</span></span>|<span data-ttu-id="db181-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db181-166">Version of the device configuration.</span></span> <span data-ttu-id="db181-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="db181-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="db181-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="db181-168">authenticationMethod</span></span>|[<span data-ttu-id="db181-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="db181-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="db181-170">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="db181-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="db181-171">Herdada do [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="db181-171">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="db181-172">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="db181-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="db181-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="db181-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="db181-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="db181-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="db181-175">Duração de email de tempo deve ser sincronizada para.</span><span class="sxs-lookup"><span data-stu-id="db181-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="db181-176">Herdada do [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="db181-176">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="db181-177">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="db181-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="db181-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="db181-178">emailAddressSource</span></span>|[<span data-ttu-id="db181-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="db181-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="db181-180">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db181-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="db181-181">Herdada do [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="db181-181">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="db181-182">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="db181-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="db181-183">hostName</span><span class="sxs-lookup"><span data-stu-id="db181-183">hostName</span></span>|<span data-ttu-id="db181-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db181-184">String</span></span>|<span data-ttu-id="db181-185">Exchange local (URL) que conecta-se para o aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="db181-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="db181-186">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="db181-186">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="db181-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="db181-187">requireSsl</span></span>|<span data-ttu-id="db181-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="db181-188">Boolean</span></span>|<span data-ttu-id="db181-189">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="db181-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="db181-190">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="db181-190">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="db181-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="db181-191">usernameSource</span></span>|[<span data-ttu-id="db181-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="db181-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="db181-193">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="db181-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="db181-194">Herdada do [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="db181-194">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="db181-195">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="db181-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="db181-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="db181-196">Response</span></span>
<span data-ttu-id="db181-197">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db181-197">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db181-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db181-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="db181-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db181-199">Request</span></span>
<span data-ttu-id="db181-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db181-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="db181-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="db181-201">Response</span></span>
<span data-ttu-id="db181-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db181-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




