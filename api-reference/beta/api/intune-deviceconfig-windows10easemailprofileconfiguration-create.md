---
title: Criar windows10EasEmailProfileConfiguration
description: Crie um novo objeto de windows10EasEmailProfileConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6960e145cf5677dc85ae02baed7aec8dae16e773
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411292"
---
# <a name="create-windows10easemailprofileconfiguration"></a><span data-ttu-id="ca50c-103">Criar windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca50c-103">Create windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="ca50c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ca50c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ca50c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ca50c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca50c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ca50c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca50c-107">Crie um novo objeto de [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ca50c-107">Create a new [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca50c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca50c-108">Prerequisites</span></span>
<span data-ttu-id="ca50c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ca50c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ca50c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca50c-111">Permission type</span></span>|<span data-ttu-id="ca50c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca50c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca50c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca50c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca50c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca50c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca50c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca50c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca50c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca50c-116">Not supported.</span></span>|
|<span data-ttu-id="ca50c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca50c-117">Application</span></span>|<span data-ttu-id="ca50c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca50c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca50c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca50c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ca50c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca50c-120">Request headers</span></span>
|<span data-ttu-id="ca50c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca50c-121">Header</span></span>|<span data-ttu-id="ca50c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ca50c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca50c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca50c-123">Authorization</span></span>|<span data-ttu-id="ca50c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca50c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca50c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca50c-125">Accept</span></span>|<span data-ttu-id="ca50c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca50c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca50c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca50c-127">Request body</span></span>
<span data-ttu-id="ca50c-128">No corpo da solicitação, fornece uma representação JSON para o objeto windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ca50c-128">In the request body, supply a JSON representation for the windows10EasEmailProfileConfiguration object.</span></span>

<span data-ttu-id="ca50c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o windows10EasEmailProfileConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ca50c-129">The following table shows the properties that are required when you create the windows10EasEmailProfileConfiguration.</span></span>

|<span data-ttu-id="ca50c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca50c-130">Property</span></span>|<span data-ttu-id="ca50c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca50c-131">Type</span></span>|<span data-ttu-id="ca50c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca50c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca50c-133">id</span><span class="sxs-lookup"><span data-stu-id="ca50c-133">id</span></span>|<span data-ttu-id="ca50c-134">String</span><span class="sxs-lookup"><span data-stu-id="ca50c-134">String</span></span>|<span data-ttu-id="ca50c-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ca50c-135">Key of the entity.</span></span> <span data-ttu-id="ca50c-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca50c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca50c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca50c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ca50c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca50c-138">DateTimeOffset</span></span>|<span data-ttu-id="ca50c-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ca50c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ca50c-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca50c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca50c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca50c-141">roleScopeTagIds</span></span>|<span data-ttu-id="ca50c-142">String collection</span><span class="sxs-lookup"><span data-stu-id="ca50c-142">String collection</span></span>|<span data-ttu-id="ca50c-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="ca50c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ca50c-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca50c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca50c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ca50c-145">supportsScopeTags</span></span>|<span data-ttu-id="ca50c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca50c-146">Boolean</span></span>|<span data-ttu-id="ca50c-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ca50c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ca50c-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ca50c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ca50c-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="ca50c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ca50c-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca50c-150">This property is read-only.</span></span> <span data-ttu-id="ca50c-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca50c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca50c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca50c-152">createdDateTime</span></span>|<span data-ttu-id="ca50c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca50c-153">DateTimeOffset</span></span>|<span data-ttu-id="ca50c-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ca50c-154">DateTime the object was created.</span></span> <span data-ttu-id="ca50c-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca50c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca50c-156">description</span><span class="sxs-lookup"><span data-stu-id="ca50c-156">description</span></span>|<span data-ttu-id="ca50c-157">String</span><span class="sxs-lookup"><span data-stu-id="ca50c-157">String</span></span>|<span data-ttu-id="ca50c-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca50c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ca50c-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca50c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca50c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ca50c-160">displayName</span></span>|<span data-ttu-id="ca50c-161">String</span><span class="sxs-lookup"><span data-stu-id="ca50c-161">String</span></span>|<span data-ttu-id="ca50c-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca50c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ca50c-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca50c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca50c-164">version</span><span class="sxs-lookup"><span data-stu-id="ca50c-164">version</span></span>|<span data-ttu-id="ca50c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ca50c-165">Int32</span></span>|<span data-ttu-id="ca50c-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca50c-166">Version of the device configuration.</span></span> <span data-ttu-id="ca50c-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca50c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca50c-168">usernameSource</span><span class="sxs-lookup"><span data-stu-id="ca50c-168">usernameSource</span></span>|[<span data-ttu-id="ca50c-169">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="ca50c-169">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="ca50c-170">Atributo de nome de usuário que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca50c-170">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ca50c-171">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="ca50c-171">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="ca50c-172">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="ca50c-172">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="ca50c-173">usernameAADSource</span><span class="sxs-lookup"><span data-stu-id="ca50c-173">usernameAADSource</span></span>|[<span data-ttu-id="ca50c-174">usernameSource</span><span class="sxs-lookup"><span data-stu-id="ca50c-174">usernameSource</span></span>](../resources/intune-deviceconfig-usernamesource.md)|<span data-ttu-id="ca50c-175">Nome do campo AAD, que será usado para recuperar o nome de usuário para o perfil de email.</span><span class="sxs-lookup"><span data-stu-id="ca50c-175">Name of the AAD field, that will be used to retrieve UserName for email profile.</span></span> <span data-ttu-id="ca50c-176">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="ca50c-176">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="ca50c-177">Os valores possíveis são: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span><span class="sxs-lookup"><span data-stu-id="ca50c-177">Possible values are: `userPrincipalName`, `primarySmtpAddress`, `samAccountName`.</span></span>|
|<span data-ttu-id="ca50c-178">userDomainNameSource</span><span class="sxs-lookup"><span data-stu-id="ca50c-178">userDomainNameSource</span></span>|[<span data-ttu-id="ca50c-179">domainNameSource</span><span class="sxs-lookup"><span data-stu-id="ca50c-179">domainNameSource</span></span>](../resources/intune-deviceconfig-domainnamesource.md)|<span data-ttu-id="ca50c-180">Atributo nome_do_domínio que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca50c-180">UserDomainname attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ca50c-181">Herdada do [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="ca50c-181">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md).</span></span> <span data-ttu-id="ca50c-182">Os valores possíveis são: `fullDomainName` e `netBiosDomainName`.</span><span class="sxs-lookup"><span data-stu-id="ca50c-182">Possible values are: `fullDomainName`, `netBiosDomainName`.</span></span>|
|<span data-ttu-id="ca50c-183">customDomainName</span><span class="sxs-lookup"><span data-stu-id="ca50c-183">customDomainName</span></span>|<span data-ttu-id="ca50c-184">String</span><span class="sxs-lookup"><span data-stu-id="ca50c-184">String</span></span>|<span data-ttu-id="ca50c-185">Valor de nome de domínio personalizado usado ao gerar um perfil de email antes de instalar no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca50c-185">Custom domain name value used while generating an email profile before installing on the device.</span></span> <span data-ttu-id="ca50c-186">Herdado de [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="ca50c-186">Inherited from [easEmailProfileConfigurationBase](../resources/intune-deviceconfig-easemailprofileconfigurationbase.md)</span></span>|
|<span data-ttu-id="ca50c-187">accountName</span><span class="sxs-lookup"><span data-stu-id="ca50c-187">accountName</span></span>|<span data-ttu-id="ca50c-188">String</span><span class="sxs-lookup"><span data-stu-id="ca50c-188">String</span></span>|<span data-ttu-id="ca50c-189">Nome da conta.</span><span class="sxs-lookup"><span data-stu-id="ca50c-189">Account name.</span></span>|
|<span data-ttu-id="ca50c-190">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="ca50c-190">syncCalendar</span></span>|<span data-ttu-id="ca50c-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca50c-191">Boolean</span></span>|<span data-ttu-id="ca50c-192">Se deseja ou não sincronizar o calendário.</span><span class="sxs-lookup"><span data-stu-id="ca50c-192">Whether or not to sync the calendar.</span></span>|
|<span data-ttu-id="ca50c-193">syncContacts</span><span class="sxs-lookup"><span data-stu-id="ca50c-193">syncContacts</span></span>|<span data-ttu-id="ca50c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca50c-194">Boolean</span></span>|<span data-ttu-id="ca50c-195">Se deseja ou não sincronizar contatos.</span><span class="sxs-lookup"><span data-stu-id="ca50c-195">Whether or not to sync contacts.</span></span>|
|<span data-ttu-id="ca50c-196">syncTasks</span><span class="sxs-lookup"><span data-stu-id="ca50c-196">syncTasks</span></span>|<span data-ttu-id="ca50c-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca50c-197">Boolean</span></span>|<span data-ttu-id="ca50c-198">Se deseja ou não sincronizar tarefas.</span><span class="sxs-lookup"><span data-stu-id="ca50c-198">Whether or not to sync tasks.</span></span>|
|<span data-ttu-id="ca50c-199">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="ca50c-199">durationOfEmailToSync</span></span>|[<span data-ttu-id="ca50c-200">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="ca50c-200">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="ca50c-201">Duração de email para sincronizar. Os valores possíveis são: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span><span class="sxs-lookup"><span data-stu-id="ca50c-201">Duration of email to sync. Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="ca50c-202">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="ca50c-202">emailAddressSource</span></span>|[<span data-ttu-id="ca50c-203">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="ca50c-203">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="ca50c-204">Atributo de email que é separado a partir do AAD e inserido nesse perfil antes da instalação no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca50c-204">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ca50c-205">Os valores possíveis são: `userPrincipalName` e `primarySmtpAddress`.</span><span class="sxs-lookup"><span data-stu-id="ca50c-205">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="ca50c-206">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="ca50c-206">emailSyncSchedule</span></span>|[<span data-ttu-id="ca50c-207">emailSyncSchedule</span><span class="sxs-lookup"><span data-stu-id="ca50c-207">emailSyncSchedule</span></span>](../resources/intune-deviceconfig-emailsyncschedule.md)|<span data-ttu-id="ca50c-208">Agenda de sincronização de email.</span><span class="sxs-lookup"><span data-stu-id="ca50c-208">Email sync schedule.</span></span> <span data-ttu-id="ca50c-209">Os valores possíveis são: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span><span class="sxs-lookup"><span data-stu-id="ca50c-209">Possible values are: `userDefined`, `asMessagesArrive`, `manual`, `fifteenMinutes`, `thirtyMinutes`, `sixtyMinutes`, `basedOnMyUsage`.</span></span>|
|<span data-ttu-id="ca50c-210">hostName</span><span class="sxs-lookup"><span data-stu-id="ca50c-210">hostName</span></span>|<span data-ttu-id="ca50c-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca50c-211">String</span></span>|<span data-ttu-id="ca50c-212">Local do Exchange que (URL) que o aplicativo de email nativo se conecta ao.</span><span class="sxs-lookup"><span data-stu-id="ca50c-212">Exchange location that (URL) that the native mail app connects to.</span></span>|
|<span data-ttu-id="ca50c-213">requireSsl</span><span class="sxs-lookup"><span data-stu-id="ca50c-213">requireSsl</span></span>|<span data-ttu-id="ca50c-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca50c-214">Boolean</span></span>|<span data-ttu-id="ca50c-215">Indica se deve ou não usar SSL.</span><span class="sxs-lookup"><span data-stu-id="ca50c-215">Indicates whether or not to use SSL.</span></span>|



## <a name="response"></a><span data-ttu-id="ca50c-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca50c-216">Response</span></span>
<span data-ttu-id="ca50c-217">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca50c-217">If successful, this method returns a `201 Created` response code and a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca50c-218">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca50c-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca50c-219">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca50c-219">Request</span></span>
<span data-ttu-id="ca50c-220">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca50c-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="ca50c-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca50c-221">Response</span></span>
<span data-ttu-id="ca50c-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca50c-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




