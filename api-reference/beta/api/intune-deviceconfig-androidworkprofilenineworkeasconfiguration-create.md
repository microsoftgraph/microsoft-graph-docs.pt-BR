---
title: Criar androidWorkProfileNineWorkEasConfiguration
description: Criar um novo objeto androidWorkProfileNineWorkEasConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0d5efa26ed6c1860303220e00f758824dd042f84
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35950683"
---
# <a name="create-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="03e62-103">Criar androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="03e62-103">Create androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="03e62-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03e62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03e62-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03e62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03e62-106">Criar um novo objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="03e62-106">Create a new [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03e62-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03e62-107">Prerequisites</span></span>
<span data-ttu-id="03e62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03e62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03e62-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03e62-110">Permission type</span></span>|<span data-ttu-id="03e62-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03e62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03e62-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03e62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03e62-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03e62-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03e62-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03e62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03e62-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03e62-115">Not supported.</span></span>|
|<span data-ttu-id="03e62-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03e62-116">Application</span></span>|<span data-ttu-id="03e62-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03e62-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03e62-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03e62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="03e62-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03e62-119">Request headers</span></span>
|<span data-ttu-id="03e62-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03e62-120">Header</span></span>|<span data-ttu-id="03e62-121">Valor</span><span class="sxs-lookup"><span data-stu-id="03e62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03e62-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="03e62-122">Authorization</span></span>|<span data-ttu-id="03e62-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03e62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03e62-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03e62-124">Accept</span></span>|<span data-ttu-id="03e62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="03e62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03e62-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03e62-126">Request body</span></span>
<span data-ttu-id="03e62-127">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="03e62-127">In the request body, supply a JSON representation for the androidWorkProfileNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="03e62-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="03e62-128">The following table shows the properties that are required when you create the androidWorkProfileNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="03e62-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03e62-129">Property</span></span>|<span data-ttu-id="03e62-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="03e62-130">Type</span></span>|<span data-ttu-id="03e62-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="03e62-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03e62-132">id</span><span class="sxs-lookup"><span data-stu-id="03e62-132">id</span></span>|<span data-ttu-id="03e62-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03e62-133">String</span></span>|<span data-ttu-id="03e62-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="03e62-134">Key of the entity.</span></span> <span data-ttu-id="03e62-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e62-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03e62-136">lastModifiedDateTime</span></span>|<span data-ttu-id="03e62-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e62-137">DateTimeOffset</span></span>|<span data-ttu-id="03e62-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="03e62-138">DateTime the object was last modified.</span></span> <span data-ttu-id="03e62-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e62-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="03e62-140">roleScopeTagIds</span></span>|<span data-ttu-id="03e62-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="03e62-141">String collection</span></span>|<span data-ttu-id="03e62-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="03e62-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="03e62-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e62-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="03e62-144">supportsScopeTags</span></span>|<span data-ttu-id="03e62-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="03e62-145">Boolean</span></span>|<span data-ttu-id="03e62-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="03e62-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="03e62-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="03e62-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="03e62-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="03e62-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="03e62-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="03e62-149">This property is read-only.</span></span> <span data-ttu-id="03e62-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e62-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="03e62-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="03e62-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="03e62-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="03e62-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="03e62-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="03e62-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e62-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="03e62-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="03e62-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="03e62-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="03e62-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="03e62-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="03e62-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e62-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="03e62-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="03e62-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="03e62-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="03e62-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="03e62-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="03e62-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e62-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03e62-163">createdDateTime</span></span>|<span data-ttu-id="03e62-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03e62-164">DateTimeOffset</span></span>|<span data-ttu-id="03e62-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="03e62-165">DateTime the object was created.</span></span> <span data-ttu-id="03e62-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e62-167">descrição</span><span class="sxs-lookup"><span data-stu-id="03e62-167">description</span></span>|<span data-ttu-id="03e62-168">String</span><span class="sxs-lookup"><span data-stu-id="03e62-168">String</span></span>|<span data-ttu-id="03e62-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e62-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="03e62-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e62-171">displayName</span><span class="sxs-lookup"><span data-stu-id="03e62-171">displayName</span></span>|<span data-ttu-id="03e62-172">String</span><span class="sxs-lookup"><span data-stu-id="03e62-172">String</span></span>|<span data-ttu-id="03e62-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e62-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="03e62-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e62-175">versão</span><span class="sxs-lookup"><span data-stu-id="03e62-175">version</span></span>|<span data-ttu-id="03e62-176">Int32</span><span class="sxs-lookup"><span data-stu-id="03e62-176">Int32</span></span>|<span data-ttu-id="03e62-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e62-177">Version of the device configuration.</span></span> <span data-ttu-id="03e62-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03e62-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="03e62-179">authenticationMethod</span></span>|[<span data-ttu-id="03e62-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="03e62-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="03e62-181">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="03e62-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="03e62-182">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03e62-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="03e62-183">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="03e62-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="03e62-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="03e62-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="03e62-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="03e62-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="03e62-186">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="03e62-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="03e62-187">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03e62-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="03e62-188">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="03e62-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="03e62-189">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="03e62-189">emailAddressSource</span></span>|[<span data-ttu-id="03e62-190">UserEmail</span><span class="sxs-lookup"><span data-stu-id="03e62-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="03e62-191">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e62-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="03e62-192">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03e62-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="03e62-193">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="03e62-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="03e62-194">hostName</span><span class="sxs-lookup"><span data-stu-id="03e62-194">hostName</span></span>|<span data-ttu-id="03e62-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03e62-195">String</span></span>|<span data-ttu-id="03e62-196">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="03e62-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="03e62-197">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="03e62-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="03e62-198">requireSsl</span></span>|<span data-ttu-id="03e62-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="03e62-199">Boolean</span></span>|<span data-ttu-id="03e62-200">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="03e62-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="03e62-201">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="03e62-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="03e62-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="03e62-202">usernameSource</span></span>|[<span data-ttu-id="03e62-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="03e62-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="03e62-204">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e62-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="03e62-205">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="03e62-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="03e62-206">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="03e62-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="03e62-207">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="03e62-207">syncCalendar</span></span>|<span data-ttu-id="03e62-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="03e62-208">Boolean</span></span>|<span data-ttu-id="03e62-209">Alterna a sincronização do calendário.</span><span class="sxs-lookup"><span data-stu-id="03e62-209">Toggles syncing the calendar.</span></span> <span data-ttu-id="03e62-210">Se definido como falso, o calendário será desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e62-210">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="03e62-211">syncContacts</span><span class="sxs-lookup"><span data-stu-id="03e62-211">syncContacts</span></span>|<span data-ttu-id="03e62-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="03e62-212">Boolean</span></span>|<span data-ttu-id="03e62-213">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="03e62-213">Toggles syncing contacts.</span></span> <span data-ttu-id="03e62-214">Se definido como falso, os contatos serão desativados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e62-214">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="03e62-215">syncTasks</span><span class="sxs-lookup"><span data-stu-id="03e62-215">syncTasks</span></span>|<span data-ttu-id="03e62-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="03e62-216">Boolean</span></span>|<span data-ttu-id="03e62-217">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="03e62-217">Toggles syncing tasks.</span></span> <span data-ttu-id="03e62-218">Se definido como falso, as tarefas serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="03e62-218">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="03e62-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="03e62-219">Response</span></span>
<span data-ttu-id="03e62-220">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03e62-220">If successful, this method returns a `201 Created` response code and a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03e62-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03e62-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="03e62-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03e62-222">Request</span></span>
<span data-ttu-id="03e62-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03e62-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="03e62-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="03e62-224">Response</span></span>
<span data-ttu-id="03e62-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03e62-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





