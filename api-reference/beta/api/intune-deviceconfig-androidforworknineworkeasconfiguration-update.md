---
title: Atualizar androidForWorkNineWorkEasConfiguration
description: Atualiza as propriedades de um objeto androidForWorkNineWorkEasConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e16f44832164e3bdd6822a6a675b4623161e12d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39954759"
---
# <a name="update-androidforworknineworkeasconfiguration"></a><span data-ttu-id="d525e-103">Atualizar androidForWorkNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="d525e-103">Update androidForWorkNineWorkEasConfiguration</span></span>

> <span data-ttu-id="d525e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d525e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d525e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d525e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d525e-106">Atualiza as propriedades de um objeto [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d525e-106">Update the properties of a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d525e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d525e-107">Prerequisites</span></span>
<span data-ttu-id="d525e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d525e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d525e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d525e-110">Permission type</span></span>|<span data-ttu-id="d525e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d525e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d525e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d525e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d525e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d525e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d525e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d525e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d525e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d525e-115">Not supported.</span></span>|
|<span data-ttu-id="d525e-116">Application</span><span class="sxs-lookup"><span data-stu-id="d525e-116">Application</span></span>|<span data-ttu-id="d525e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d525e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d525e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d525e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d525e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d525e-119">Request headers</span></span>
|<span data-ttu-id="d525e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d525e-120">Header</span></span>|<span data-ttu-id="d525e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d525e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d525e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d525e-122">Authorization</span></span>|<span data-ttu-id="d525e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d525e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d525e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d525e-124">Accept</span></span>|<span data-ttu-id="d525e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d525e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d525e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d525e-126">Request body</span></span>
<span data-ttu-id="d525e-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d525e-127">In the request body, supply a JSON representation for the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="d525e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d525e-128">The following table shows the properties that are required when you create the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="d525e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d525e-129">Property</span></span>|<span data-ttu-id="d525e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d525e-130">Type</span></span>|<span data-ttu-id="d525e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d525e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d525e-132">id</span><span class="sxs-lookup"><span data-stu-id="d525e-132">id</span></span>|<span data-ttu-id="d525e-133">String</span><span class="sxs-lookup"><span data-stu-id="d525e-133">String</span></span>|<span data-ttu-id="d525e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d525e-134">Key of the entity.</span></span> <span data-ttu-id="d525e-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d525e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d525e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d525e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d525e-137">DateTimeOffset</span></span>|<span data-ttu-id="d525e-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d525e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d525e-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d525e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d525e-140">roleScopeTagIds</span></span>|<span data-ttu-id="d525e-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d525e-141">String collection</span></span>|<span data-ttu-id="d525e-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d525e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d525e-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d525e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d525e-144">supportsScopeTags</span></span>|<span data-ttu-id="d525e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d525e-145">Boolean</span></span>|<span data-ttu-id="d525e-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d525e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d525e-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d525e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d525e-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d525e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d525e-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d525e-149">This property is read-only.</span></span> <span data-ttu-id="d525e-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d525e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d525e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d525e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d525e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d525e-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="d525e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d525e-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d525e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d525e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d525e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d525e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d525e-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="d525e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d525e-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d525e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d525e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d525e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d525e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d525e-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="d525e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d525e-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d525e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d525e-163">createdDateTime</span></span>|<span data-ttu-id="d525e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d525e-164">DateTimeOffset</span></span>|<span data-ttu-id="d525e-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d525e-165">DateTime the object was created.</span></span> <span data-ttu-id="d525e-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d525e-167">description</span><span class="sxs-lookup"><span data-stu-id="d525e-167">description</span></span>|<span data-ttu-id="d525e-168">String</span><span class="sxs-lookup"><span data-stu-id="d525e-168">String</span></span>|<span data-ttu-id="d525e-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d525e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d525e-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d525e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d525e-171">displayName</span></span>|<span data-ttu-id="d525e-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d525e-172">String</span></span>|<span data-ttu-id="d525e-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d525e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d525e-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d525e-175">versão</span><span class="sxs-lookup"><span data-stu-id="d525e-175">version</span></span>|<span data-ttu-id="d525e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d525e-176">Int32</span></span>|<span data-ttu-id="d525e-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d525e-177">Version of the device configuration.</span></span> <span data-ttu-id="d525e-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d525e-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d525e-179">authenticationMethod</span></span>|[<span data-ttu-id="d525e-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d525e-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="d525e-181">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="d525e-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="d525e-182">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d525e-182">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="d525e-183">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="d525e-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d525e-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="d525e-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="d525e-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="d525e-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="d525e-186">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="d525e-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="d525e-187">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d525e-187">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="d525e-188">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="d525e-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="d525e-189">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="d525e-189">emailAddressSource</span></span>|[<span data-ttu-id="d525e-190">UserEmail</span><span class="sxs-lookup"><span data-stu-id="d525e-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d525e-191">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d525e-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d525e-192">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d525e-192">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="d525e-193">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d525e-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d525e-194">hostName</span><span class="sxs-lookup"><span data-stu-id="d525e-194">hostName</span></span>|<span data-ttu-id="d525e-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d525e-195">String</span></span>|<span data-ttu-id="d525e-196">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="d525e-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="d525e-197">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-197">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="d525e-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="d525e-198">requireSsl</span></span>|<span data-ttu-id="d525e-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="d525e-199">Boolean</span></span>|<span data-ttu-id="d525e-200">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="d525e-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="d525e-201">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d525e-201">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="d525e-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d525e-202">usernameSource</span></span>|[<span data-ttu-id="d525e-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="d525e-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="d525e-204">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d525e-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d525e-205">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d525e-205">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="d525e-206">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d525e-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d525e-207">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="d525e-207">syncCalendar</span></span>|<span data-ttu-id="d525e-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="d525e-208">Boolean</span></span>|<span data-ttu-id="d525e-209">Alterna a sincronização do calendário.</span><span class="sxs-lookup"><span data-stu-id="d525e-209">Toggles syncing the calendar.</span></span> <span data-ttu-id="d525e-210">Se definido como falso, o calendário será desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d525e-210">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="d525e-211">syncContacts</span><span class="sxs-lookup"><span data-stu-id="d525e-211">syncContacts</span></span>|<span data-ttu-id="d525e-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="d525e-212">Boolean</span></span>|<span data-ttu-id="d525e-213">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="d525e-213">Toggles syncing contacts.</span></span> <span data-ttu-id="d525e-214">Se definido como falso, os contatos serão desativados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d525e-214">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="d525e-215">syncTasks</span><span class="sxs-lookup"><span data-stu-id="d525e-215">syncTasks</span></span>|<span data-ttu-id="d525e-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="d525e-216">Boolean</span></span>|<span data-ttu-id="d525e-217">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d525e-217">Toggles syncing tasks.</span></span> <span data-ttu-id="d525e-218">Se definido como falso, as tarefas serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d525e-218">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="d525e-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="d525e-219">Response</span></span>
<span data-ttu-id="d525e-220">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d525e-220">If successful, this method returns a `200 OK` response code and an updated [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d525e-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d525e-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="d525e-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d525e-222">Request</span></span>
<span data-ttu-id="d525e-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d525e-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1339

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="d525e-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="d525e-224">Response</span></span>
<span data-ttu-id="d525e-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d525e-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1511

{
  "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
  "id": "f8ef19e0-19e0-f8ef-e019-eff8e019eff8",
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





