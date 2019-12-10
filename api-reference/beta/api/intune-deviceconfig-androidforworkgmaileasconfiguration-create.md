---
title: Criar androidForWorkGmailEasConfiguration
description: Criar um novo objeto androidForWorkGmailEasConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5afbfc13351c8e844763a6535034401c9ed3be4b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39928438"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="6a9ab-103">Criar androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a9ab-103">Create androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="6a9ab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a9ab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a9ab-106">Criar um novo objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6a9ab-106">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a9ab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a9ab-107">Prerequisites</span></span>
<span data-ttu-id="6a9ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a9ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a9ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a9ab-110">Permission type</span></span>|<span data-ttu-id="6a9ab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a9ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a9ab-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a9ab-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a9ab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a9ab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-115">Not supported.</span></span>|
|<span data-ttu-id="6a9ab-116">Application</span><span class="sxs-lookup"><span data-stu-id="6a9ab-116">Application</span></span>|<span data-ttu-id="6a9ab-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a9ab-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a9ab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a9ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6a9ab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a9ab-119">Request headers</span></span>
|<span data-ttu-id="6a9ab-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a9ab-120">Header</span></span>|<span data-ttu-id="6a9ab-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6a9ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a9ab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a9ab-122">Authorization</span></span>|<span data-ttu-id="6a9ab-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a9ab-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a9ab-124">Accept</span></span>|<span data-ttu-id="6a9ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a9ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a9ab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a9ab-126">Request body</span></span>
<span data-ttu-id="6a9ab-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-127">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="6a9ab-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-128">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="6a9ab-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a9ab-129">Property</span></span>|<span data-ttu-id="6a9ab-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a9ab-130">Type</span></span>|<span data-ttu-id="6a9ab-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a9ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a9ab-132">id</span><span class="sxs-lookup"><span data-stu-id="6a9ab-132">id</span></span>|<span data-ttu-id="6a9ab-133">String</span><span class="sxs-lookup"><span data-stu-id="6a9ab-133">String</span></span>|<span data-ttu-id="6a9ab-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-134">Key of the entity.</span></span> <span data-ttu-id="6a9ab-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9ab-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a9ab-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6a9ab-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a9ab-137">DateTimeOffset</span></span>|<span data-ttu-id="6a9ab-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6a9ab-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9ab-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6a9ab-140">roleScopeTagIds</span></span>|<span data-ttu-id="6a9ab-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a9ab-141">String collection</span></span>|<span data-ttu-id="6a9ab-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6a9ab-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9ab-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6a9ab-144">supportsScopeTags</span></span>|<span data-ttu-id="6a9ab-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a9ab-145">Boolean</span></span>|<span data-ttu-id="6a9ab-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6a9ab-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6a9ab-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6a9ab-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-149">This property is read-only.</span></span> <span data-ttu-id="6a9ab-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9ab-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6a9ab-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6a9ab-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6a9ab-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6a9ab-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6a9ab-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9ab-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6a9ab-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6a9ab-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6a9ab-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6a9ab-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6a9ab-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9ab-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6a9ab-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6a9ab-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6a9ab-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6a9ab-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6a9ab-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9ab-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a9ab-163">createdDateTime</span></span>|<span data-ttu-id="6a9ab-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a9ab-164">DateTimeOffset</span></span>|<span data-ttu-id="6a9ab-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-165">DateTime the object was created.</span></span> <span data-ttu-id="6a9ab-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9ab-167">description</span><span class="sxs-lookup"><span data-stu-id="6a9ab-167">description</span></span>|<span data-ttu-id="6a9ab-168">String</span><span class="sxs-lookup"><span data-stu-id="6a9ab-168">String</span></span>|<span data-ttu-id="6a9ab-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6a9ab-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9ab-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6a9ab-171">displayName</span></span>|<span data-ttu-id="6a9ab-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a9ab-172">String</span></span>|<span data-ttu-id="6a9ab-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6a9ab-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9ab-175">versão</span><span class="sxs-lookup"><span data-stu-id="6a9ab-175">version</span></span>|<span data-ttu-id="6a9ab-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6a9ab-176">Int32</span></span>|<span data-ttu-id="6a9ab-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-177">Version of the device configuration.</span></span> <span data-ttu-id="6a9ab-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6a9ab-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6a9ab-179">authenticationMethod</span></span>|[<span data-ttu-id="6a9ab-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6a9ab-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="6a9ab-181">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="6a9ab-182">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6a9ab-182">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="6a9ab-183">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="6a9ab-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="6a9ab-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="6a9ab-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="6a9ab-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="6a9ab-186">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="6a9ab-187">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6a9ab-187">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="6a9ab-188">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="6a9ab-189">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="6a9ab-189">emailAddressSource</span></span>|[<span data-ttu-id="6a9ab-190">UserEmail</span><span class="sxs-lookup"><span data-stu-id="6a9ab-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="6a9ab-191">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6a9ab-192">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6a9ab-192">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="6a9ab-193">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="6a9ab-194">hostName</span><span class="sxs-lookup"><span data-stu-id="6a9ab-194">hostName</span></span>|<span data-ttu-id="6a9ab-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a9ab-195">String</span></span>|<span data-ttu-id="6a9ab-196">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="6a9ab-197">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-197">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="6a9ab-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="6a9ab-198">requireSsl</span></span>|<span data-ttu-id="6a9ab-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a9ab-199">Boolean</span></span>|<span data-ttu-id="6a9ab-200">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="6a9ab-201">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="6a9ab-201">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="6a9ab-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="6a9ab-202">usernameSource</span></span>|[<span data-ttu-id="6a9ab-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="6a9ab-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="6a9ab-204">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="6a9ab-205">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="6a9ab-205">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="6a9ab-206">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="6a9ab-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a9ab-207">Response</span></span>
<span data-ttu-id="6a9ab-208">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-208">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a9ab-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a9ab-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a9ab-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a9ab-210">Request</span></span>
<span data-ttu-id="6a9ab-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1264

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="6a9ab-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a9ab-212">Response</span></span>
<span data-ttu-id="6a9ab-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a9ab-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1436

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
  "id": "2bafc891-c891-2baf-91c8-af2b91c8af2b",
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





