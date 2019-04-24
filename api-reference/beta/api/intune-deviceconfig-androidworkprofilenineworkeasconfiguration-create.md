---
title: Criar androidWorkProfileNineWorkEasConfiguration
description: Criar um novo objeto androidWorkProfileNineWorkEasConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73892115e393fd18e312bf6a5a7bd2c0d51da68c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32474385"
---
# <a name="create-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="3b9d9-103">Criar androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="3b9d9-103">Create androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="3b9d9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b9d9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b9d9-106">Criar um novo objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3b9d9-106">Create a new [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b9d9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b9d9-107">Prerequisites</span></span>
<span data-ttu-id="3b9d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b9d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b9d9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b9d9-110">Permission type</span></span>|<span data-ttu-id="3b9d9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b9d9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b9d9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b9d9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b9d9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b9d9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-115">Not supported.</span></span>|
|<span data-ttu-id="3b9d9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b9d9-116">Application</span></span>|<span data-ttu-id="3b9d9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b9d9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b9d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3b9d9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b9d9-119">Request headers</span></span>
|<span data-ttu-id="3b9d9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b9d9-120">Header</span></span>|<span data-ttu-id="3b9d9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3b9d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b9d9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b9d9-122">Authorization</span></span>|<span data-ttu-id="3b9d9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b9d9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b9d9-124">Accept</span></span>|<span data-ttu-id="3b9d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b9d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b9d9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b9d9-126">Request body</span></span>
<span data-ttu-id="3b9d9-127">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-127">In the request body, supply a JSON representation for the androidWorkProfileNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="3b9d9-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-128">The following table shows the properties that are required when you create the androidWorkProfileNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="3b9d9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b9d9-129">Property</span></span>|<span data-ttu-id="3b9d9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b9d9-130">Type</span></span>|<span data-ttu-id="3b9d9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b9d9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b9d9-132">id</span><span class="sxs-lookup"><span data-stu-id="3b9d9-132">id</span></span>|<span data-ttu-id="3b9d9-133">String</span><span class="sxs-lookup"><span data-stu-id="3b9d9-133">String</span></span>|<span data-ttu-id="3b9d9-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-134">Key of the entity.</span></span> <span data-ttu-id="3b9d9-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b9d9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b9d9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3b9d9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b9d9-137">DateTimeOffset</span></span>|<span data-ttu-id="3b9d9-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3b9d9-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b9d9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3b9d9-140">roleScopeTagIds</span></span>|<span data-ttu-id="3b9d9-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b9d9-141">String collection</span></span>|<span data-ttu-id="3b9d9-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3b9d9-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b9d9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3b9d9-144">supportsScopeTags</span></span>|<span data-ttu-id="3b9d9-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b9d9-145">Boolean</span></span>|<span data-ttu-id="3b9d9-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3b9d9-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3b9d9-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3b9d9-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-149">This property is read-only.</span></span> <span data-ttu-id="3b9d9-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b9d9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b9d9-151">createdDateTime</span></span>|<span data-ttu-id="3b9d9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b9d9-152">DateTimeOffset</span></span>|<span data-ttu-id="3b9d9-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-153">DateTime the object was created.</span></span> <span data-ttu-id="3b9d9-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b9d9-155">description</span><span class="sxs-lookup"><span data-stu-id="3b9d9-155">description</span></span>|<span data-ttu-id="3b9d9-156">String</span><span class="sxs-lookup"><span data-stu-id="3b9d9-156">String</span></span>|<span data-ttu-id="3b9d9-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3b9d9-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b9d9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3b9d9-159">displayName</span></span>|<span data-ttu-id="3b9d9-160">String</span><span class="sxs-lookup"><span data-stu-id="3b9d9-160">String</span></span>|<span data-ttu-id="3b9d9-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3b9d9-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b9d9-163">versão</span><span class="sxs-lookup"><span data-stu-id="3b9d9-163">version</span></span>|<span data-ttu-id="3b9d9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3b9d9-164">Int32</span></span>|<span data-ttu-id="3b9d9-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-165">Version of the device configuration.</span></span> <span data-ttu-id="3b9d9-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b9d9-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3b9d9-167">authenticationMethod</span></span>|[<span data-ttu-id="3b9d9-168">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="3b9d9-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="3b9d9-169">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="3b9d9-170">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3b9d9-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="3b9d9-171">Os valores possíveis são: `usernameAndPassword` e `certificate`.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="3b9d9-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="3b9d9-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="3b9d9-173">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="3b9d9-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="3b9d9-174">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="3b9d9-175">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3b9d9-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="3b9d9-176">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="3b9d9-177">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="3b9d9-177">emailAddressSource</span></span>|[<span data-ttu-id="3b9d9-178">userEmail</span><span class="sxs-lookup"><span data-stu-id="3b9d9-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="3b9d9-179">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="3b9d9-180">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3b9d9-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="3b9d9-181">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="3b9d9-182">hostName</span><span class="sxs-lookup"><span data-stu-id="3b9d9-182">hostName</span></span>|<span data-ttu-id="3b9d9-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b9d9-183">String</span></span>|<span data-ttu-id="3b9d9-184">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="3b9d9-185">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="3b9d9-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="3b9d9-186">requireSsl</span></span>|<span data-ttu-id="3b9d9-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b9d9-187">Boolean</span></span>|<span data-ttu-id="3b9d9-188">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="3b9d9-189">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="3b9d9-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="3b9d9-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="3b9d9-190">usernameSource</span></span>|[<span data-ttu-id="3b9d9-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="3b9d9-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="3b9d9-192">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="3b9d9-193">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="3b9d9-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="3b9d9-194">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="3b9d9-195">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="3b9d9-195">syncCalendar</span></span>|<span data-ttu-id="3b9d9-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b9d9-196">Boolean</span></span>|<span data-ttu-id="3b9d9-197">Alterna a sincronização do calendário.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-197">Toggles syncing the calendar.</span></span> <span data-ttu-id="3b9d9-198">Se definido como falso, o calendário será desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-198">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="3b9d9-199">syncContacts</span><span class="sxs-lookup"><span data-stu-id="3b9d9-199">syncContacts</span></span>|<span data-ttu-id="3b9d9-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b9d9-200">Boolean</span></span>|<span data-ttu-id="3b9d9-201">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-201">Toggles syncing contacts.</span></span> <span data-ttu-id="3b9d9-202">Se definido como falso, os contatos serão desativados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-202">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="3b9d9-203">syncTasks</span><span class="sxs-lookup"><span data-stu-id="3b9d9-203">syncTasks</span></span>|<span data-ttu-id="3b9d9-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b9d9-204">Boolean</span></span>|<span data-ttu-id="3b9d9-205">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-205">Toggles syncing tasks.</span></span> <span data-ttu-id="3b9d9-206">Se definido como falso, as tarefas serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-206">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="3b9d9-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b9d9-207">Response</span></span>
<span data-ttu-id="3b9d9-208">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b9d9-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b9d9-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b9d9-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b9d9-210">Request</span></span>
<span data-ttu-id="3b9d9-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3b9d9-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b9d9-212">Response</span></span>
<span data-ttu-id="3b9d9-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b9d9-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





