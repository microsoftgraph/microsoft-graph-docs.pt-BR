---
title: Criar windows81GeneralConfiguration
description: Criar um novo objeto windows81GeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a205fce73ab918107a4aa4582e08f92b2e1fdc2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33918273"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="4028e-103">Criar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4028e-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="4028e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4028e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4028e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4028e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4028e-106">Criar um novo objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4028e-106">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4028e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4028e-107">Prerequisites</span></span>
<span data-ttu-id="4028e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4028e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4028e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4028e-110">Permission type</span></span>|<span data-ttu-id="4028e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4028e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4028e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4028e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4028e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4028e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4028e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4028e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4028e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4028e-115">Not supported.</span></span>|
|<span data-ttu-id="4028e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4028e-116">Application</span></span>|<span data-ttu-id="4028e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4028e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4028e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4028e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4028e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4028e-119">Request headers</span></span>
|<span data-ttu-id="4028e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4028e-120">Header</span></span>|<span data-ttu-id="4028e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4028e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4028e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4028e-122">Authorization</span></span>|<span data-ttu-id="4028e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4028e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4028e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4028e-124">Accept</span></span>|<span data-ttu-id="4028e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4028e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4028e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4028e-126">Request body</span></span>
<span data-ttu-id="4028e-127">No corpo da solicitação, forneça uma representação JSON do objeto windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4028e-127">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="4028e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4028e-128">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="4028e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4028e-129">Property</span></span>|<span data-ttu-id="4028e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4028e-130">Type</span></span>|<span data-ttu-id="4028e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4028e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4028e-132">id</span><span class="sxs-lookup"><span data-stu-id="4028e-132">id</span></span>|<span data-ttu-id="4028e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4028e-133">String</span></span>|<span data-ttu-id="4028e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4028e-134">Key of the entity.</span></span> <span data-ttu-id="4028e-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4028e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4028e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4028e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4028e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4028e-137">DateTimeOffset</span></span>|<span data-ttu-id="4028e-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4028e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4028e-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4028e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4028e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4028e-140">roleScopeTagIds</span></span>|<span data-ttu-id="4028e-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4028e-141">String collection</span></span>|<span data-ttu-id="4028e-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="4028e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4028e-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4028e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4028e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4028e-144">supportsScopeTags</span></span>|<span data-ttu-id="4028e-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-145">Boolean</span></span>|<span data-ttu-id="4028e-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4028e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4028e-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4028e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4028e-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4028e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4028e-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4028e-149">This property is read-only.</span></span> <span data-ttu-id="4028e-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4028e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4028e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4028e-151">createdDateTime</span></span>|<span data-ttu-id="4028e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4028e-152">DateTimeOffset</span></span>|<span data-ttu-id="4028e-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4028e-153">DateTime the object was created.</span></span> <span data-ttu-id="4028e-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4028e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4028e-155">description</span><span class="sxs-lookup"><span data-stu-id="4028e-155">description</span></span>|<span data-ttu-id="4028e-156">String</span><span class="sxs-lookup"><span data-stu-id="4028e-156">String</span></span>|<span data-ttu-id="4028e-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4028e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4028e-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4028e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4028e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4028e-159">displayName</span></span>|<span data-ttu-id="4028e-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4028e-160">String</span></span>|<span data-ttu-id="4028e-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4028e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4028e-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4028e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4028e-163">versão</span><span class="sxs-lookup"><span data-stu-id="4028e-163">version</span></span>|<span data-ttu-id="4028e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4028e-164">Int32</span></span>|<span data-ttu-id="4028e-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4028e-165">Version of the device configuration.</span></span> <span data-ttu-id="4028e-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4028e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4028e-167">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="4028e-167">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="4028e-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-168">Boolean</span></span>|<span data-ttu-id="4028e-169">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4028e-169">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="4028e-170">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="4028e-170">applyOnlyToWindows81</span></span>|<span data-ttu-id="4028e-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-171">Boolean</span></span>|<span data-ttu-id="4028e-172">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="4028e-172">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="4028e-173">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4028e-173">This property is read-only.</span></span>|
|<span data-ttu-id="4028e-174">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="4028e-174">browserBlockAutofill</span></span>|<span data-ttu-id="4028e-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-175">Boolean</span></span>|<span data-ttu-id="4028e-176">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4028e-176">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="4028e-177">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="4028e-177">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="4028e-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-178">Boolean</span></span>|<span data-ttu-id="4028e-179">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4028e-179">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="4028e-180">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="4028e-180">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="4028e-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-181">Boolean</span></span>|<span data-ttu-id="4028e-182">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4028e-182">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="4028e-183">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="4028e-183">browserBlockJavaScript</span></span>|<span data-ttu-id="4028e-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-184">Boolean</span></span>|<span data-ttu-id="4028e-185">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="4028e-185">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="4028e-186">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="4028e-186">browserBlockPlugins</span></span>|<span data-ttu-id="4028e-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-187">Boolean</span></span>|<span data-ttu-id="4028e-188">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4028e-188">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="4028e-189">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="4028e-189">browserBlockPopups</span></span>|<span data-ttu-id="4028e-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-190">Boolean</span></span>|<span data-ttu-id="4028e-191">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="4028e-191">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="4028e-192">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="4028e-192">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="4028e-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-193">Boolean</span></span>|<span data-ttu-id="4028e-194">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="4028e-194">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="4028e-195">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="4028e-195">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="4028e-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-196">Boolean</span></span>|<span data-ttu-id="4028e-197">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4028e-197">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="4028e-198">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="4028e-198">browserRequireSmartScreen</span></span>|<span data-ttu-id="4028e-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-199">Boolean</span></span>|<span data-ttu-id="4028e-200">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="4028e-200">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="4028e-201">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="4028e-201">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="4028e-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4028e-202">String</span></span>|<span data-ttu-id="4028e-203">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="4028e-203">The enterprise mode site list location.</span></span> <span data-ttu-id="4028e-204">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="4028e-204">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="4028e-205">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4028e-205">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="4028e-206">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4028e-206">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="4028e-207">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="4028e-207">The internet security level.</span></span> <span data-ttu-id="4028e-208">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="4028e-208">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="4028e-209">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4028e-209">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="4028e-210">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4028e-210">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="4028e-211">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="4028e-211">The Intranet security level.</span></span> <span data-ttu-id="4028e-212">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="4028e-212">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="4028e-213">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="4028e-213">browserLoggingReportLocation</span></span>|<span data-ttu-id="4028e-214">String</span><span class="sxs-lookup"><span data-stu-id="4028e-214">String</span></span>|<span data-ttu-id="4028e-215">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="4028e-215">The logging report location.</span></span>|
|<span data-ttu-id="4028e-216">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="4028e-216">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="4028e-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-217">Boolean</span></span>|<span data-ttu-id="4028e-218">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="4028e-218">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="4028e-219">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="4028e-219">browserRequireFirewall</span></span>|<span data-ttu-id="4028e-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-220">Boolean</span></span>|<span data-ttu-id="4028e-221">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="4028e-221">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="4028e-222">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="4028e-222">browserRequireFraudWarning</span></span>|<span data-ttu-id="4028e-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="4028e-223">Boolean</span></span>|<span data-ttu-id="4028e-224">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="4028e-224">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="4028e-225">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4028e-225">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="4028e-226">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="4028e-226">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="4028e-227">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="4028e-227">The trusted sites security level.</span></span> <span data-ttu-id="4028e-228">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="4028e-228">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="4028e-229">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="4028e-229">cellularBlockDataRoaming</span></span>|<span data-ttu-id="4028e-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-230">Boolean</span></span>|<span data-ttu-id="4028e-231">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4028e-231">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="4028e-232">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="4028e-232">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="4028e-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-233">Boolean</span></span>|<span data-ttu-id="4028e-234">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4028e-234">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4028e-235">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="4028e-235">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="4028e-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-236">Boolean</span></span>|<span data-ttu-id="4028e-237">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="4028e-237">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="4028e-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4028e-238">passwordExpirationDays</span></span>|<span data-ttu-id="4028e-239">Int32</span><span class="sxs-lookup"><span data-stu-id="4028e-239">Int32</span></span>|<span data-ttu-id="4028e-240">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="4028e-240">Password expiration in days.</span></span>|
|<span data-ttu-id="4028e-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4028e-241">passwordMinimumLength</span></span>|<span data-ttu-id="4028e-242">Int32</span><span class="sxs-lookup"><span data-stu-id="4028e-242">Int32</span></span>|<span data-ttu-id="4028e-243">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="4028e-243">The minimum password length.</span></span>|
|<span data-ttu-id="4028e-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4028e-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4028e-245">Int32</span><span class="sxs-lookup"><span data-stu-id="4028e-245">Int32</span></span>|<span data-ttu-id="4028e-246">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="4028e-246">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4028e-247">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4028e-247">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4028e-248">Int32</span><span class="sxs-lookup"><span data-stu-id="4028e-248">Int32</span></span>|<span data-ttu-id="4028e-249">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="4028e-249">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="4028e-250">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4028e-250">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4028e-251">Int32</span><span class="sxs-lookup"><span data-stu-id="4028e-251">Int32</span></span>|<span data-ttu-id="4028e-252">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="4028e-252">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="4028e-253">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="4028e-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4028e-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4028e-254">passwordRequiredType</span></span>|[<span data-ttu-id="4028e-255">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4028e-255">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4028e-256">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="4028e-256">The required password type.</span></span> <span data-ttu-id="4028e-257">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4028e-257">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4028e-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4028e-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4028e-259">Int32</span><span class="sxs-lookup"><span data-stu-id="4028e-259">Int32</span></span>|<span data-ttu-id="4028e-260">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="4028e-260">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="4028e-261">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="4028e-261">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="4028e-262">Booliano</span><span class="sxs-lookup"><span data-stu-id="4028e-262">Boolean</span></span>|<span data-ttu-id="4028e-263">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="4028e-263">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="4028e-264">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="4028e-264">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="4028e-265">updateClassification</span><span class="sxs-lookup"><span data-stu-id="4028e-265">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="4028e-266">A classificação de atualização mínima para instalar automaticamente.</span><span class="sxs-lookup"><span data-stu-id="4028e-266">The minimum update classification to install automatically.</span></span> <span data-ttu-id="4028e-267">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="4028e-267">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="4028e-268">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="4028e-268">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="4028e-269">updateClassification</span><span class="sxs-lookup"><span data-stu-id="4028e-269">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="4028e-270">A classificação de atualização mínima para instalar automaticamente.</span><span class="sxs-lookup"><span data-stu-id="4028e-270">The minimum update classification to install automatically.</span></span> <span data-ttu-id="4028e-271">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="4028e-271">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="4028e-272">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="4028e-272">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="4028e-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="4028e-273">Boolean</span></span>|<span data-ttu-id="4028e-274">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="4028e-274">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="4028e-275">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="4028e-275">userAccountControlSettings</span></span>|[<span data-ttu-id="4028e-276">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="4028e-276">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="4028e-277">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="4028e-277">The user account control settings.</span></span> <span data-ttu-id="4028e-278">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="4028e-278">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="4028e-279">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="4028e-279">workFoldersUrl</span></span>|<span data-ttu-id="4028e-280">String</span><span class="sxs-lookup"><span data-stu-id="4028e-280">String</span></span>|<span data-ttu-id="4028e-281">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="4028e-281">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="4028e-282">Resposta</span><span class="sxs-lookup"><span data-stu-id="4028e-282">Response</span></span>
<span data-ttu-id="4028e-283">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4028e-283">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4028e-284">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4028e-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="4028e-285">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4028e-285">Request</span></span>
<span data-ttu-id="4028e-286">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4028e-286">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4028e-287">Resposta</span><span class="sxs-lookup"><span data-stu-id="4028e-287">Response</span></span>
<span data-ttu-id="4028e-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4028e-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




