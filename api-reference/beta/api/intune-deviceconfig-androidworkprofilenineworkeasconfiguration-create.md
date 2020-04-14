---
title: Criar androidWorkProfileNineWorkEasConfiguration
description: Criar um novo objeto androidWorkProfileNineWorkEasConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 947d9a250a1c17dec790a9d498ef87b71d04a4f2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43434918"
---
# <a name="create-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="a740b-103">Criar androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="a740b-103">Create androidWorkProfileNineWorkEasConfiguration</span></span>

<span data-ttu-id="a740b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a740b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a740b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a740b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a740b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a740b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a740b-107">Criar um novo objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a740b-107">Create a new [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a740b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a740b-108">Prerequisites</span></span>
<span data-ttu-id="a740b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a740b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a740b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a740b-111">Permission type</span></span>|<span data-ttu-id="a740b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a740b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a740b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a740b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a740b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a740b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a740b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a740b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a740b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a740b-116">Not supported.</span></span>|
|<span data-ttu-id="a740b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a740b-117">Application</span></span>|<span data-ttu-id="a740b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a740b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a740b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a740b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a740b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a740b-120">Request headers</span></span>
|<span data-ttu-id="a740b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a740b-121">Header</span></span>|<span data-ttu-id="a740b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a740b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a740b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a740b-123">Authorization</span></span>|<span data-ttu-id="a740b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a740b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a740b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a740b-125">Accept</span></span>|<span data-ttu-id="a740b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a740b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a740b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a740b-127">Request body</span></span>
<span data-ttu-id="a740b-128">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a740b-128">In the request body, supply a JSON representation for the androidWorkProfileNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="a740b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a740b-129">The following table shows the properties that are required when you create the androidWorkProfileNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="a740b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a740b-130">Property</span></span>|<span data-ttu-id="a740b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a740b-131">Type</span></span>|<span data-ttu-id="a740b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a740b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a740b-133">id</span><span class="sxs-lookup"><span data-stu-id="a740b-133">id</span></span>|<span data-ttu-id="a740b-134">String</span><span class="sxs-lookup"><span data-stu-id="a740b-134">String</span></span>|<span data-ttu-id="a740b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a740b-135">Key of the entity.</span></span> <span data-ttu-id="a740b-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a740b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a740b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a740b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a740b-138">DateTimeOffset</span></span>|<span data-ttu-id="a740b-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a740b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a740b-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a740b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a740b-141">roleScopeTagIds</span></span>|<span data-ttu-id="a740b-142">Coleção String</span><span class="sxs-lookup"><span data-stu-id="a740b-142">String collection</span></span>|<span data-ttu-id="a740b-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a740b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a740b-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a740b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a740b-145">supportsScopeTags</span></span>|<span data-ttu-id="a740b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a740b-146">Boolean</span></span>|<span data-ttu-id="a740b-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a740b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a740b-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a740b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a740b-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a740b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a740b-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a740b-150">This property is read-only.</span></span> <span data-ttu-id="a740b-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a740b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a740b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a740b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a740b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a740b-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="a740b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a740b-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a740b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a740b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a740b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a740b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a740b-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="a740b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a740b-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a740b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a740b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a740b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a740b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a740b-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="a740b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a740b-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a740b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a740b-164">createdDateTime</span></span>|<span data-ttu-id="a740b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a740b-165">DateTimeOffset</span></span>|<span data-ttu-id="a740b-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a740b-166">DateTime the object was created.</span></span> <span data-ttu-id="a740b-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a740b-168">description</span><span class="sxs-lookup"><span data-stu-id="a740b-168">description</span></span>|<span data-ttu-id="a740b-169">String</span><span class="sxs-lookup"><span data-stu-id="a740b-169">String</span></span>|<span data-ttu-id="a740b-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a740b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a740b-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a740b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a740b-172">displayName</span></span>|<span data-ttu-id="a740b-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a740b-173">String</span></span>|<span data-ttu-id="a740b-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a740b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a740b-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a740b-176">versão</span><span class="sxs-lookup"><span data-stu-id="a740b-176">version</span></span>|<span data-ttu-id="a740b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a740b-177">Int32</span></span>|<span data-ttu-id="a740b-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a740b-178">Version of the device configuration.</span></span> <span data-ttu-id="a740b-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a740b-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a740b-180">authenticationMethod</span></span>|[<span data-ttu-id="a740b-181">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a740b-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="a740b-182">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="a740b-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="a740b-183">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a740b-183">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="a740b-184">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="a740b-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="a740b-185">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="a740b-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="a740b-186">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="a740b-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="a740b-187">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="a740b-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="a740b-188">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a740b-188">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="a740b-189">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="a740b-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="a740b-190">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="a740b-190">emailAddressSource</span></span>|[<span data-ttu-id="a740b-191">UserEmail</span><span class="sxs-lookup"><span data-stu-id="a740b-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="a740b-192">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a740b-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a740b-193">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a740b-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="a740b-194">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a740b-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a740b-195">hostName</span><span class="sxs-lookup"><span data-stu-id="a740b-195">hostName</span></span>|<span data-ttu-id="a740b-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a740b-196">String</span></span>|<span data-ttu-id="a740b-197">Local do Exchange (URL) ao qual o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="a740b-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="a740b-198">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-198">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="a740b-199">requireSsl</span><span class="sxs-lookup"><span data-stu-id="a740b-199">requireSsl</span></span>|<span data-ttu-id="a740b-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a740b-200">Boolean</span></span>|<span data-ttu-id="a740b-201">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="a740b-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="a740b-202">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="a740b-202">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="a740b-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="a740b-203">usernameSource</span></span>|[<span data-ttu-id="a740b-204">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="a740b-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="a740b-205">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a740b-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="a740b-206">Herdado de [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="a740b-206">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="a740b-207">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="a740b-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="a740b-208">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="a740b-208">syncCalendar</span></span>|<span data-ttu-id="a740b-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="a740b-209">Boolean</span></span>|<span data-ttu-id="a740b-210">Alterna a sincronização do calendário.</span><span class="sxs-lookup"><span data-stu-id="a740b-210">Toggles syncing the calendar.</span></span> <span data-ttu-id="a740b-211">Se definido como falso, o calendário será desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a740b-211">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="a740b-212">syncContacts</span><span class="sxs-lookup"><span data-stu-id="a740b-212">syncContacts</span></span>|<span data-ttu-id="a740b-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="a740b-213">Boolean</span></span>|<span data-ttu-id="a740b-214">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="a740b-214">Toggles syncing contacts.</span></span> <span data-ttu-id="a740b-215">Se definido como falso, os contatos serão desativados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a740b-215">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="a740b-216">syncTasks</span><span class="sxs-lookup"><span data-stu-id="a740b-216">syncTasks</span></span>|<span data-ttu-id="a740b-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="a740b-217">Boolean</span></span>|<span data-ttu-id="a740b-218">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="a740b-218">Toggles syncing tasks.</span></span> <span data-ttu-id="a740b-219">Se definido como falso, as tarefas serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a740b-219">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="a740b-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="a740b-220">Response</span></span>
<span data-ttu-id="a740b-221">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a740b-221">If successful, this method returns a `201 Created` response code and a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a740b-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a740b-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="a740b-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a740b-223">Request</span></span>
<span data-ttu-id="a740b-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a740b-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a740b-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="a740b-225">Response</span></span>
<span data-ttu-id="a740b-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a740b-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



