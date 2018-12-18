---
title: Atualizar androidWorkProfileNineWorkEasConfiguration
description: Atualize as propriedades de um objeto androidWorkProfileNineWorkEasConfiguration.
author: tfitzmac
ms.openlocfilehash: e0ecb99966c9966afce379d4c4546bc303f24e42
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345287"
---
# <a name="update-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="18264-103">Atualizar androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="18264-103">Update androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="18264-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="18264-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18264-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="18264-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18264-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="18264-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18264-107">Atualize as propriedades de um objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="18264-107">Update the properties of a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18264-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18264-108">Prerequisites</span></span>
<span data-ttu-id="18264-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18264-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18264-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18264-111">Permission type</span></span>|<span data-ttu-id="18264-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18264-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18264-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18264-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18264-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18264-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18264-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18264-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18264-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18264-116">Not supported.</span></span>|
|<span data-ttu-id="18264-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18264-117">Application</span></span>|<span data-ttu-id="18264-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18264-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18264-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18264-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="18264-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18264-120">Request headers</span></span>
|<span data-ttu-id="18264-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18264-121">Header</span></span>|<span data-ttu-id="18264-122">Valor</span><span class="sxs-lookup"><span data-stu-id="18264-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18264-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="18264-123">Authorization</span></span>|<span data-ttu-id="18264-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18264-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18264-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18264-125">Accept</span></span>|<span data-ttu-id="18264-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18264-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18264-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18264-127">Request body</span></span>
<span data-ttu-id="18264-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="18264-128">In the request body, supply a JSON representation for the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="18264-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18264-129">The following table shows the properties that are required when you create the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="18264-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18264-130">Property</span></span>|<span data-ttu-id="18264-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="18264-131">Type</span></span>|<span data-ttu-id="18264-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="18264-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18264-133">id</span><span class="sxs-lookup"><span data-stu-id="18264-133">id</span></span>|<span data-ttu-id="18264-134">String</span><span class="sxs-lookup"><span data-stu-id="18264-134">String</span></span>|<span data-ttu-id="18264-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="18264-135">Key of the entity.</span></span> <span data-ttu-id="18264-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18264-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18264-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18264-137">lastModifiedDateTime</span></span>|<span data-ttu-id="18264-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18264-138">DateTimeOffset</span></span>|<span data-ttu-id="18264-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="18264-139">DateTime the object was last modified.</span></span> <span data-ttu-id="18264-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18264-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18264-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18264-141">roleScopeTagIds</span></span>|<span data-ttu-id="18264-142">String collection</span><span class="sxs-lookup"><span data-stu-id="18264-142">String collection</span></span>|<span data-ttu-id="18264-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="18264-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="18264-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18264-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18264-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="18264-145">supportsScopeTags</span></span>|<span data-ttu-id="18264-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="18264-146">Boolean</span></span>|<span data-ttu-id="18264-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="18264-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="18264-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="18264-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="18264-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="18264-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="18264-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18264-150">This property is read-only.</span></span> <span data-ttu-id="18264-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18264-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18264-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18264-152">createdDateTime</span></span>|<span data-ttu-id="18264-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18264-153">DateTimeOffset</span></span>|<span data-ttu-id="18264-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="18264-154">DateTime the object was created.</span></span> <span data-ttu-id="18264-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18264-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18264-156">description</span><span class="sxs-lookup"><span data-stu-id="18264-156">description</span></span>|<span data-ttu-id="18264-157">String</span><span class="sxs-lookup"><span data-stu-id="18264-157">String</span></span>|<span data-ttu-id="18264-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18264-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="18264-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18264-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18264-160">displayName</span><span class="sxs-lookup"><span data-stu-id="18264-160">displayName</span></span>|<span data-ttu-id="18264-161">String</span><span class="sxs-lookup"><span data-stu-id="18264-161">String</span></span>|<span data-ttu-id="18264-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18264-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="18264-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18264-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18264-164">version</span><span class="sxs-lookup"><span data-stu-id="18264-164">version</span></span>|<span data-ttu-id="18264-165">Int32</span><span class="sxs-lookup"><span data-stu-id="18264-165">Int32</span></span>|<span data-ttu-id="18264-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18264-166">Version of the device configuration.</span></span> <span data-ttu-id="18264-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18264-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18264-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="18264-168">authenticationMethod</span></span>|[<span data-ttu-id="18264-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="18264-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="18264-170">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="18264-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="18264-171">Herdada do [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="18264-171">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="18264-172">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="18264-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="18264-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="18264-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="18264-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="18264-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="18264-175">Duração de email de tempo deve ser sincronizada para.</span><span class="sxs-lookup"><span data-stu-id="18264-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="18264-176">Herdada do [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="18264-176">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="18264-177">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="18264-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="18264-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="18264-178">emailAddressSource</span></span>|[<span data-ttu-id="18264-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="18264-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="18264-180">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18264-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="18264-181">Herdada do [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="18264-181">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="18264-182">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="18264-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="18264-183">hostName</span><span class="sxs-lookup"><span data-stu-id="18264-183">hostName</span></span>|<span data-ttu-id="18264-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18264-184">String</span></span>|<span data-ttu-id="18264-185">Exchange local (URL) que conecta-se para o aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="18264-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="18264-186">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="18264-186">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="18264-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="18264-187">requireSsl</span></span>|<span data-ttu-id="18264-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="18264-188">Boolean</span></span>|<span data-ttu-id="18264-189">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="18264-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="18264-190">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="18264-190">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="18264-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="18264-191">usernameSource</span></span>|[<span data-ttu-id="18264-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="18264-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="18264-193">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18264-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="18264-194">Herdada do [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="18264-194">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="18264-195">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="18264-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="18264-196">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="18264-196">syncCalendar</span></span>|<span data-ttu-id="18264-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="18264-197">Boolean</span></span>|<span data-ttu-id="18264-198">Alterna o calendário está sincronizando.</span><span class="sxs-lookup"><span data-stu-id="18264-198">Toggles syncing the calendar.</span></span> <span data-ttu-id="18264-199">Se definido como falso, o calendário está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18264-199">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="18264-200">syncContacts</span><span class="sxs-lookup"><span data-stu-id="18264-200">syncContacts</span></span>|<span data-ttu-id="18264-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="18264-201">Boolean</span></span>|<span data-ttu-id="18264-202">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="18264-202">Toggles syncing contacts.</span></span> <span data-ttu-id="18264-203">Se definido como falsos contatos está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18264-203">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="18264-204">syncTasks</span><span class="sxs-lookup"><span data-stu-id="18264-204">syncTasks</span></span>|<span data-ttu-id="18264-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="18264-205">Boolean</span></span>|<span data-ttu-id="18264-206">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="18264-206">Toggles syncing tasks.</span></span> <span data-ttu-id="18264-207">Se definido como falsos tarefas está desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18264-207">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="18264-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="18264-208">Response</span></span>
<span data-ttu-id="18264-209">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18264-209">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18264-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18264-210">Example</span></span>
### <a name="request"></a><span data-ttu-id="18264-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18264-211">Request</span></span>
<span data-ttu-id="18264-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18264-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="18264-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="18264-213">Response</span></span>
<span data-ttu-id="18264-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18264-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





