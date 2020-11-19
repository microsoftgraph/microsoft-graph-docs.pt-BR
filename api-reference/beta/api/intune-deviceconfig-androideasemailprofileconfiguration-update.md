---
title: Atualizar androidEasEmailProfileConfiguration
description: Atualiza as propriedades de um objeto androidEasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32870ae3112a9f11951ee05f8339c19621b3c0ca
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49239827"
---
# <a name="update-androideasemailprofileconfiguration"></a><span data-ttu-id="0b898-103">Atualizar androidEasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="0b898-103">Update androidEasEmailProfileConfiguration</span></span>

<span data-ttu-id="0b898-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b898-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b898-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b898-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b898-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b898-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b898-107">Atualiza as propriedades de um objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0b898-107">Update the properties of a [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b898-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b898-108">Prerequisites</span></span>
<span data-ttu-id="0b898-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b898-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b898-111">Permission type</span></span>|<span data-ttu-id="0b898-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b898-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b898-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b898-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b898-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b898-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b898-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b898-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b898-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b898-116">Not supported.</span></span>|
|<span data-ttu-id="0b898-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b898-117">Application</span></span>|<span data-ttu-id="0b898-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b898-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b898-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b898-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0b898-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b898-120">Request headers</span></span>
|<span data-ttu-id="0b898-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b898-121">Header</span></span>|<span data-ttu-id="0b898-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0b898-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b898-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b898-123">Authorization</span></span>|<span data-ttu-id="0b898-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b898-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b898-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b898-125">Accept</span></span>|<span data-ttu-id="0b898-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b898-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b898-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b898-127">Request body</span></span>
<span data-ttu-id="0b898-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="0b898-128">In the request body, supply a JSON representation for the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="0b898-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0b898-129">The following table shows the properties that are required when you create the [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="0b898-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b898-130">Property</span></span>|<span data-ttu-id="0b898-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b898-131">Type</span></span>|<span data-ttu-id="0b898-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b898-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b898-133">id</span><span class="sxs-lookup"><span data-stu-id="0b898-133">id</span></span>|<span data-ttu-id="0b898-134">String</span><span class="sxs-lookup"><span data-stu-id="0b898-134">String</span></span>|<span data-ttu-id="0b898-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0b898-135">Key of the entity.</span></span> <span data-ttu-id="0b898-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b898-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b898-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b898-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0b898-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b898-138">DateTimeOffset</span></span>|<span data-ttu-id="0b898-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0b898-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0b898-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b898-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b898-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0b898-141">roleScopeTagIds</span></span>|<span data-ttu-id="0b898-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b898-142">String collection</span></span>|<span data-ttu-id="0b898-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0b898-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0b898-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b898-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b898-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0b898-145">supportsScopeTags</span></span>|<span data-ttu-id="0b898-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b898-146">Boolean</span></span>|<span data-ttu-id="0b898-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="0b898-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0b898-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="0b898-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0b898-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="0b898-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0b898-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b898-150">This property is read-only.</span></span> <span data-ttu-id="0b898-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b898-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b898-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0b898-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0b898-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0b898-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0b898-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="0b898-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0b898-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b898-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b898-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0b898-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0b898-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0b898-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0b898-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="0b898-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0b898-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b898-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b898-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0b898-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0b898-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0b898-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0b898-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="0b898-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0b898-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b898-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b898-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b898-164">createdDateTime</span></span>|<span data-ttu-id="0b898-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b898-165">DateTimeOffset</span></span>|<span data-ttu-id="0b898-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0b898-166">DateTime the object was created.</span></span> <span data-ttu-id="0b898-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b898-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b898-168">description</span><span class="sxs-lookup"><span data-stu-id="0b898-168">description</span></span>|<span data-ttu-id="0b898-169">String</span><span class="sxs-lookup"><span data-stu-id="0b898-169">String</span></span>|<span data-ttu-id="0b898-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b898-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0b898-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b898-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b898-172">displayName</span><span class="sxs-lookup"><span data-stu-id="0b898-172">displayName</span></span>|<span data-ttu-id="0b898-173">String</span><span class="sxs-lookup"><span data-stu-id="0b898-173">String</span></span>|<span data-ttu-id="0b898-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b898-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0b898-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b898-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b898-176">versão</span><span class="sxs-lookup"><span data-stu-id="0b898-176">version</span></span>|<span data-ttu-id="0b898-177">Int32</span><span class="sxs-lookup"><span data-stu-id="0b898-177">Int32</span></span>|<span data-ttu-id="0b898-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b898-178">Version of the device configuration.</span></span> <span data-ttu-id="0b898-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0b898-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0b898-180">accountName</span><span class="sxs-lookup"><span data-stu-id="0b898-180">accountName</span></span>|<span data-ttu-id="0b898-181">String</span><span class="sxs-lookup"><span data-stu-id="0b898-181">String</span></span>|<span data-ttu-id="0b898-182">Nome da conta do Exchange ActiveSync, exibido para os usuários como o nome do perfil EAS (este).</span><span class="sxs-lookup"><span data-stu-id="0b898-182">Exchange ActiveSync account name, displayed to users as name of EAS (this) profile.</span></span>|
|<span data-ttu-id="0b898-183">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0b898-183">authenticationMethod</span></span>|[<span data-ttu-id="0b898-184">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0b898-184">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="0b898-185">Método de autenticação para o Exchange ActiveSync.</span><span class="sxs-lookup"><span data-stu-id="0b898-185">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="0b898-186">Os valores possíveis são: `usernameAndPassword`, `certificate`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="0b898-186">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="0b898-187">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="0b898-187">syncCalendar</span></span>|<span data-ttu-id="0b898-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b898-188">Boolean</span></span>|<span data-ttu-id="0b898-189">Alterna a sincronização do calendário.</span><span class="sxs-lookup"><span data-stu-id="0b898-189">Toggles syncing the calendar.</span></span> <span data-ttu-id="0b898-190">Se definido como falso, o calendário será desativado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b898-190">If set to false calendar is turned off on the device.</span></span>|
|<span data-ttu-id="0b898-191">syncContacts</span><span class="sxs-lookup"><span data-stu-id="0b898-191">syncContacts</span></span>|<span data-ttu-id="0b898-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b898-192">Boolean</span></span>|<span data-ttu-id="0b898-193">Alterna a sincronização de contatos.</span><span class="sxs-lookup"><span data-stu-id="0b898-193">Toggles syncing contacts.</span></span> <span data-ttu-id="0b898-194">Se definido como falso, os contatos serão desativados no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b898-194">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="0b898-195">syncTasks</span><span class="sxs-lookup"><span data-stu-id="0b898-195">syncTasks</span></span>|<span data-ttu-id="0b898-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b898-196">Boolean</span></span>|<span data-ttu-id="0b898-197">Alterna a sincronização de tarefas.</span><span class="sxs-lookup"><span data-stu-id="0b898-197">Toggles syncing tasks.</span></span> <span data-ttu-id="0b898-198">Se definido como falso, as tarefas serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b898-198">If set to false tasks are turned off on the device.</span></span>|
|<span data-ttu-id="0b898-199">syncNotes</span><span class="sxs-lookup"><span data-stu-id="0b898-199">syncNotes</span></span>|<span data-ttu-id="0b898-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b898-200">Boolean</span></span>|<span data-ttu-id="0b898-201">Alterna a sincronização das anotações.</span><span class="sxs-lookup"><span data-stu-id="0b898-201">Toggles syncing notes.</span></span> <span data-ttu-id="0b898-202">Se definido como false, as anotações serão desativadas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b898-202">If set to false notes are turned off on the device.</span></span>|
|<span data-ttu-id="0b898-203">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="0b898-203">durationOfEmailToSync</span></span>|[<span data-ttu-id="0b898-204">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="0b898-204">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="0b898-205">Duração de tempo que o email deve ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="0b898-205">Duration of time email should be synced to.</span></span> <span data-ttu-id="0b898-206">Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="0b898-206">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="0b898-207">emailAddresse</span><span class="sxs-lookup"><span data-stu-id="0b898-207">emailAddressSource</span></span>|[<span data-ttu-id="0b898-208">UserEmail</span><span class="sxs-lookup"><span data-stu-id="0b898-208">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="0b898-209">Atributo de email separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b898-209">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0b898-210">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0b898-210">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0b898-211">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="0b898-211">emailSyncSchedule</span></span>|[<span data-ttu-id="0b898-212">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="0b898-212">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="0b898-213">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="0b898-213">Email sync schedule.</span></span> <span data-ttu-id="0b898-214">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="0b898-214">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="0b898-215">hostName</span><span class="sxs-lookup"><span data-stu-id="0b898-215">hostName</span></span>|<span data-ttu-id="0b898-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b898-216">String</span></span>|<span data-ttu-id="0b898-217">Local do Exchange (URL) ao qual o aplicativo de email nativo se conecta.</span><span class="sxs-lookup"><span data-stu-id="0b898-217">Exchange location (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="0b898-218">requireSmime</span><span class="sxs-lookup"><span data-stu-id="0b898-218">requireSmime</span></span>|<span data-ttu-id="0b898-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b898-219">Boolean</span></span>|<span data-ttu-id="0b898-220">Indica se o certificado S/MIME deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="0b898-220">Indicates whether or not to use S/MIME certificate.</span></span>|
|<span data-ttu-id="0b898-221">requireSsl</span><span class="sxs-lookup"><span data-stu-id="0b898-221">requireSsl</span></span>|<span data-ttu-id="0b898-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="0b898-222">Boolean</span></span>|<span data-ttu-id="0b898-223">Indica se o SSL deve ou não ser usado.</span><span class="sxs-lookup"><span data-stu-id="0b898-223">Indicates whether or not to use SSL.</span></span>|
|<span data-ttu-id="0b898-224">usernameSource</span><span class="sxs-lookup"><span data-stu-id="0b898-224">usernameSource</span></span>|[<span data-ttu-id="0b898-225">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="0b898-225">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="0b898-226">Atributo username que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b898-226">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0b898-227">Os valores possíveis são: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="0b898-227">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="0b898-228">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="0b898-228">userDomainNameSource</span></span>|[<span data-ttu-id="0b898-229">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="0b898-229">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="0b898-230">Atributo UserDomainName que é separado do AAD e injetado nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b898-230">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="0b898-231">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="0b898-231">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="0b898-232">customDomainName</span><span class="sxs-lookup"><span data-stu-id="0b898-232">customDomainName</span></span>|<span data-ttu-id="0b898-233">String</span><span class="sxs-lookup"><span data-stu-id="0b898-233">String</span></span>|<span data-ttu-id="0b898-234">Valor de nome de domínio personalizado usado durante a geração de um perfil de email antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0b898-234">Custom domain name value used while generating an email profile before installing on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="0b898-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b898-235">Response</span></span>
<span data-ttu-id="0b898-236">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b898-236">If successful, this method returns a `200 OK` response code and an updated [androidEasEmailProfileConfiguration](../resources/intune-deviceconfig-androideasemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b898-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b898-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b898-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b898-238">Request</span></span>
<span data-ttu-id="0b898-239">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b898-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="0b898-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b898-240">Response</span></span>
<span data-ttu-id="0b898-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b898-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




