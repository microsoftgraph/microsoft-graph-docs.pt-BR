---
title: Atualizar androidForWorkNineWorkEasConfiguration
description: Atualize as propriedades de um objeto androidForWorkNineWorkEasConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02f60954251ad79cc2db09753111773bb1c5b7b7
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138411"
---
# <a name="update-androidforworknineworkeasconfiguration"></a><span data-ttu-id="fce3e-103">Atualizar androidForWorkNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="fce3e-103">Update androidForWorkNineWorkEasConfiguration</span></span>

<span data-ttu-id="fce3e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fce3e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fce3e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fce3e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fce3e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fce3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fce3e-107">Atualize as propriedades de um [objeto androidForWorkNineWorkEasConfiguration.](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-107">Update the properties of a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fce3e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fce3e-108">Prerequisites</span></span>
<span data-ttu-id="fce3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fce3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fce3e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fce3e-111">Permission type</span></span>|<span data-ttu-id="fce3e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fce3e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fce3e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fce3e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fce3e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fce3e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fce3e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fce3e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fce3e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fce3e-116">Not supported.</span></span>|
|<span data-ttu-id="fce3e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fce3e-117">Application</span></span>|<span data-ttu-id="fce3e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fce3e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fce3e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fce3e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fce3e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fce3e-120">Request headers</span></span>
|<span data-ttu-id="fce3e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fce3e-121">Header</span></span>|<span data-ttu-id="fce3e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fce3e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fce3e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fce3e-123">Authorization</span></span>|<span data-ttu-id="fce3e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fce3e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fce3e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fce3e-125">Accept</span></span>|<span data-ttu-id="fce3e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fce3e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fce3e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fce3e-127">Request body</span></span>
<span data-ttu-id="fce3e-128">No corpo da solicitação, fornece uma representação JSON para o [objeto androidForWorkNineWorkEasConfiguration.](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-128">In the request body, supply a JSON representation for the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="fce3e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fce3e-129">The following table shows the properties that are required when you create the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="fce3e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fce3e-130">Property</span></span>|<span data-ttu-id="fce3e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fce3e-131">Type</span></span>|<span data-ttu-id="fce3e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fce3e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fce3e-133">id</span><span class="sxs-lookup"><span data-stu-id="fce3e-133">id</span></span>|<span data-ttu-id="fce3e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fce3e-134">String</span></span>|<span data-ttu-id="fce3e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fce3e-135">Key of the entity.</span></span> <span data-ttu-id="fce3e-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fce3e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fce3e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fce3e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fce3e-138">DateTimeOffset</span></span>|<span data-ttu-id="fce3e-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="fce3e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fce3e-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fce3e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fce3e-141">roleScopeTagIds</span></span>|<span data-ttu-id="fce3e-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fce3e-142">String collection</span></span>|<span data-ttu-id="fce3e-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="fce3e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fce3e-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fce3e-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fce3e-145">supportsScopeTags</span></span>|<span data-ttu-id="fce3e-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="fce3e-146">Boolean</span></span>|<span data-ttu-id="fce3e-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="fce3e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fce3e-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="fce3e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fce3e-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="fce3e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fce3e-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fce3e-150">This property is read-only.</span></span> <span data-ttu-id="fce3e-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fce3e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fce3e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fce3e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fce3e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fce3e-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="fce3e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fce3e-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fce3e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fce3e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fce3e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fce3e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fce3e-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="fce3e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fce3e-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fce3e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fce3e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fce3e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fce3e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fce3e-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="fce3e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fce3e-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fce3e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fce3e-164">createdDateTime</span></span>|<span data-ttu-id="fce3e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fce3e-165">DateTimeOffset</span></span>|<span data-ttu-id="fce3e-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fce3e-166">DateTime the object was created.</span></span> <span data-ttu-id="fce3e-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fce3e-168">descrição</span><span class="sxs-lookup"><span data-stu-id="fce3e-168">description</span></span>|<span data-ttu-id="fce3e-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fce3e-169">String</span></span>|<span data-ttu-id="fce3e-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fce3e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fce3e-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fce3e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fce3e-172">displayName</span></span>|<span data-ttu-id="fce3e-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fce3e-173">String</span></span>|<span data-ttu-id="fce3e-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fce3e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fce3e-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fce3e-176">versão</span><span class="sxs-lookup"><span data-stu-id="fce3e-176">version</span></span>|<span data-ttu-id="fce3e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fce3e-177">Int32</span></span>|<span data-ttu-id="fce3e-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fce3e-178">Version of the device configuration.</span></span> <span data-ttu-id="fce3e-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fce3e-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fce3e-180">authenticationMethod</span></span>|[<span data-ttu-id="fce3e-181">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fce3e-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="fce3e-182">Método de autenticação para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="fce3e-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="fce3e-183">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fce3e-183">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="fce3e-184">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="fce3e-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="fce3e-185">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="fce3e-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="fce3e-186">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="fce3e-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="fce3e-187">A duração do tempo em que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="fce3e-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="fce3e-188">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fce3e-188">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="fce3e-189">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="fce3e-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="fce3e-190">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="fce3e-190">emailAddressSource</span></span>|[<span data-ttu-id="fce3e-191">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="fce3e-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="fce3e-192">Atributo de email que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fce3e-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="fce3e-193">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fce3e-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="fce3e-194">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="fce3e-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="fce3e-195">hostName</span><span class="sxs-lookup"><span data-stu-id="fce3e-195">hostName</span></span>|<span data-ttu-id="fce3e-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fce3e-196">String</span></span>|<span data-ttu-id="fce3e-197">Local do Exchange (URL) ao que o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="fce3e-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="fce3e-198">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-198">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="fce3e-199">requireSsl</span><span class="sxs-lookup"><span data-stu-id="fce3e-199">requireSsl</span></span>|<span data-ttu-id="fce3e-200">Booleano</span><span class="sxs-lookup"><span data-stu-id="fce3e-200">Boolean</span></span>|<span data-ttu-id="fce3e-201">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="fce3e-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="fce3e-202">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="fce3e-202">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="fce3e-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="fce3e-203">usernameSource</span></span>|[<span data-ttu-id="fce3e-204">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="fce3e-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="fce3e-205">Atributo username que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fce3e-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="fce3e-206">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="fce3e-206">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="fce3e-207">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="fce3e-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="fce3e-208">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="fce3e-208">syncCalendar</span></span>|<span data-ttu-id="fce3e-209">Booleano</span><span class="sxs-lookup"><span data-stu-id="fce3e-209">Boolean</span></span>|<span data-ttu-id="fce3e-210">Alterna sincronizando o calendário.</span><span class="sxs-lookup"><span data-stu-id="fce3e-210">Toggles syncing the calendar.</span></span> <span data-ttu-id="fce3e-211">Se definido como false, o calendário será desligado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fce3e-211">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="fce3e-212">syncContacts</span><span class="sxs-lookup"><span data-stu-id="fce3e-212">syncContacts</span></span>|<span data-ttu-id="fce3e-213">Booleano</span><span class="sxs-lookup"><span data-stu-id="fce3e-213">Boolean</span></span>|<span data-ttu-id="fce3e-214">Alterna contatos de sincronização.</span><span class="sxs-lookup"><span data-stu-id="fce3e-214">Toggles syncing contacts.</span></span> <span data-ttu-id="fce3e-215">Se definido como falsos contatos estão desligados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fce3e-215">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="fce3e-216">syncTasks</span><span class="sxs-lookup"><span data-stu-id="fce3e-216">syncTasks</span></span>|<span data-ttu-id="fce3e-217">Booleano</span><span class="sxs-lookup"><span data-stu-id="fce3e-217">Boolean</span></span>|<span data-ttu-id="fce3e-218">Alterna tarefas de sincronização.</span><span class="sxs-lookup"><span data-stu-id="fce3e-218">Toggles syncing tasks.</span></span> <span data-ttu-id="fce3e-219">Se as tarefas definidas como false são desligadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fce3e-219">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="fce3e-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="fce3e-220">Response</span></span>
<span data-ttu-id="fce3e-221">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fce3e-221">If successful, this method returns a `200 OK` response code and an updated [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fce3e-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fce3e-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="fce3e-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fce3e-223">Request</span></span>
<span data-ttu-id="fce3e-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fce3e-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fce3e-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="fce3e-225">Response</span></span>
<span data-ttu-id="fce3e-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fce3e-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




