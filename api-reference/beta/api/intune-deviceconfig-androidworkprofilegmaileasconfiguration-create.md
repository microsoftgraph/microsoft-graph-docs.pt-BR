---
title: Criar androidWorkProfileGmailEasConfiguration
description: Criar um novo objeto androidWorkProfileGmailEasConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cbc76964358af4b5530f5cdc2b7e8aac30113a9c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42758450"
---
# <a name="create-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="a0b8e-103">Criar androidWorkProfileGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="a0b8e-103">Create androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="a0b8e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0b8e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0b8e-106">Criar um novo objeto [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a0b8e-106">Create a new [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0b8e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0b8e-107">Prerequisites</span></span>
<span data-ttu-id="a0b8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0b8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0b8e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0b8e-110">Permission type</span></span>|<span data-ttu-id="a0b8e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0b8e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0b8e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0b8e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0b8e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0b8e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-115">Not supported.</span></span>|
|<span data-ttu-id="a0b8e-116">Application</span><span class="sxs-lookup"><span data-stu-id="a0b8e-116">Application</span></span>|<span data-ttu-id="a0b8e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0b8e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0b8e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0b8e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0b8e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0b8e-119">Request headers</span></span>
|<span data-ttu-id="a0b8e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0b8e-120">Header</span></span>|<span data-ttu-id="a0b8e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a0b8e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0b8e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0b8e-122">Authorization</span></span>|<span data-ttu-id="a0b8e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0b8e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0b8e-124">Accept</span></span>|<span data-ttu-id="a0b8e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0b8e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0b8e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0b8e-126">Request body</span></span>
<span data-ttu-id="a0b8e-127">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-127">In the request body, supply a JSON representation for the androidWorkProfileGmailEasConfiguration object.</span></span>

<span data-ttu-id="a0b8e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileGmailEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-128">The following table shows the properties that are required when you create the androidWorkProfileGmailEasConfiguration.</span></span>

|<span data-ttu-id="a0b8e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0b8e-129">Property</span></span>|<span data-ttu-id="a0b8e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0b8e-130">Type</span></span>|<span data-ttu-id="a0b8e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0b8e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0b8e-132">id</span><span class="sxs-lookup"><span data-stu-id="a0b8e-132">id</span></span>|<span data-ttu-id="a0b8e-133">String</span><span class="sxs-lookup"><span data-stu-id="a0b8e-133">String</span></span>|<span data-ttu-id="a0b8e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-134">Key of the entity.</span></span> <span data-ttu-id="a0b8e-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b8e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0b8e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a0b8e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0b8e-137">DateTimeOffset</span></span>|<span data-ttu-id="a0b8e-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a0b8e-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b8e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0b8e-140">roleScopeTagIds</span></span>|<span data-ttu-id="a0b8e-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0b8e-141">String collection</span></span>|<span data-ttu-id="a0b8e-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a0b8e-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b8e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a0b8e-144">supportsScopeTags</span></span>|<span data-ttu-id="a0b8e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0b8e-145">Boolean</span></span>|<span data-ttu-id="a0b8e-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a0b8e-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a0b8e-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a0b8e-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-149">This property is read-only.</span></span> <span data-ttu-id="a0b8e-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b8e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a0b8e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a0b8e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a0b8e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a0b8e-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a0b8e-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b8e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a0b8e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a0b8e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a0b8e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a0b8e-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a0b8e-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b8e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a0b8e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a0b8e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a0b8e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a0b8e-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a0b8e-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b8e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0b8e-163">createdDateTime</span></span>|<span data-ttu-id="a0b8e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0b8e-164">DateTimeOffset</span></span>|<span data-ttu-id="a0b8e-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-165">DateTime the object was created.</span></span> <span data-ttu-id="a0b8e-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b8e-167">description</span><span class="sxs-lookup"><span data-stu-id="a0b8e-167">description</span></span>|<span data-ttu-id="a0b8e-168">String</span><span class="sxs-lookup"><span data-stu-id="a0b8e-168">String</span></span>|<span data-ttu-id="a0b8e-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a0b8e-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b8e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a0b8e-171">displayName</span></span>|<span data-ttu-id="a0b8e-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0b8e-172">String</span></span>|<span data-ttu-id="a0b8e-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a0b8e-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b8e-175">versão</span><span class="sxs-lookup"><span data-stu-id="a0b8e-175">version</span></span>|<span data-ttu-id="a0b8e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b8e-176">Int32</span></span>|<span data-ttu-id="a0b8e-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-177">Version of the device configuration.</span></span> <span data-ttu-id="a0b8e-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b8e-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a0b8e-179">authenticationMethod</span></span>|[<span data-ttu-id="a0b8e-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a0b8e-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="a0b8e-181">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="a0b8e-182">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0b8e-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="a0b8e-183">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a0b8e-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="a0b8e-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="a0b8e-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="a0b8e-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="a0b8e-186">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="a0b8e-187">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0b8e-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="a0b8e-188">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="a0b8e-189">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="a0b8e-189">emailAddressSource</span></span>|[<span data-ttu-id="a0b8e-190">UserEmail</span><span class="sxs-lookup"><span data-stu-id="a0b8e-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a0b8e-191">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a0b8e-192">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0b8e-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="a0b8e-193">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a0b8e-194">hostName</span><span class="sxs-lookup"><span data-stu-id="a0b8e-194">hostName</span></span>|<span data-ttu-id="a0b8e-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0b8e-195">String</span></span>|<span data-ttu-id="a0b8e-196">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="a0b8e-197">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="a0b8e-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="a0b8e-198">requireSsl</span></span>|<span data-ttu-id="a0b8e-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0b8e-199">Boolean</span></span>|<span data-ttu-id="a0b8e-200">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="a0b8e-201">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a0b8e-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="a0b8e-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a0b8e-202">usernameSource</span></span>|[<span data-ttu-id="a0b8e-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="a0b8e-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="a0b8e-204">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a0b8e-205">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a0b8e-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="a0b8e-206">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="a0b8e-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0b8e-207">Response</span></span>
<span data-ttu-id="a0b8e-208">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-208">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0b8e-209">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0b8e-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0b8e-210">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0b8e-210">Request</span></span>
<span data-ttu-id="a0b8e-211">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-211">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0b8e-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0b8e-212">Response</span></span>
<span data-ttu-id="a0b8e-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0b8e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




