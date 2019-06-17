---
title: Criar androidEasEmailProfileConfiguration
description: Criar um novo objeto androidEasEmailProfileConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1c5b7c12e306f0ac718f86cb129e158cff50da1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971258"
---
# <a name="create-androideasemailprofileconfiguration"></a><span data-ttu-id="7ad3c-103">Criar androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ad3c-103">Create androidEasEmailProfileConfiguration</span></span>

> <span data-ttu-id="7ad3c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ad3c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ad3c-106">Criar um novo objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7ad3c-106">Create a new [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ad3c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ad3c-107">Prerequisites</span></span>
<span data-ttu-id="7ad3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ad3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ad3c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ad3c-110">Permission type</span></span>|<span data-ttu-id="7ad3c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ad3c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ad3c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ad3c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ad3c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ad3c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-115">Not supported.</span></span>|
|<span data-ttu-id="7ad3c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ad3c-116">Application</span></span>|<span data-ttu-id="7ad3c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ad3c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ad3c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7ad3c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ad3c-119">Request headers</span></span>
|<span data-ttu-id="7ad3c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ad3c-120">Header</span></span>|<span data-ttu-id="7ad3c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7ad3c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ad3c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ad3c-122">Authorization</span></span>|<span data-ttu-id="7ad3c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ad3c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ad3c-124">Accept</span></span>|<span data-ttu-id="7ad3c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ad3c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ad3c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ad3c-126">Request body</span></span>
<span data-ttu-id="7ad3c-127">No corpo da solicitação, forneça uma representação JSON do objeto androidEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-127">In the request body, supply a JSON representation for the androidEasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="7ad3c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidEasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-128">The following table shows the properties that are required when you create the androidEasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="7ad3c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ad3c-129">Property</span></span>|<span data-ttu-id="7ad3c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ad3c-130">Type</span></span>|<span data-ttu-id="7ad3c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ad3c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ad3c-132">id</span><span class="sxs-lookup"><span data-stu-id="7ad3c-132">id</span></span>|<span data-ttu-id="7ad3c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ad3c-133">String</span></span>|<span data-ttu-id="7ad3c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-134">Key of the entity.</span></span> <span data-ttu-id="7ad3c-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad3c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ad3c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7ad3c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ad3c-137">DateTimeOffset</span></span>|<span data-ttu-id="7ad3c-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7ad3c-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad3c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7ad3c-140">roleScopeTagIds</span></span>|<span data-ttu-id="7ad3c-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ad3c-141">String collection</span></span>|<span data-ttu-id="7ad3c-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7ad3c-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad3c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7ad3c-144">supportsScopeTags</span></span>|<span data-ttu-id="7ad3c-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ad3c-145">Boolean</span></span>|<span data-ttu-id="7ad3c-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7ad3c-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7ad3c-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7ad3c-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-149">This property is read-only.</span></span> <span data-ttu-id="7ad3c-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad3c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7ad3c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7ad3c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7ad3c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7ad3c-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7ad3c-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad3c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7ad3c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7ad3c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7ad3c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7ad3c-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7ad3c-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad3c-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7ad3c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7ad3c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7ad3c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7ad3c-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7ad3c-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad3c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ad3c-163">createdDateTime</span></span>|<span data-ttu-id="7ad3c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ad3c-164">DateTimeOffset</span></span>|<span data-ttu-id="7ad3c-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-165">DateTime the object was created.</span></span> <span data-ttu-id="7ad3c-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad3c-167">descrição</span><span class="sxs-lookup"><span data-stu-id="7ad3c-167">description</span></span>|<span data-ttu-id="7ad3c-168">String</span><span class="sxs-lookup"><span data-stu-id="7ad3c-168">String</span></span>|<span data-ttu-id="7ad3c-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7ad3c-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad3c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="7ad3c-171">displayName</span></span>|<span data-ttu-id="7ad3c-172">String</span><span class="sxs-lookup"><span data-stu-id="7ad3c-172">String</span></span>|<span data-ttu-id="7ad3c-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7ad3c-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad3c-175">versão</span><span class="sxs-lookup"><span data-stu-id="7ad3c-175">version</span></span>|<span data-ttu-id="7ad3c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7ad3c-176">Int32</span></span>|<span data-ttu-id="7ad3c-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-177">Version of the device configuration.</span></span> <span data-ttu-id="7ad3c-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7ad3c-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7ad3c-179">accountName</span><span class="sxs-lookup"><span data-stu-id="7ad3c-179">accountName</span></span>|<span data-ttu-id="7ad3c-180">String</span><span class="sxs-lookup"><span data-stu-id="7ad3c-180">String</span></span>|<span data-ttu-id="7ad3c-181">Nome da conta do Exchange ActiveSync, exibido para os usuários como o nome do perfil EAS (este).</span><span class="sxs-lookup"><span data-stu-id="7ad3c-181">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="7ad3c-182">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7ad3c-182">authenticationMethod</span></span>|[<span data-ttu-id="7ad3c-183">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7ad3c-183">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="7ad3c-184">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-184">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="7ad3c-185">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-185">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="7ad3c-186">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="7ad3c-186">syncCalendar</span></span>|<span data-ttu-id="7ad3c-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ad3c-187">Boolean</span></span>|<span data-ttu-id="7ad3c-188">Alterna a sincronização do calendário.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-188">Toggles syncing the calendar.</span></span> <span data-ttu-id="7ad3c-189">Se definido como falso, o calendário será desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-189">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="7ad3c-190">syncContacts</span><span class="sxs-lookup"><span data-stu-id="7ad3c-190">syncContacts</span></span>|<span data-ttu-id="7ad3c-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ad3c-191">Boolean</span></span>|<span data-ttu-id="7ad3c-192">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-192">Toggles syncing contacts.</span></span> <span data-ttu-id="7ad3c-193">Se definido como falso, os contatos serão desativados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-193">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="7ad3c-194">syncTasks</span><span class="sxs-lookup"><span data-stu-id="7ad3c-194">syncTasks</span></span>|<span data-ttu-id="7ad3c-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ad3c-195">Boolean</span></span>|<span data-ttu-id="7ad3c-196">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-196">Toggles syncing tasks.</span></span> <span data-ttu-id="7ad3c-197">Se definido como falso, as tarefas serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-197">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="7ad3c-198">syncNotes</span><span class="sxs-lookup"><span data-stu-id="7ad3c-198">syncNotes</span></span>|<span data-ttu-id="7ad3c-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ad3c-199">Boolean</span></span>|<span data-ttu-id="7ad3c-200">Alterna a sincronização das anotações.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-200">Toggles syncing notes.</span></span> <span data-ttu-id="7ad3c-201">Se definido como false, as anotações serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-201">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="7ad3c-202">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="7ad3c-202">durationOfEmailToSync</span></span>|[<span data-ttu-id="7ad3c-203">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="7ad3c-203">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="7ad3c-204">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-204">Duration of time email should be synced to.</span></span> <span data-ttu-id="7ad3c-205">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-205">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="7ad3c-206">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="7ad3c-206">emailAddressSource</span></span>|[<span data-ttu-id="7ad3c-207">UserEmail</span><span class="sxs-lookup"><span data-stu-id="7ad3c-207">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7ad3c-208">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-208">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7ad3c-209">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-209">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7ad3c-210">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="7ad3c-210">emailSyncSchedule</span></span>|[<span data-ttu-id="7ad3c-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="7ad3c-211">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="7ad3c-212">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-212">Email sync schedule.</span></span> <span data-ttu-id="7ad3c-213">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-213">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="7ad3c-214">hostName</span><span class="sxs-lookup"><span data-stu-id="7ad3c-214">hostName</span></span>|<span data-ttu-id="7ad3c-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ad3c-215">String</span></span>|<span data-ttu-id="7ad3c-216">Local do Exchange (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-216">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="7ad3c-217">requireSmime</span><span class="sxs-lookup"><span data-stu-id="7ad3c-217">requireSmime</span></span>|<span data-ttu-id="7ad3c-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ad3c-218">Boolean</span></span>|<span data-ttu-id="7ad3c-219">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-219">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="7ad3c-220">requireSsl</span><span class="sxs-lookup"><span data-stu-id="7ad3c-220">requireSsl</span></span>|<span data-ttu-id="7ad3c-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ad3c-221">Boolean</span></span>|<span data-ttu-id="7ad3c-222">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-222">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="7ad3c-223">usernameSource</span><span class="sxs-lookup"><span data-stu-id="7ad3c-223">usernameSource</span></span>|[<span data-ttu-id="7ad3c-224">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="7ad3c-224">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="7ad3c-225">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-225">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7ad3c-226">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-226">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7ad3c-227">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="7ad3c-227">userDomainNameSource</span></span>|[<span data-ttu-id="7ad3c-228">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="7ad3c-228">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="7ad3c-229">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-229">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7ad3c-230">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-230">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="7ad3c-231">customDomainName</span><span class="sxs-lookup"><span data-stu-id="7ad3c-231">customDomainName</span></span>|<span data-ttu-id="7ad3c-232">String</span><span class="sxs-lookup"><span data-stu-id="7ad3c-232">String</span></span>|<span data-ttu-id="7ad3c-233">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-233">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="7ad3c-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ad3c-234">Response</span></span>
<span data-ttu-id="7ad3c-235">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-235">If successful, this method returns a `201 Created` response code and a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ad3c-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ad3c-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ad3c-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ad3c-237">Request</span></span>
<span data-ttu-id="7ad3c-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1566

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
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
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```

### <a name="response"></a><span data-ttu-id="7ad3c-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ad3c-239">Response</span></span>
<span data-ttu-id="7ad3c-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ad3c-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1738

{
  "@odata.type": "#microsoft.graph.androidEasEmailProfileConfiguration",
  "id": "ee5e5610-5610-ee5e-1056-5eee10565eee",
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
  "accountName": "Account Name value",
  "authenticationMethod": "certificate",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "syncNotes": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSmime": true,
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value"
}
```





