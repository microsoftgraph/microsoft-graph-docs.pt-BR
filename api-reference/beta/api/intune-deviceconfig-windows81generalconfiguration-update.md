---
title: Atualizar windows81GeneralConfiguration
description: Atualizar as propriedades de um objeto windows81GeneralConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 285b568ec1a7ee9da00d8dd54eac507c4f39755f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416221"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="95907-103">Atualizar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="95907-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="95907-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="95907-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="95907-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="95907-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95907-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="95907-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95907-107">Atualizar as propriedades de um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95907-107">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95907-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="95907-108">Prerequisites</span></span>
<span data-ttu-id="95907-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="95907-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="95907-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95907-111">Permission type</span></span>|<span data-ttu-id="95907-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="95907-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95907-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95907-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95907-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95907-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95907-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95907-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95907-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95907-116">Not supported.</span></span>|
|<span data-ttu-id="95907-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95907-117">Application</span></span>|<span data-ttu-id="95907-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95907-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95907-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95907-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="95907-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95907-120">Request headers</span></span>
|<span data-ttu-id="95907-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95907-121">Header</span></span>|<span data-ttu-id="95907-122">Valor</span><span class="sxs-lookup"><span data-stu-id="95907-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95907-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="95907-123">Authorization</span></span>|<span data-ttu-id="95907-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95907-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95907-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="95907-125">Accept</span></span>|<span data-ttu-id="95907-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95907-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95907-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95907-127">Request body</span></span>
<span data-ttu-id="95907-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95907-128">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="95907-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95907-129">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="95907-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95907-130">Property</span></span>|<span data-ttu-id="95907-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="95907-131">Type</span></span>|<span data-ttu-id="95907-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="95907-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95907-133">id</span><span class="sxs-lookup"><span data-stu-id="95907-133">id</span></span>|<span data-ttu-id="95907-134">String</span><span class="sxs-lookup"><span data-stu-id="95907-134">String</span></span>|<span data-ttu-id="95907-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="95907-135">Key of the entity.</span></span> <span data-ttu-id="95907-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95907-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95907-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95907-137">lastModifiedDateTime</span></span>|<span data-ttu-id="95907-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95907-138">DateTimeOffset</span></span>|<span data-ttu-id="95907-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="95907-139">DateTime the object was last modified.</span></span> <span data-ttu-id="95907-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95907-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95907-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95907-141">roleScopeTagIds</span></span>|<span data-ttu-id="95907-142">String collection</span><span class="sxs-lookup"><span data-stu-id="95907-142">String collection</span></span>|<span data-ttu-id="95907-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="95907-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95907-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95907-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95907-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="95907-145">supportsScopeTags</span></span>|<span data-ttu-id="95907-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-146">Boolean</span></span>|<span data-ttu-id="95907-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="95907-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95907-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="95907-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95907-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="95907-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95907-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="95907-150">This property is read-only.</span></span> <span data-ttu-id="95907-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95907-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95907-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95907-152">createdDateTime</span></span>|<span data-ttu-id="95907-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95907-153">DateTimeOffset</span></span>|<span data-ttu-id="95907-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="95907-154">DateTime the object was created.</span></span> <span data-ttu-id="95907-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95907-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95907-156">description</span><span class="sxs-lookup"><span data-stu-id="95907-156">description</span></span>|<span data-ttu-id="95907-157">String</span><span class="sxs-lookup"><span data-stu-id="95907-157">String</span></span>|<span data-ttu-id="95907-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95907-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95907-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95907-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95907-160">displayName</span><span class="sxs-lookup"><span data-stu-id="95907-160">displayName</span></span>|<span data-ttu-id="95907-161">String</span><span class="sxs-lookup"><span data-stu-id="95907-161">String</span></span>|<span data-ttu-id="95907-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95907-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95907-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95907-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95907-164">version</span><span class="sxs-lookup"><span data-stu-id="95907-164">version</span></span>|<span data-ttu-id="95907-165">Int32</span><span class="sxs-lookup"><span data-stu-id="95907-165">Int32</span></span>|<span data-ttu-id="95907-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95907-166">Version of the device configuration.</span></span> <span data-ttu-id="95907-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95907-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95907-168">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="95907-168">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="95907-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-169">Boolean</span></span>|<span data-ttu-id="95907-170">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="95907-170">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="95907-171">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="95907-171">applyOnlyToWindows81</span></span>|<span data-ttu-id="95907-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-172">Boolean</span></span>|<span data-ttu-id="95907-173">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="95907-173">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="95907-174">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="95907-174">This property is read-only.</span></span>|
|<span data-ttu-id="95907-175">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="95907-175">browserBlockAutofill</span></span>|<span data-ttu-id="95907-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-176">Boolean</span></span>|<span data-ttu-id="95907-177">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="95907-177">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="95907-178">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="95907-178">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="95907-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-179">Boolean</span></span>|<span data-ttu-id="95907-180">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="95907-180">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="95907-181">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="95907-181">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="95907-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-182">Boolean</span></span>|<span data-ttu-id="95907-183">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="95907-183">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="95907-184">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="95907-184">browserBlockJavaScript</span></span>|<span data-ttu-id="95907-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-185">Boolean</span></span>|<span data-ttu-id="95907-186">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="95907-186">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="95907-187">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="95907-187">browserBlockPlugins</span></span>|<span data-ttu-id="95907-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-188">Boolean</span></span>|<span data-ttu-id="95907-189">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="95907-189">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="95907-190">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="95907-190">browserBlockPopups</span></span>|<span data-ttu-id="95907-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-191">Boolean</span></span>|<span data-ttu-id="95907-192">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="95907-192">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="95907-193">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="95907-193">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="95907-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-194">Boolean</span></span>|<span data-ttu-id="95907-195">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="95907-195">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="95907-196">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="95907-196">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="95907-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-197">Boolean</span></span>|<span data-ttu-id="95907-198">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="95907-198">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="95907-199">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="95907-199">browserRequireSmartScreen</span></span>|<span data-ttu-id="95907-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-200">Boolean</span></span>|<span data-ttu-id="95907-201">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="95907-201">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="95907-202">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="95907-202">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="95907-203">String</span><span class="sxs-lookup"><span data-stu-id="95907-203">String</span></span>|<span data-ttu-id="95907-204">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="95907-204">The enterprise mode site list location.</span></span> <span data-ttu-id="95907-205">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="95907-205">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="95907-206">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="95907-206">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="95907-207">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="95907-207">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="95907-208">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="95907-208">The internet security level.</span></span> <span data-ttu-id="95907-209">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="95907-209">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="95907-210">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="95907-210">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="95907-211">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="95907-211">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="95907-212">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="95907-212">The Intranet security level.</span></span> <span data-ttu-id="95907-213">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="95907-213">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="95907-214">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="95907-214">browserLoggingReportLocation</span></span>|<span data-ttu-id="95907-215">String</span><span class="sxs-lookup"><span data-stu-id="95907-215">String</span></span>|<span data-ttu-id="95907-216">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="95907-216">The logging report location.</span></span>|
|<span data-ttu-id="95907-217">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="95907-217">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="95907-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-218">Boolean</span></span>|<span data-ttu-id="95907-219">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="95907-219">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="95907-220">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="95907-220">browserRequireFirewall</span></span>|<span data-ttu-id="95907-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-221">Boolean</span></span>|<span data-ttu-id="95907-222">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="95907-222">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="95907-223">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="95907-223">browserRequireFraudWarning</span></span>|<span data-ttu-id="95907-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-224">Boolean</span></span>|<span data-ttu-id="95907-225">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="95907-225">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="95907-226">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="95907-226">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="95907-227">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="95907-227">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="95907-228">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="95907-228">The trusted sites security level.</span></span> <span data-ttu-id="95907-229">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="95907-229">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="95907-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="95907-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="95907-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-231">Boolean</span></span>|<span data-ttu-id="95907-232">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="95907-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="95907-233">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="95907-233">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="95907-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-234">Boolean</span></span>|<span data-ttu-id="95907-235">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="95907-235">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="95907-236">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="95907-236">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="95907-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-237">Boolean</span></span>|<span data-ttu-id="95907-238">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="95907-238">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="95907-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="95907-239">passwordExpirationDays</span></span>|<span data-ttu-id="95907-240">Int32</span><span class="sxs-lookup"><span data-stu-id="95907-240">Int32</span></span>|<span data-ttu-id="95907-241">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="95907-241">Password expiration in days.</span></span>|
|<span data-ttu-id="95907-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="95907-242">passwordMinimumLength</span></span>|<span data-ttu-id="95907-243">Int32</span><span class="sxs-lookup"><span data-stu-id="95907-243">Int32</span></span>|<span data-ttu-id="95907-244">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="95907-244">The minimum password length.</span></span>|
|<span data-ttu-id="95907-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="95907-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="95907-246">Int32</span><span class="sxs-lookup"><span data-stu-id="95907-246">Int32</span></span>|<span data-ttu-id="95907-247">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="95907-247">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="95907-248">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="95907-248">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="95907-249">Int32</span><span class="sxs-lookup"><span data-stu-id="95907-249">Int32</span></span>|<span data-ttu-id="95907-250">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="95907-250">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="95907-251">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="95907-251">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="95907-252">Int32</span><span class="sxs-lookup"><span data-stu-id="95907-252">Int32</span></span>|<span data-ttu-id="95907-253">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="95907-253">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="95907-254">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="95907-254">Valid values 0 to 24</span></span>|
|<span data-ttu-id="95907-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="95907-255">passwordRequiredType</span></span>|[<span data-ttu-id="95907-256">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="95907-256">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="95907-257">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="95907-257">The required password type.</span></span> <span data-ttu-id="95907-258">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="95907-258">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="95907-259">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="95907-259">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="95907-260">Int32</span><span class="sxs-lookup"><span data-stu-id="95907-260">Int32</span></span>|<span data-ttu-id="95907-261">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="95907-261">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="95907-262">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="95907-262">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="95907-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-263">Boolean</span></span>|<span data-ttu-id="95907-264">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="95907-264">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="95907-265">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="95907-265">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="95907-266">updateClassification</span><span class="sxs-lookup"><span data-stu-id="95907-266">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="95907-267">O mínimo de classificação para instalar automaticamente de atualização.</span><span class="sxs-lookup"><span data-stu-id="95907-267">The minimum update classification to install automatically.</span></span> <span data-ttu-id="95907-268">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="95907-268">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="95907-269">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="95907-269">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="95907-270">updateClassification</span><span class="sxs-lookup"><span data-stu-id="95907-270">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="95907-271">O mínimo de classificação para instalar automaticamente de atualização.</span><span class="sxs-lookup"><span data-stu-id="95907-271">The minimum update classification to install automatically.</span></span> <span data-ttu-id="95907-272">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="95907-272">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="95907-273">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="95907-273">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="95907-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="95907-274">Boolean</span></span>|<span data-ttu-id="95907-275">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="95907-275">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="95907-276">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="95907-276">userAccountControlSettings</span></span>|[<span data-ttu-id="95907-277">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="95907-277">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="95907-278">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="95907-278">The user account control settings.</span></span> <span data-ttu-id="95907-279">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="95907-279">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="95907-280">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="95907-280">workFoldersUrl</span></span>|<span data-ttu-id="95907-281">String</span><span class="sxs-lookup"><span data-stu-id="95907-281">String</span></span>|<span data-ttu-id="95907-282">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="95907-282">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="95907-283">Resposta</span><span class="sxs-lookup"><span data-stu-id="95907-283">Response</span></span>
<span data-ttu-id="95907-284">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95907-284">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95907-285">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95907-285">Example</span></span>

### <a name="request"></a><span data-ttu-id="95907-286">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95907-286">Request</span></span>
<span data-ttu-id="95907-287">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95907-287">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1924

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="95907-288">Resposta</span><span class="sxs-lookup"><span data-stu-id="95907-288">Response</span></span>
<span data-ttu-id="95907-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95907-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2096

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```




