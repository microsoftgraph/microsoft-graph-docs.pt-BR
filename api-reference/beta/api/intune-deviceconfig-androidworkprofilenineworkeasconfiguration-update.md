---
title: Atualizar androidWorkProfileNineWorkEasConfiguration
description: Atualiza as propriedades de um objeto androidWorkProfileNineWorkEasConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 957601c618c5e5c0d7ed8bd5c2cd7be29fe0d0a8
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37168632"
---
# <a name="update-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="38c4c-103">Atualizar androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="38c4c-103">Update androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="38c4c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="38c4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38c4c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38c4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38c4c-106">Atualiza as propriedades de um objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="38c4c-106">Update the properties of a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38c4c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38c4c-107">Prerequisites</span></span>
<span data-ttu-id="38c4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38c4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38c4c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38c4c-110">Permission type</span></span>|<span data-ttu-id="38c4c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38c4c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38c4c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38c4c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38c4c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38c4c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38c4c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38c4c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38c4c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38c4c-115">Not supported.</span></span>|
|<span data-ttu-id="38c4c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38c4c-116">Application</span></span>|<span data-ttu-id="38c4c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38c4c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38c4c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38c4c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="38c4c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38c4c-119">Request headers</span></span>
|<span data-ttu-id="38c4c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38c4c-120">Header</span></span>|<span data-ttu-id="38c4c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="38c4c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38c4c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="38c4c-122">Authorization</span></span>|<span data-ttu-id="38c4c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38c4c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38c4c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38c4c-124">Accept</span></span>|<span data-ttu-id="38c4c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38c4c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38c4c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38c4c-126">Request body</span></span>
<span data-ttu-id="38c4c-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="38c4c-127">In the request body, supply a JSON representation for the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="38c4c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38c4c-128">The following table shows the properties that are required when you create the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="38c4c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38c4c-129">Property</span></span>|<span data-ttu-id="38c4c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="38c4c-130">Type</span></span>|<span data-ttu-id="38c4c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="38c4c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38c4c-132">id</span><span class="sxs-lookup"><span data-stu-id="38c4c-132">id</span></span>|<span data-ttu-id="38c4c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38c4c-133">String</span></span>|<span data-ttu-id="38c4c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="38c4c-134">Key of the entity.</span></span> <span data-ttu-id="38c4c-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38c4c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38c4c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="38c4c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38c4c-137">DateTimeOffset</span></span>|<span data-ttu-id="38c4c-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="38c4c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="38c4c-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38c4c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="38c4c-140">roleScopeTagIds</span></span>|<span data-ttu-id="38c4c-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="38c4c-141">String collection</span></span>|<span data-ttu-id="38c4c-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="38c4c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="38c4c-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38c4c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="38c4c-144">supportsScopeTags</span></span>|<span data-ttu-id="38c4c-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="38c4c-145">Boolean</span></span>|<span data-ttu-id="38c4c-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="38c4c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="38c4c-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="38c4c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="38c4c-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="38c4c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="38c4c-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38c4c-149">This property is read-only.</span></span> <span data-ttu-id="38c4c-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38c4c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="38c4c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="38c4c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="38c4c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="38c4c-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="38c4c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="38c4c-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38c4c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="38c4c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="38c4c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="38c4c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="38c4c-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="38c4c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="38c4c-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38c4c-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="38c4c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="38c4c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="38c4c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="38c4c-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="38c4c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="38c4c-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38c4c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38c4c-163">createdDateTime</span></span>|<span data-ttu-id="38c4c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38c4c-164">DateTimeOffset</span></span>|<span data-ttu-id="38c4c-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="38c4c-165">DateTime the object was created.</span></span> <span data-ttu-id="38c4c-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38c4c-167">descrição</span><span class="sxs-lookup"><span data-stu-id="38c4c-167">description</span></span>|<span data-ttu-id="38c4c-168">String</span><span class="sxs-lookup"><span data-stu-id="38c4c-168">String</span></span>|<span data-ttu-id="38c4c-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38c4c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="38c4c-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38c4c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="38c4c-171">displayName</span></span>|<span data-ttu-id="38c4c-172">String</span><span class="sxs-lookup"><span data-stu-id="38c4c-172">String</span></span>|<span data-ttu-id="38c4c-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38c4c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="38c4c-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38c4c-175">versão</span><span class="sxs-lookup"><span data-stu-id="38c4c-175">version</span></span>|<span data-ttu-id="38c4c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="38c4c-176">Int32</span></span>|<span data-ttu-id="38c4c-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38c4c-177">Version of the device configuration.</span></span> <span data-ttu-id="38c4c-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38c4c-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="38c4c-179">authenticationMethod</span></span>|[<span data-ttu-id="38c4c-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="38c4c-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="38c4c-181">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="38c4c-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="38c4c-182">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="38c4c-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="38c4c-183">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="38c4c-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="38c4c-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="38c4c-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="38c4c-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="38c4c-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="38c4c-186">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="38c4c-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="38c4c-187">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="38c4c-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="38c4c-188">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="38c4c-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="38c4c-189">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="38c4c-189">emailAddressSource</span></span>|[<span data-ttu-id="38c4c-190">UserEmail</span><span class="sxs-lookup"><span data-stu-id="38c4c-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="38c4c-191">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38c4c-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="38c4c-192">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="38c4c-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="38c4c-193">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="38c4c-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="38c4c-194">hostName</span><span class="sxs-lookup"><span data-stu-id="38c4c-194">hostName</span></span>|<span data-ttu-id="38c4c-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38c4c-195">String</span></span>|<span data-ttu-id="38c4c-196">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="38c4c-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="38c4c-197">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="38c4c-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="38c4c-198">requireSsl</span></span>|<span data-ttu-id="38c4c-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="38c4c-199">Boolean</span></span>|<span data-ttu-id="38c4c-200">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="38c4c-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="38c4c-201">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="38c4c-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="38c4c-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="38c4c-202">usernameSource</span></span>|[<span data-ttu-id="38c4c-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="38c4c-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="38c4c-204">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38c4c-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="38c4c-205">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="38c4c-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="38c4c-206">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="38c4c-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="38c4c-207">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="38c4c-207">syncCalendar</span></span>|<span data-ttu-id="38c4c-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="38c4c-208">Boolean</span></span>|<span data-ttu-id="38c4c-209">Alterna a sincronização do calendário.</span><span class="sxs-lookup"><span data-stu-id="38c4c-209">Toggles syncing the calendar.</span></span> <span data-ttu-id="38c4c-210">Se definido como falso, o calendário será desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38c4c-210">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="38c4c-211">syncContacts</span><span class="sxs-lookup"><span data-stu-id="38c4c-211">syncContacts</span></span>|<span data-ttu-id="38c4c-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="38c4c-212">Boolean</span></span>|<span data-ttu-id="38c4c-213">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="38c4c-213">Toggles syncing contacts.</span></span> <span data-ttu-id="38c4c-214">Se definido como falso, os contatos serão desativados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38c4c-214">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="38c4c-215">syncTasks</span><span class="sxs-lookup"><span data-stu-id="38c4c-215">syncTasks</span></span>|<span data-ttu-id="38c4c-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="38c4c-216">Boolean</span></span>|<span data-ttu-id="38c4c-217">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="38c4c-217">Toggles syncing tasks.</span></span> <span data-ttu-id="38c4c-218">Se definido como falso, as tarefas serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38c4c-218">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="38c4c-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="38c4c-219">Response</span></span>
<span data-ttu-id="38c4c-220">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38c4c-220">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38c4c-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38c4c-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="38c4c-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38c4c-222">Request</span></span>
<span data-ttu-id="38c4c-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38c4c-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1343

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
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
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```

### <a name="response"></a><span data-ttu-id="38c4c-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="38c4c-224">Response</span></span>
<span data-ttu-id="38c4c-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38c4c-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1515

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
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
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```




