---
title: Criar androidWorkProfileGmailEasConfiguration
description: Criar um novo objeto androidWorkProfileGmailEasConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6941bbec0907c9bbc79650b383b4cae771a32300
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49265553"
---
# <a name="create-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="b3140-103">Criar androidWorkProfileGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3140-103">Create androidWorkProfileGmailEasConfiguration</span></span>

<span data-ttu-id="b3140-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3140-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3140-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3140-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3140-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3140-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3140-107">Criar um novo objeto [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b3140-107">Create a new [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3140-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3140-108">Prerequisites</span></span>
<span data-ttu-id="b3140-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3140-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3140-111">Permission type</span></span>|<span data-ttu-id="b3140-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3140-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3140-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3140-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3140-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3140-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3140-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3140-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3140-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3140-116">Not supported.</span></span>|
|<span data-ttu-id="b3140-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3140-117">Application</span></span>|<span data-ttu-id="b3140-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3140-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3140-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3140-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b3140-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3140-120">Request headers</span></span>
|<span data-ttu-id="b3140-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3140-121">Header</span></span>|<span data-ttu-id="b3140-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b3140-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3140-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3140-123">Authorization</span></span>|<span data-ttu-id="b3140-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3140-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3140-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3140-125">Accept</span></span>|<span data-ttu-id="b3140-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3140-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3140-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3140-127">Request body</span></span>
<span data-ttu-id="b3140-128">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b3140-128">In the request body, supply a JSON representation for the androidWorkProfileGmailEasConfiguration object.</span></span>

<span data-ttu-id="b3140-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b3140-129">The following table shows the properties that are required when you create the androidWorkProfileGmailEasConfiguration.</span></span>

|<span data-ttu-id="b3140-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3140-130">Property</span></span>|<span data-ttu-id="b3140-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3140-131">Type</span></span>|<span data-ttu-id="b3140-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3140-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3140-133">id</span><span class="sxs-lookup"><span data-stu-id="b3140-133">id</span></span>|<span data-ttu-id="b3140-134">String</span><span class="sxs-lookup"><span data-stu-id="b3140-134">String</span></span>|<span data-ttu-id="b3140-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b3140-135">Key of the entity.</span></span> <span data-ttu-id="b3140-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3140-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3140-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b3140-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3140-138">DateTimeOffset</span></span>|<span data-ttu-id="b3140-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b3140-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b3140-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3140-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3140-141">roleScopeTagIds</span></span>|<span data-ttu-id="b3140-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3140-142">String collection</span></span>|<span data-ttu-id="b3140-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b3140-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b3140-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3140-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b3140-145">supportsScopeTags</span></span>|<span data-ttu-id="b3140-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3140-146">Boolean</span></span>|<span data-ttu-id="b3140-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b3140-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b3140-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b3140-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b3140-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b3140-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b3140-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3140-150">This property is read-only.</span></span> <span data-ttu-id="b3140-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3140-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b3140-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b3140-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b3140-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b3140-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b3140-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b3140-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3140-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3140-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b3140-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3140-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b3140-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b3140-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b3140-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3140-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b3140-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b3140-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b3140-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b3140-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b3140-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b3140-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3140-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3140-164">createdDateTime</span></span>|<span data-ttu-id="b3140-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3140-165">DateTimeOffset</span></span>|<span data-ttu-id="b3140-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b3140-166">DateTime the object was created.</span></span> <span data-ttu-id="b3140-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3140-168">description</span><span class="sxs-lookup"><span data-stu-id="b3140-168">description</span></span>|<span data-ttu-id="b3140-169">String</span><span class="sxs-lookup"><span data-stu-id="b3140-169">String</span></span>|<span data-ttu-id="b3140-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b3140-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b3140-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3140-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b3140-172">displayName</span></span>|<span data-ttu-id="b3140-173">String</span><span class="sxs-lookup"><span data-stu-id="b3140-173">String</span></span>|<span data-ttu-id="b3140-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b3140-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b3140-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3140-176">versão</span><span class="sxs-lookup"><span data-stu-id="b3140-176">version</span></span>|<span data-ttu-id="b3140-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b3140-177">Int32</span></span>|<span data-ttu-id="b3140-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b3140-178">Version of the device configuration.</span></span> <span data-ttu-id="b3140-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3140-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b3140-180">authenticationMethod</span></span>|[<span data-ttu-id="b3140-181">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b3140-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="b3140-182">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="b3140-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="b3140-183">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b3140-183">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="b3140-184">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="b3140-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="b3140-185">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="b3140-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="b3140-186">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="b3140-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="b3140-187">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="b3140-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="b3140-188">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b3140-188">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="b3140-189">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="b3140-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="b3140-190">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="b3140-190">emailAddressSource</span></span>|[<span data-ttu-id="b3140-191">UserEmail</span><span class="sxs-lookup"><span data-stu-id="b3140-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="b3140-192">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b3140-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b3140-193">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b3140-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="b3140-194">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="b3140-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="b3140-195">hostName</span><span class="sxs-lookup"><span data-stu-id="b3140-195">hostName</span></span>|<span data-ttu-id="b3140-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3140-196">String</span></span>|<span data-ttu-id="b3140-197">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="b3140-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="b3140-198">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-198">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="b3140-199">requireSsl</span><span class="sxs-lookup"><span data-stu-id="b3140-199">requireSsl</span></span>|<span data-ttu-id="b3140-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3140-200">Boolean</span></span>|<span data-ttu-id="b3140-201">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="b3140-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="b3140-202">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="b3140-202">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="b3140-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="b3140-203">usernameSource</span></span>|[<span data-ttu-id="b3140-204">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="b3140-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="b3140-205">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b3140-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="b3140-206">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="b3140-206">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="b3140-207">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="b3140-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="b3140-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3140-208">Response</span></span>
<span data-ttu-id="b3140-209">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3140-209">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3140-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3140-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3140-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3140-211">Request</span></span>
<span data-ttu-id="b3140-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3140-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1268

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="b3140-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3140-213">Response</span></span>
<span data-ttu-id="b3140-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3140-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1440

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "id": "a4a44bb5-4bb5-a4a4-b54b-a4a4b54ba4a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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




