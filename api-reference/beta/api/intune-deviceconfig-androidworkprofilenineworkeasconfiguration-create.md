---
title: Criar androidWorkProfileNineWorkEasConfiguration
description: Criar um novo objeto androidWorkProfileNineWorkEasConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 555ddaa8819dd52cc1caba3e8b98f1981e055f11
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969383"
---
# <a name="create-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="6d035-103">Criar androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="6d035-103">Create androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="6d035-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d035-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d035-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d035-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d035-106">Criar um novo objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6d035-106">Create a new [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d035-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d035-107">Prerequisites</span></span>
<span data-ttu-id="6d035-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d035-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d035-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d035-110">Permission type</span></span>|<span data-ttu-id="6d035-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d035-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d035-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d035-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d035-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d035-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d035-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d035-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d035-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d035-115">Not supported.</span></span>|
|<span data-ttu-id="6d035-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d035-116">Application</span></span>|<span data-ttu-id="6d035-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d035-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d035-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d035-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6d035-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d035-119">Request headers</span></span>
|<span data-ttu-id="6d035-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d035-120">Header</span></span>|<span data-ttu-id="6d035-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6d035-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d035-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d035-122">Authorization</span></span>|<span data-ttu-id="6d035-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d035-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d035-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d035-124">Accept</span></span>|<span data-ttu-id="6d035-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d035-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d035-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d035-126">Request body</span></span>
<span data-ttu-id="6d035-127">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6d035-127">In the request body, supply a JSON representation for the androidWorkProfileNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="6d035-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6d035-128">The following table shows the properties that are required when you create the androidWorkProfileNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="6d035-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d035-129">Property</span></span>|<span data-ttu-id="6d035-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d035-130">Type</span></span>|<span data-ttu-id="6d035-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d035-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d035-132">id</span><span class="sxs-lookup"><span data-stu-id="6d035-132">id</span></span>|<span data-ttu-id="6d035-133">String</span><span class="sxs-lookup"><span data-stu-id="6d035-133">String</span></span>|<span data-ttu-id="6d035-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6d035-134">Key of the entity.</span></span> <span data-ttu-id="6d035-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d035-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d035-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d035-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6d035-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d035-137">DateTimeOffset</span></span>|<span data-ttu-id="6d035-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6d035-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6d035-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d035-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d035-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6d035-140">roleScopeTagIds</span></span>|<span data-ttu-id="6d035-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="6d035-141">String collection</span></span>|<span data-ttu-id="6d035-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6d035-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6d035-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d035-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d035-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6d035-144">supportsScopeTags</span></span>|<span data-ttu-id="6d035-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d035-145">Boolean</span></span>|<span data-ttu-id="6d035-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6d035-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6d035-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6d035-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6d035-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6d035-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6d035-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d035-149">This property is read-only.</span></span> <span data-ttu-id="6d035-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d035-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d035-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d035-151">createdDateTime</span></span>|<span data-ttu-id="6d035-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d035-152">DateTimeOffset</span></span>|<span data-ttu-id="6d035-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6d035-153">DateTime the object was created.</span></span> <span data-ttu-id="6d035-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d035-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d035-155">descrição</span><span class="sxs-lookup"><span data-stu-id="6d035-155">description</span></span>|<span data-ttu-id="6d035-156">String</span><span class="sxs-lookup"><span data-stu-id="6d035-156">String</span></span>|<span data-ttu-id="6d035-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d035-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6d035-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d035-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d035-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6d035-159">displayName</span></span>|<span data-ttu-id="6d035-160">String</span><span class="sxs-lookup"><span data-stu-id="6d035-160">String</span></span>|<span data-ttu-id="6d035-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d035-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6d035-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d035-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d035-163">versão</span><span class="sxs-lookup"><span data-stu-id="6d035-163">version</span></span>|<span data-ttu-id="6d035-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6d035-164">Int32</span></span>|<span data-ttu-id="6d035-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d035-165">Version of the device configuration.</span></span> <span data-ttu-id="6d035-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d035-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d035-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6d035-167">authenticationMethod</span></span>|[<span data-ttu-id="6d035-168">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6d035-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="6d035-169">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="6d035-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="6d035-170">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6d035-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="6d035-171">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="6d035-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="6d035-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="6d035-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="6d035-173">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="6d035-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="6d035-174">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="6d035-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="6d035-175">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6d035-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="6d035-176">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="6d035-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="6d035-177">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="6d035-177">emailAddressSource</span></span>|[<span data-ttu-id="6d035-178">userEmail</span><span class="sxs-lookup"><span data-stu-id="6d035-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6d035-179">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d035-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6d035-180">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6d035-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="6d035-181">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="6d035-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6d035-182">hostName</span><span class="sxs-lookup"><span data-stu-id="6d035-182">hostName</span></span>|<span data-ttu-id="6d035-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d035-183">String</span></span>|<span data-ttu-id="6d035-184">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="6d035-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="6d035-185">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6d035-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="6d035-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="6d035-186">requireSsl</span></span>|<span data-ttu-id="6d035-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d035-187">Boolean</span></span>|<span data-ttu-id="6d035-188">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="6d035-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="6d035-189">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6d035-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="6d035-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="6d035-190">usernameSource</span></span>|[<span data-ttu-id="6d035-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="6d035-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="6d035-192">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d035-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6d035-193">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6d035-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="6d035-194">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="6d035-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6d035-195">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="6d035-195">syncCalendar</span></span>|<span data-ttu-id="6d035-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d035-196">Boolean</span></span>|<span data-ttu-id="6d035-197">Alterna a sincronização do calendário.</span><span class="sxs-lookup"><span data-stu-id="6d035-197">Toggles syncing the calendar.</span></span> <span data-ttu-id="6d035-198">Se definido como falso, o calendário será desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d035-198">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="6d035-199">syncContacts</span><span class="sxs-lookup"><span data-stu-id="6d035-199">syncContacts</span></span>|<span data-ttu-id="6d035-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d035-200">Boolean</span></span>|<span data-ttu-id="6d035-201">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="6d035-201">Toggles syncing contacts.</span></span> <span data-ttu-id="6d035-202">Se definido como falso, os contatos serão desativados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d035-202">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="6d035-203">syncTasks</span><span class="sxs-lookup"><span data-stu-id="6d035-203">syncTasks</span></span>|<span data-ttu-id="6d035-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d035-204">Boolean</span></span>|<span data-ttu-id="6d035-205">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="6d035-205">Toggles syncing tasks.</span></span> <span data-ttu-id="6d035-206">Se definido como falso, as tarefas serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d035-206">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="6d035-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d035-207">Response</span></span>
<span data-ttu-id="6d035-208">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d035-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d035-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d035-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d035-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d035-210">Request</span></span>
<span data-ttu-id="6d035-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d035-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 570

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="6d035-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d035-212">Response</span></span>
<span data-ttu-id="6d035-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d035-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




