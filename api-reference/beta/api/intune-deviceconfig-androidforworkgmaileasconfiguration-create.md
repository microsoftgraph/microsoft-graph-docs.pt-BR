---
title: Criar androidForWorkGmailEasConfiguration
description: Criar um novo objeto androidForWorkGmailEasConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10244a8fa59b9c920f315546b723e5a9cf096613
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759292"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="d9d69-103">Criar androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9d69-103">Create androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="d9d69-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9d69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9d69-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9d69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9d69-106">Criar um novo objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d9d69-106">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9d69-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9d69-107">Prerequisites</span></span>
<span data-ttu-id="d9d69-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9d69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9d69-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9d69-110">Permission type</span></span>|<span data-ttu-id="d9d69-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9d69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9d69-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9d69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9d69-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9d69-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9d69-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9d69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9d69-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9d69-115">Not supported.</span></span>|
|<span data-ttu-id="d9d69-116">Application</span><span class="sxs-lookup"><span data-stu-id="d9d69-116">Application</span></span>|<span data-ttu-id="d9d69-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9d69-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9d69-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9d69-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d9d69-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d69-119">Request headers</span></span>
|<span data-ttu-id="d9d69-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9d69-120">Header</span></span>|<span data-ttu-id="d9d69-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d9d69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9d69-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9d69-122">Authorization</span></span>|<span data-ttu-id="d9d69-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9d69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9d69-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9d69-124">Accept</span></span>|<span data-ttu-id="d9d69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9d69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9d69-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d69-126">Request body</span></span>
<span data-ttu-id="d9d69-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d9d69-127">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="d9d69-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d9d69-128">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="d9d69-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9d69-129">Property</span></span>|<span data-ttu-id="d9d69-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9d69-130">Type</span></span>|<span data-ttu-id="d9d69-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9d69-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9d69-132">id</span><span class="sxs-lookup"><span data-stu-id="d9d69-132">id</span></span>|<span data-ttu-id="d9d69-133">String</span><span class="sxs-lookup"><span data-stu-id="d9d69-133">String</span></span>|<span data-ttu-id="d9d69-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d9d69-134">Key of the entity.</span></span> <span data-ttu-id="d9d69-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9d69-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9d69-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d9d69-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9d69-137">DateTimeOffset</span></span>|<span data-ttu-id="d9d69-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d9d69-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d9d69-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9d69-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d9d69-140">roleScopeTagIds</span></span>|<span data-ttu-id="d9d69-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9d69-141">String collection</span></span>|<span data-ttu-id="d9d69-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d9d69-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d9d69-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9d69-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d9d69-144">supportsScopeTags</span></span>|<span data-ttu-id="d9d69-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9d69-145">Boolean</span></span>|<span data-ttu-id="d9d69-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d9d69-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d9d69-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d9d69-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d9d69-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d9d69-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d9d69-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9d69-149">This property is read-only.</span></span> <span data-ttu-id="d9d69-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9d69-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d9d69-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d9d69-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d9d69-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d9d69-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="d9d69-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d9d69-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9d69-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d9d69-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d9d69-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d9d69-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d9d69-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="d9d69-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d9d69-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9d69-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d9d69-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d9d69-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d9d69-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d9d69-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="d9d69-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d9d69-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9d69-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9d69-163">createdDateTime</span></span>|<span data-ttu-id="d9d69-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9d69-164">DateTimeOffset</span></span>|<span data-ttu-id="d9d69-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d9d69-165">DateTime the object was created.</span></span> <span data-ttu-id="d9d69-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9d69-167">description</span><span class="sxs-lookup"><span data-stu-id="d9d69-167">description</span></span>|<span data-ttu-id="d9d69-168">String</span><span class="sxs-lookup"><span data-stu-id="d9d69-168">String</span></span>|<span data-ttu-id="d9d69-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9d69-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d9d69-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9d69-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d9d69-171">displayName</span></span>|<span data-ttu-id="d9d69-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9d69-172">String</span></span>|<span data-ttu-id="d9d69-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9d69-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d9d69-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9d69-175">versão</span><span class="sxs-lookup"><span data-stu-id="d9d69-175">version</span></span>|<span data-ttu-id="d9d69-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d9d69-176">Int32</span></span>|<span data-ttu-id="d9d69-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9d69-177">Version of the device configuration.</span></span> <span data-ttu-id="d9d69-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9d69-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d9d69-179">authenticationMethod</span></span>|[<span data-ttu-id="d9d69-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d9d69-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="d9d69-181">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="d9d69-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="d9d69-182">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d9d69-182">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="d9d69-183">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="d9d69-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="d9d69-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="d9d69-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="d9d69-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="d9d69-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="d9d69-186">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="d9d69-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="d9d69-187">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d9d69-187">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="d9d69-188">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="d9d69-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="d9d69-189">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="d9d69-189">emailAddressSource</span></span>|[<span data-ttu-id="d9d69-190">UserEmail</span><span class="sxs-lookup"><span data-stu-id="d9d69-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="d9d69-191">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9d69-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d9d69-192">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d9d69-192">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="d9d69-193">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d9d69-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="d9d69-194">hostName</span><span class="sxs-lookup"><span data-stu-id="d9d69-194">hostName</span></span>|<span data-ttu-id="d9d69-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9d69-195">String</span></span>|<span data-ttu-id="d9d69-196">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="d9d69-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="d9d69-197">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-197">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="d9d69-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="d9d69-198">requireSsl</span></span>|<span data-ttu-id="d9d69-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9d69-199">Boolean</span></span>|<span data-ttu-id="d9d69-200">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="d9d69-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="d9d69-201">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="d9d69-201">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="d9d69-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="d9d69-202">usernameSource</span></span>|[<span data-ttu-id="d9d69-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="d9d69-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="d9d69-204">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9d69-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="d9d69-205">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="d9d69-205">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="d9d69-206">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="d9d69-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="d9d69-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9d69-207">Response</span></span>
<span data-ttu-id="d9d69-208">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9d69-208">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9d69-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9d69-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9d69-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9d69-210">Request</span></span>
<span data-ttu-id="d9d69-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9d69-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d9d69-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9d69-212">Response</span></span>
<span data-ttu-id="d9d69-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9d69-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




