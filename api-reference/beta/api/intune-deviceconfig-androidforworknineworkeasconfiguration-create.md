---
title: Criar androidForWorkNineWorkEasConfiguration
description: Criar um novo objeto androidForWorkNineWorkEasConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b5b5d7cc1d93064801b5069a82bee66d145454c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43435957"
---
# <a name="create-androidforworknineworkeasconfiguration"></a><span data-ttu-id="0bf68-103">Criar androidForWorkNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="0bf68-103">Create androidForWorkNineWorkEasConfiguration</span></span>

<span data-ttu-id="0bf68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bf68-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0bf68-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0bf68-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bf68-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0bf68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bf68-107">Criar um novo objeto [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0bf68-107">Create a new [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0bf68-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0bf68-108">Prerequisites</span></span>
<span data-ttu-id="0bf68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bf68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bf68-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bf68-111">Permission type</span></span>|<span data-ttu-id="0bf68-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0bf68-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bf68-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bf68-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bf68-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bf68-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0bf68-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bf68-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bf68-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bf68-116">Not supported.</span></span>|
|<span data-ttu-id="0bf68-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0bf68-117">Application</span></span>|<span data-ttu-id="0bf68-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bf68-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bf68-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bf68-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0bf68-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bf68-120">Request headers</span></span>
|<span data-ttu-id="0bf68-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0bf68-121">Header</span></span>|<span data-ttu-id="0bf68-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0bf68-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bf68-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bf68-123">Authorization</span></span>|<span data-ttu-id="0bf68-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bf68-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bf68-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0bf68-125">Accept</span></span>|<span data-ttu-id="0bf68-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bf68-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bf68-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bf68-127">Request body</span></span>
<span data-ttu-id="0bf68-128">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0bf68-128">In the request body, supply a JSON representation for the androidForWorkNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="0bf68-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0bf68-129">The following table shows the properties that are required when you create the androidForWorkNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="0bf68-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0bf68-130">Property</span></span>|<span data-ttu-id="0bf68-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0bf68-131">Type</span></span>|<span data-ttu-id="0bf68-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bf68-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bf68-133">id</span><span class="sxs-lookup"><span data-stu-id="0bf68-133">id</span></span>|<span data-ttu-id="0bf68-134">String</span><span class="sxs-lookup"><span data-stu-id="0bf68-134">String</span></span>|<span data-ttu-id="0bf68-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0bf68-135">Key of the entity.</span></span> <span data-ttu-id="0bf68-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bf68-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bf68-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0bf68-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bf68-138">DateTimeOffset</span></span>|<span data-ttu-id="0bf68-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0bf68-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0bf68-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bf68-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0bf68-141">roleScopeTagIds</span></span>|<span data-ttu-id="0bf68-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="0bf68-142">String collection</span></span>|<span data-ttu-id="0bf68-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0bf68-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0bf68-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bf68-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0bf68-145">supportsScopeTags</span></span>|<span data-ttu-id="0bf68-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bf68-146">Boolean</span></span>|<span data-ttu-id="0bf68-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0bf68-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0bf68-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0bf68-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0bf68-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0bf68-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0bf68-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0bf68-150">This property is read-only.</span></span> <span data-ttu-id="0bf68-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bf68-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0bf68-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0bf68-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0bf68-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0bf68-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="0bf68-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0bf68-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bf68-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0bf68-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0bf68-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0bf68-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0bf68-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="0bf68-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0bf68-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bf68-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0bf68-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0bf68-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0bf68-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0bf68-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="0bf68-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0bf68-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bf68-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0bf68-164">createdDateTime</span></span>|<span data-ttu-id="0bf68-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bf68-165">DateTimeOffset</span></span>|<span data-ttu-id="0bf68-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0bf68-166">DateTime the object was created.</span></span> <span data-ttu-id="0bf68-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bf68-168">description</span><span class="sxs-lookup"><span data-stu-id="0bf68-168">description</span></span>|<span data-ttu-id="0bf68-169">String</span><span class="sxs-lookup"><span data-stu-id="0bf68-169">String</span></span>|<span data-ttu-id="0bf68-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bf68-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0bf68-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bf68-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0bf68-172">displayName</span></span>|<span data-ttu-id="0bf68-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bf68-173">String</span></span>|<span data-ttu-id="0bf68-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bf68-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0bf68-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bf68-176">versão</span><span class="sxs-lookup"><span data-stu-id="0bf68-176">version</span></span>|<span data-ttu-id="0bf68-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0bf68-177">Int32</span></span>|<span data-ttu-id="0bf68-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bf68-178">Version of the device configuration.</span></span> <span data-ttu-id="0bf68-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bf68-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0bf68-180">authenticationMethod</span></span>|[<span data-ttu-id="0bf68-181">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0bf68-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="0bf68-182">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="0bf68-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="0bf68-183">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0bf68-183">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="0bf68-184">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="0bf68-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="0bf68-185">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="0bf68-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="0bf68-186">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="0bf68-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="0bf68-187">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="0bf68-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="0bf68-188">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0bf68-188">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="0bf68-189">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="0bf68-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="0bf68-190">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="0bf68-190">emailAddressSource</span></span>|[<span data-ttu-id="0bf68-191">UserEmail</span><span class="sxs-lookup"><span data-stu-id="0bf68-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0bf68-192">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bf68-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0bf68-193">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0bf68-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="0bf68-194">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0bf68-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0bf68-195">hostName</span><span class="sxs-lookup"><span data-stu-id="0bf68-195">hostName</span></span>|<span data-ttu-id="0bf68-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0bf68-196">String</span></span>|<span data-ttu-id="0bf68-197">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="0bf68-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="0bf68-198">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-198">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="0bf68-199">requireSsl</span><span class="sxs-lookup"><span data-stu-id="0bf68-199">requireSsl</span></span>|<span data-ttu-id="0bf68-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bf68-200">Boolean</span></span>|<span data-ttu-id="0bf68-201">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="0bf68-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="0bf68-202">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="0bf68-202">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="0bf68-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="0bf68-203">usernameSource</span></span>|[<span data-ttu-id="0bf68-204">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="0bf68-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="0bf68-205">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bf68-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0bf68-206">Herdado de [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="0bf68-206">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="0bf68-207">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0bf68-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0bf68-208">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="0bf68-208">syncCalendar</span></span>|<span data-ttu-id="0bf68-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bf68-209">Boolean</span></span>|<span data-ttu-id="0bf68-210">Alterna a sincronização do calendário.</span><span class="sxs-lookup"><span data-stu-id="0bf68-210">Toggles syncing the calendar.</span></span> <span data-ttu-id="0bf68-211">Se definido como falso, o calendário será desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bf68-211">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="0bf68-212">syncContacts</span><span class="sxs-lookup"><span data-stu-id="0bf68-212">syncContacts</span></span>|<span data-ttu-id="0bf68-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bf68-213">Boolean</span></span>|<span data-ttu-id="0bf68-214">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="0bf68-214">Toggles syncing contacts.</span></span> <span data-ttu-id="0bf68-215">Se definido como falso, os contatos serão desativados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bf68-215">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="0bf68-216">syncTasks</span><span class="sxs-lookup"><span data-stu-id="0bf68-216">syncTasks</span></span>|<span data-ttu-id="0bf68-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bf68-217">Boolean</span></span>|<span data-ttu-id="0bf68-218">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="0bf68-218">Toggles syncing tasks.</span></span> <span data-ttu-id="0bf68-219">Se definido como falso, as tarefas serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0bf68-219">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="0bf68-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bf68-220">Response</span></span>
<span data-ttu-id="0bf68-221">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bf68-221">If successful, this method returns a `201 Created` response code and a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bf68-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bf68-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bf68-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bf68-223">Request</span></span>
<span data-ttu-id="0bf68-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bf68-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="0bf68-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bf68-225">Response</span></span>
<span data-ttu-id="0bf68-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0bf68-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



