---
title: Criar androidForWorkGmailEasConfiguration
description: Crie um novo objeto androidForWorkGmailEasConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf724d7d3522d780c145238327a4070f8d0ededa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130277"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="ef404-103">Criar androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="ef404-103">Create androidForWorkGmailEasConfiguration</span></span>

<span data-ttu-id="ef404-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef404-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef404-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef404-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef404-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef404-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef404-107">Crie um novo [objeto androidForWorkGmailEasConfiguration.](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-107">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef404-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef404-108">Prerequisites</span></span>
<span data-ttu-id="ef404-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef404-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef404-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef404-111">Permission type</span></span>|<span data-ttu-id="ef404-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef404-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef404-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef404-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef404-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef404-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef404-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef404-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef404-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef404-116">Not supported.</span></span>|
|<span data-ttu-id="ef404-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef404-117">Application</span></span>|<span data-ttu-id="ef404-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef404-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef404-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef404-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ef404-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef404-120">Request headers</span></span>
|<span data-ttu-id="ef404-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef404-121">Header</span></span>|<span data-ttu-id="ef404-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ef404-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef404-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef404-123">Authorization</span></span>|<span data-ttu-id="ef404-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef404-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef404-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef404-125">Accept</span></span>|<span data-ttu-id="ef404-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef404-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef404-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef404-127">Request body</span></span>
<span data-ttu-id="ef404-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ef404-128">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="ef404-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o androidForWorkGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ef404-129">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="ef404-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef404-130">Property</span></span>|<span data-ttu-id="ef404-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef404-131">Type</span></span>|<span data-ttu-id="ef404-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef404-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef404-133">id</span><span class="sxs-lookup"><span data-stu-id="ef404-133">id</span></span>|<span data-ttu-id="ef404-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef404-134">String</span></span>|<span data-ttu-id="ef404-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ef404-135">Key of the entity.</span></span> <span data-ttu-id="ef404-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef404-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef404-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ef404-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef404-138">DateTimeOffset</span></span>|<span data-ttu-id="ef404-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ef404-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ef404-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef404-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef404-141">roleScopeTagIds</span></span>|<span data-ttu-id="ef404-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef404-142">String collection</span></span>|<span data-ttu-id="ef404-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="ef404-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ef404-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef404-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ef404-145">supportsScopeTags</span></span>|<span data-ttu-id="ef404-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="ef404-146">Boolean</span></span>|<span data-ttu-id="ef404-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ef404-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ef404-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ef404-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ef404-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ef404-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ef404-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef404-150">This property is read-only.</span></span> <span data-ttu-id="ef404-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef404-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ef404-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ef404-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ef404-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ef404-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ef404-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ef404-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef404-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef404-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ef404-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ef404-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ef404-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ef404-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ef404-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef404-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ef404-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ef404-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ef404-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ef404-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="ef404-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ef404-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef404-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef404-164">createdDateTime</span></span>|<span data-ttu-id="ef404-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef404-165">DateTimeOffset</span></span>|<span data-ttu-id="ef404-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ef404-166">DateTime the object was created.</span></span> <span data-ttu-id="ef404-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef404-168">descrição</span><span class="sxs-lookup"><span data-stu-id="ef404-168">description</span></span>|<span data-ttu-id="ef404-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef404-169">String</span></span>|<span data-ttu-id="ef404-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef404-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef404-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef404-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ef404-172">displayName</span></span>|<span data-ttu-id="ef404-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef404-173">String</span></span>|<span data-ttu-id="ef404-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef404-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef404-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef404-176">versão</span><span class="sxs-lookup"><span data-stu-id="ef404-176">version</span></span>|<span data-ttu-id="ef404-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ef404-177">Int32</span></span>|<span data-ttu-id="ef404-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef404-178">Version of the device configuration.</span></span> <span data-ttu-id="ef404-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef404-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ef404-180">authenticationMethod</span></span>|[<span data-ttu-id="ef404-181">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ef404-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="ef404-182">Método de autenticação para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="ef404-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="ef404-183">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ef404-183">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="ef404-184">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="ef404-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ef404-185">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="ef404-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="ef404-186">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="ef404-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="ef404-187">A duração do tempo em que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="ef404-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="ef404-188">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ef404-188">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="ef404-189">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="ef404-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="ef404-190">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="ef404-190">emailAddressSource</span></span>|[<span data-ttu-id="ef404-191">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="ef404-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="ef404-192">Atributo de email que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef404-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ef404-193">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ef404-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="ef404-194">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="ef404-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="ef404-195">hostName</span><span class="sxs-lookup"><span data-stu-id="ef404-195">hostName</span></span>|<span data-ttu-id="ef404-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef404-196">String</span></span>|<span data-ttu-id="ef404-197">Local do Exchange (URL) ao que o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="ef404-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="ef404-198">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-198">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="ef404-199">requireSsl</span><span class="sxs-lookup"><span data-stu-id="ef404-199">requireSsl</span></span>|<span data-ttu-id="ef404-200">Booleano</span><span class="sxs-lookup"><span data-stu-id="ef404-200">Boolean</span></span>|<span data-ttu-id="ef404-201">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="ef404-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="ef404-202">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ef404-202">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="ef404-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="ef404-203">usernameSource</span></span>|[<span data-ttu-id="ef404-204">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="ef404-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="ef404-205">Atributo username que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef404-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ef404-206">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="ef404-206">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="ef404-207">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="ef404-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="ef404-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef404-208">Response</span></span>
<span data-ttu-id="ef404-209">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef404-209">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef404-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef404-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef404-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef404-211">Request</span></span>
<span data-ttu-id="ef404-212">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef404-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ef404-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef404-213">Response</span></span>
<span data-ttu-id="ef404-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef404-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




