---
title: Criar androidForWorkNineWorkEasConfiguration
description: Crie um novo objeto androidForWorkNineWorkEasConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 864a0d9fc3c85a83a2e01b5b990a2d043833bbe9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126581"
---
# <a name="create-androidforworknineworkeasconfiguration"></a><span data-ttu-id="7feaf-103">Criar androidForWorkNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="7feaf-103">Create androidForWorkNineWorkEasConfiguration</span></span>

<span data-ttu-id="7feaf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7feaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7feaf-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7feaf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7feaf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7feaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7feaf-107">Crie um novo [objeto androidForWorkNineWorkEasConfiguration.](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-107">Create a new [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7feaf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7feaf-108">Prerequisites</span></span>
<span data-ttu-id="7feaf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7feaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7feaf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7feaf-111">Permission type</span></span>|<span data-ttu-id="7feaf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7feaf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7feaf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7feaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7feaf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7feaf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7feaf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7feaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7feaf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7feaf-116">Not supported.</span></span>|
|<span data-ttu-id="7feaf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7feaf-117">Application</span></span>|<span data-ttu-id="7feaf-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7feaf-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7feaf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7feaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7feaf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7feaf-120">Request headers</span></span>
|<span data-ttu-id="7feaf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7feaf-121">Header</span></span>|<span data-ttu-id="7feaf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7feaf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7feaf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7feaf-123">Authorization</span></span>|<span data-ttu-id="7feaf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7feaf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7feaf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7feaf-125">Accept</span></span>|<span data-ttu-id="7feaf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7feaf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7feaf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7feaf-127">Request body</span></span>
<span data-ttu-id="7feaf-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7feaf-128">In the request body, supply a JSON representation for the androidForWorkNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="7feaf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o androidForWorkNineWorkEasConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7feaf-129">The following table shows the properties that are required when you create the androidForWorkNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="7feaf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7feaf-130">Property</span></span>|<span data-ttu-id="7feaf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7feaf-131">Type</span></span>|<span data-ttu-id="7feaf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7feaf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7feaf-133">id</span><span class="sxs-lookup"><span data-stu-id="7feaf-133">id</span></span>|<span data-ttu-id="7feaf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7feaf-134">String</span></span>|<span data-ttu-id="7feaf-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7feaf-135">Key of the entity.</span></span> <span data-ttu-id="7feaf-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7feaf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7feaf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7feaf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7feaf-138">DateTimeOffset</span></span>|<span data-ttu-id="7feaf-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7feaf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7feaf-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7feaf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7feaf-141">roleScopeTagIds</span></span>|<span data-ttu-id="7feaf-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7feaf-142">String collection</span></span>|<span data-ttu-id="7feaf-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="7feaf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7feaf-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7feaf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7feaf-145">supportsScopeTags</span></span>|<span data-ttu-id="7feaf-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="7feaf-146">Boolean</span></span>|<span data-ttu-id="7feaf-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7feaf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7feaf-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7feaf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7feaf-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7feaf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7feaf-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7feaf-150">This property is read-only.</span></span> <span data-ttu-id="7feaf-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7feaf-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7feaf-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7feaf-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7feaf-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7feaf-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="7feaf-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7feaf-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7feaf-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7feaf-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7feaf-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7feaf-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7feaf-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="7feaf-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7feaf-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7feaf-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7feaf-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7feaf-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7feaf-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7feaf-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="7feaf-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7feaf-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7feaf-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7feaf-164">createdDateTime</span></span>|<span data-ttu-id="7feaf-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7feaf-165">DateTimeOffset</span></span>|<span data-ttu-id="7feaf-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7feaf-166">DateTime the object was created.</span></span> <span data-ttu-id="7feaf-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7feaf-168">descrição</span><span class="sxs-lookup"><span data-stu-id="7feaf-168">description</span></span>|<span data-ttu-id="7feaf-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7feaf-169">String</span></span>|<span data-ttu-id="7feaf-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7feaf-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7feaf-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7feaf-172">displayName</span><span class="sxs-lookup"><span data-stu-id="7feaf-172">displayName</span></span>|<span data-ttu-id="7feaf-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7feaf-173">String</span></span>|<span data-ttu-id="7feaf-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7feaf-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7feaf-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7feaf-176">versão</span><span class="sxs-lookup"><span data-stu-id="7feaf-176">version</span></span>|<span data-ttu-id="7feaf-177">Int32</span><span class="sxs-lookup"><span data-stu-id="7feaf-177">Int32</span></span>|<span data-ttu-id="7feaf-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7feaf-178">Version of the device configuration.</span></span> <span data-ttu-id="7feaf-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7feaf-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7feaf-180">authenticationMethod</span></span>|[<span data-ttu-id="7feaf-181">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7feaf-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="7feaf-182">Método de autenticação para Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="7feaf-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="7feaf-183">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7feaf-183">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="7feaf-184">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="7feaf-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="7feaf-185">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="7feaf-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="7feaf-186">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="7feaf-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="7feaf-187">A duração do tempo em que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="7feaf-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="7feaf-188">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7feaf-188">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="7feaf-189">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="7feaf-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="7feaf-190">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="7feaf-190">emailAddressSource</span></span>|[<span data-ttu-id="7feaf-191">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="7feaf-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7feaf-192">Atributo de email que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7feaf-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7feaf-193">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7feaf-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="7feaf-194">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7feaf-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7feaf-195">hostName</span><span class="sxs-lookup"><span data-stu-id="7feaf-195">hostName</span></span>|<span data-ttu-id="7feaf-196">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7feaf-196">String</span></span>|<span data-ttu-id="7feaf-197">Local do Exchange (URL) ao que o aplicativo de email se conecta.</span><span class="sxs-lookup"><span data-stu-id="7feaf-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="7feaf-198">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-198">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="7feaf-199">requireSsl</span><span class="sxs-lookup"><span data-stu-id="7feaf-199">requireSsl</span></span>|<span data-ttu-id="7feaf-200">Booleano</span><span class="sxs-lookup"><span data-stu-id="7feaf-200">Boolean</span></span>|<span data-ttu-id="7feaf-201">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="7feaf-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="7feaf-202">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="7feaf-202">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="7feaf-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="7feaf-203">usernameSource</span></span>|[<span data-ttu-id="7feaf-204">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="7feaf-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="7feaf-205">Atributo username que é escolhido no AAD e injetado nesse perfil antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7feaf-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7feaf-206">Herdado [do androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span><span class="sxs-lookup"><span data-stu-id="7feaf-206">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="7feaf-207">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7feaf-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7feaf-208">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="7feaf-208">syncCalendar</span></span>|<span data-ttu-id="7feaf-209">Booleano</span><span class="sxs-lookup"><span data-stu-id="7feaf-209">Boolean</span></span>|<span data-ttu-id="7feaf-210">Alterna sincronizando o calendário.</span><span class="sxs-lookup"><span data-stu-id="7feaf-210">Toggles syncing the calendar.</span></span> <span data-ttu-id="7feaf-211">Se definido como false, o calendário será desligado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7feaf-211">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="7feaf-212">syncContacts</span><span class="sxs-lookup"><span data-stu-id="7feaf-212">syncContacts</span></span>|<span data-ttu-id="7feaf-213">Booleano</span><span class="sxs-lookup"><span data-stu-id="7feaf-213">Boolean</span></span>|<span data-ttu-id="7feaf-214">Alterna contatos de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7feaf-214">Toggles syncing contacts.</span></span> <span data-ttu-id="7feaf-215">Se definido como falsos contatos estão desligados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7feaf-215">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="7feaf-216">syncTasks</span><span class="sxs-lookup"><span data-stu-id="7feaf-216">syncTasks</span></span>|<span data-ttu-id="7feaf-217">Booleano</span><span class="sxs-lookup"><span data-stu-id="7feaf-217">Boolean</span></span>|<span data-ttu-id="7feaf-218">Alterna tarefas de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7feaf-218">Toggles syncing tasks.</span></span> <span data-ttu-id="7feaf-219">Se as tarefas definidas como false são desligadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7feaf-219">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="7feaf-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="7feaf-220">Response</span></span>
<span data-ttu-id="7feaf-221">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7feaf-221">If successful, this method returns a `201 Created` response code and a [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7feaf-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7feaf-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="7feaf-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7feaf-223">Request</span></span>
<span data-ttu-id="7feaf-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7feaf-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7feaf-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="7feaf-225">Response</span></span>
<span data-ttu-id="7feaf-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7feaf-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




