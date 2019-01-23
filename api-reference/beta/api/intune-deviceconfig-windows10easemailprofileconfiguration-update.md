---
title: Atualizar windows10EasEmailProfileConfiguration
description: Atualize as propriedades de um objeto windows10EasEmailProfileConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7cbb293477c2cdc3e1b022445daf381202f48d4c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398209"
---
# <a name="update-windows10easemailprofileconfiguration"></a><span data-ttu-id="7c83f-103">Atualizar windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c83f-103">Update windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="7c83f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7c83f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7c83f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7c83f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c83f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7c83f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c83f-107">Atualize as propriedades de um objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7c83f-107">Update the properties of a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c83f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c83f-108">Prerequisites</span></span>
<span data-ttu-id="7c83f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7c83f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7c83f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c83f-111">Permission type</span></span>|<span data-ttu-id="7c83f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7c83f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c83f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c83f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c83f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c83f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7c83f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c83f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c83f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c83f-116">Not supported.</span></span>|
|<span data-ttu-id="7c83f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c83f-117">Application</span></span>|<span data-ttu-id="7c83f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c83f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c83f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c83f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7c83f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c83f-120">Request headers</span></span>
|<span data-ttu-id="7c83f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c83f-121">Header</span></span>|<span data-ttu-id="7c83f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7c83f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c83f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c83f-123">Authorization</span></span>|<span data-ttu-id="7c83f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c83f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c83f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c83f-125">Accept</span></span>|<span data-ttu-id="7c83f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c83f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c83f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c83f-127">Request body</span></span>
<span data-ttu-id="7c83f-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7c83f-128">In the request body, supply a JSON representation for the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

<span data-ttu-id="7c83f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7c83f-129">The following table shows the properties that are required when you create the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

|<span data-ttu-id="7c83f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c83f-130">Property</span></span>|<span data-ttu-id="7c83f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c83f-131">Type</span></span>|<span data-ttu-id="7c83f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c83f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c83f-133">id</span><span class="sxs-lookup"><span data-stu-id="7c83f-133">id</span></span>|<span data-ttu-id="7c83f-134">String</span><span class="sxs-lookup"><span data-stu-id="7c83f-134">String</span></span>|<span data-ttu-id="7c83f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7c83f-135">Key of the entity.</span></span> <span data-ttu-id="7c83f-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c83f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c83f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c83f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7c83f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c83f-138">DateTimeOffset</span></span>|<span data-ttu-id="7c83f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7c83f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7c83f-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c83f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c83f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7c83f-141">roleScopeTagIds</span></span>|<span data-ttu-id="7c83f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="7c83f-142">String collection</span></span>|<span data-ttu-id="7c83f-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="7c83f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7c83f-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c83f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c83f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7c83f-145">supportsScopeTags</span></span>|<span data-ttu-id="7c83f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c83f-146">Boolean</span></span>|<span data-ttu-id="7c83f-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7c83f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7c83f-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7c83f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7c83f-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="7c83f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7c83f-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7c83f-150">This property is read-only.</span></span> <span data-ttu-id="7c83f-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c83f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c83f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c83f-152">createdDateTime</span></span>|<span data-ttu-id="7c83f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c83f-153">DateTimeOffset</span></span>|<span data-ttu-id="7c83f-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7c83f-154">DateTime the object was created.</span></span> <span data-ttu-id="7c83f-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c83f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c83f-156">description</span><span class="sxs-lookup"><span data-stu-id="7c83f-156">description</span></span>|<span data-ttu-id="7c83f-157">String</span><span class="sxs-lookup"><span data-stu-id="7c83f-157">String</span></span>|<span data-ttu-id="7c83f-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7c83f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7c83f-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c83f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c83f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7c83f-160">displayName</span></span>|<span data-ttu-id="7c83f-161">String</span><span class="sxs-lookup"><span data-stu-id="7c83f-161">String</span></span>|<span data-ttu-id="7c83f-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7c83f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7c83f-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c83f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c83f-164">version</span><span class="sxs-lookup"><span data-stu-id="7c83f-164">version</span></span>|<span data-ttu-id="7c83f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7c83f-165">Int32</span></span>|<span data-ttu-id="7c83f-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7c83f-166">Version of the device configuration.</span></span> <span data-ttu-id="7c83f-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7c83f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7c83f-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="7c83f-168">usernameSource</span></span>|[<span data-ttu-id="7c83f-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="7c83f-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7c83f-170">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7c83f-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7c83f-171">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7c83f-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7c83f-172">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7c83f-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7c83f-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="7c83f-173">usernameAADSource</span></span>|[<span data-ttu-id="7c83f-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="7c83f-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="7c83f-175">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="7c83f-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="7c83f-176">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7c83f-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7c83f-177">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="7c83f-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="7c83f-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="7c83f-178">userDomainNameSource</span></span>|[<span data-ttu-id="7c83f-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="7c83f-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="7c83f-180">Atributo nome_do_domínio que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7c83f-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7c83f-181">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="7c83f-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="7c83f-182">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="7c83f-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="7c83f-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="7c83f-183">customDomainName</span></span>|<span data-ttu-id="7c83f-184">String</span><span class="sxs-lookup"><span data-stu-id="7c83f-184">String</span></span>|<span data-ttu-id="7c83f-185">Valor de nome de domínio personalizado usado ao gerar um perfil de email antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7c83f-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="7c83f-186">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="7c83f-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="7c83f-187">accountName</span><span class="sxs-lookup"><span data-stu-id="7c83f-187">accountName</span></span>|<span data-ttu-id="7c83f-188">String</span><span class="sxs-lookup"><span data-stu-id="7c83f-188">String</span></span>|<span data-ttu-id="7c83f-189">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="7c83f-189">Account name.</span></span>|
|<span data-ttu-id="7c83f-190">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="7c83f-190">syncCalendar</span></span>|<span data-ttu-id="7c83f-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c83f-191">Boolean</span></span>|<span data-ttu-id="7c83f-192">Se deseja ou não sincronizar o calendário.</span><span class="sxs-lookup"><span data-stu-id="7c83f-192">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="7c83f-193">syncContacts</span><span class="sxs-lookup"><span data-stu-id="7c83f-193">syncContacts</span></span>|<span data-ttu-id="7c83f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c83f-194">Boolean</span></span>|<span data-ttu-id="7c83f-195">Se deseja ou não sincronizar contatos.</span><span class="sxs-lookup"><span data-stu-id="7c83f-195">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="7c83f-196">syncTasks</span><span class="sxs-lookup"><span data-stu-id="7c83f-196">syncTasks</span></span>|<span data-ttu-id="7c83f-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c83f-197">Boolean</span></span>|<span data-ttu-id="7c83f-198">Se deseja ou não sincronizar tarefas.</span><span class="sxs-lookup"><span data-stu-id="7c83f-198">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="7c83f-199">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="7c83f-199">durationOfEmailToSync</span></span>|[<span data-ttu-id="7c83f-200">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="7c83f-200">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="7c83f-201">Duração de email para sincronizar. Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="7c83f-201">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="7c83f-202">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="7c83f-202">emailAddressSource</span></span>|[<span data-ttu-id="7c83f-203">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="7c83f-203">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="7c83f-204">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7c83f-204">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="7c83f-205">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="7c83f-205">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="7c83f-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="7c83f-206">emailSyncSchedule</span></span>|[<span data-ttu-id="7c83f-207">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="7c83f-207">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="7c83f-208">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="7c83f-208">Email sync schedule.</span></span> <span data-ttu-id="7c83f-209">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="7c83f-209">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="7c83f-210">hostName</span><span class="sxs-lookup"><span data-stu-id="7c83f-210">hostName</span></span>|<span data-ttu-id="7c83f-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7c83f-211">String</span></span>|<span data-ttu-id="7c83f-212">Local do Exchange que (URL) que o aplicativo de email nativo se conecta ao.</span><span class="sxs-lookup"><span data-stu-id="7c83f-212">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="7c83f-213">requireSsl</span><span class="sxs-lookup"><span data-stu-id="7c83f-213">requireSsl</span></span>|<span data-ttu-id="7c83f-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c83f-214">Boolean</span></span>|<span data-ttu-id="7c83f-215">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="7c83f-215">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="7c83f-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c83f-216">Response</span></span>
<span data-ttu-id="7c83f-217">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c83f-217">If successful, this method returns a `200 OK` response code and an updated [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c83f-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c83f-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c83f-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c83f-219">Request</span></span>
<span data-ttu-id="7c83f-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c83f-220">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 753

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```

### <a name="response"></a><span data-ttu-id="7c83f-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c83f-221">Response</span></span>
<span data-ttu-id="7c83f-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c83f-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 925

{
  "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
  "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "usernameSource": "primarySmtpAddress",
  "usernameAADSource": "primarySmtpAddress",
  "userDomainNameSource": "netBiosDomainName",
  "customDomainName": "Custom Domain Name value",
  "accountName": "Account Name value",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true,
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "emailSyncSchedule": "asMessagesArrive",
  "hostName": "Host Name value",
  "requireSsl": true
}
```




