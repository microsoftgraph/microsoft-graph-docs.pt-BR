---
title: Criar windows81GeneralConfiguration
description: Criar um novo objeto windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ec40f8fbea8ba5f5c8d6c7d810a0bc9cc55086c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32515392"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="3de7f-103">Criar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="3de7f-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="3de7f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3de7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3de7f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3de7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3de7f-106">Criar um novo objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de7f-106">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3de7f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3de7f-107">Prerequisites</span></span>
<span data-ttu-id="3de7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3de7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3de7f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3de7f-110">Permission type</span></span>|<span data-ttu-id="3de7f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3de7f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3de7f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3de7f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3de7f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3de7f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3de7f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3de7f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3de7f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3de7f-115">Not supported.</span></span>|
|<span data-ttu-id="3de7f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3de7f-116">Application</span></span>|<span data-ttu-id="3de7f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3de7f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3de7f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3de7f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3de7f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3de7f-119">Request headers</span></span>
|<span data-ttu-id="3de7f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3de7f-120">Header</span></span>|<span data-ttu-id="3de7f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3de7f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3de7f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3de7f-122">Authorization</span></span>|<span data-ttu-id="3de7f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3de7f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3de7f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3de7f-124">Accept</span></span>|<span data-ttu-id="3de7f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3de7f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3de7f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3de7f-126">Request body</span></span>
<span data-ttu-id="3de7f-127">No corpo da solicitação, forneça uma representação JSON do objeto windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3de7f-127">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="3de7f-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3de7f-128">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="3de7f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3de7f-129">Property</span></span>|<span data-ttu-id="3de7f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3de7f-130">Type</span></span>|<span data-ttu-id="3de7f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3de7f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3de7f-132">id</span><span class="sxs-lookup"><span data-stu-id="3de7f-132">id</span></span>|<span data-ttu-id="3de7f-133">String</span><span class="sxs-lookup"><span data-stu-id="3de7f-133">String</span></span>|<span data-ttu-id="3de7f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3de7f-134">Key of the entity.</span></span> <span data-ttu-id="3de7f-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3de7f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de7f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3de7f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3de7f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de7f-137">DateTimeOffset</span></span>|<span data-ttu-id="3de7f-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3de7f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3de7f-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3de7f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de7f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3de7f-140">roleScopeTagIds</span></span>|<span data-ttu-id="3de7f-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3de7f-141">String collection</span></span>|<span data-ttu-id="3de7f-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3de7f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3de7f-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3de7f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de7f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3de7f-144">supportsScopeTags</span></span>|<span data-ttu-id="3de7f-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-145">Boolean</span></span>|<span data-ttu-id="3de7f-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3de7f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3de7f-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3de7f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3de7f-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3de7f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3de7f-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3de7f-149">This property is read-only.</span></span> <span data-ttu-id="3de7f-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3de7f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de7f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3de7f-151">createdDateTime</span></span>|<span data-ttu-id="3de7f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de7f-152">DateTimeOffset</span></span>|<span data-ttu-id="3de7f-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3de7f-153">DateTime the object was created.</span></span> <span data-ttu-id="3de7f-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3de7f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de7f-155">description</span><span class="sxs-lookup"><span data-stu-id="3de7f-155">description</span></span>|<span data-ttu-id="3de7f-156">String</span><span class="sxs-lookup"><span data-stu-id="3de7f-156">String</span></span>|<span data-ttu-id="3de7f-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3de7f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3de7f-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3de7f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de7f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3de7f-159">displayName</span></span>|<span data-ttu-id="3de7f-160">String</span><span class="sxs-lookup"><span data-stu-id="3de7f-160">String</span></span>|<span data-ttu-id="3de7f-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3de7f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3de7f-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3de7f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de7f-163">versão</span><span class="sxs-lookup"><span data-stu-id="3de7f-163">version</span></span>|<span data-ttu-id="3de7f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3de7f-164">Int32</span></span>|<span data-ttu-id="3de7f-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3de7f-165">Version of the device configuration.</span></span> <span data-ttu-id="3de7f-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3de7f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de7f-167">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="3de7f-167">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="3de7f-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-168">Boolean</span></span>|<span data-ttu-id="3de7f-169">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3de7f-169">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="3de7f-170">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="3de7f-170">applyOnlyToWindows81</span></span>|<span data-ttu-id="3de7f-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-171">Boolean</span></span>|<span data-ttu-id="3de7f-172">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="3de7f-172">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="3de7f-173">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3de7f-173">This property is read-only.</span></span>|
|<span data-ttu-id="3de7f-174">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="3de7f-174">browserBlockAutofill</span></span>|<span data-ttu-id="3de7f-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-175">Boolean</span></span>|<span data-ttu-id="3de7f-176">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3de7f-176">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="3de7f-177">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="3de7f-177">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="3de7f-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-178">Boolean</span></span>|<span data-ttu-id="3de7f-179">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="3de7f-179">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="3de7f-180">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="3de7f-180">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="3de7f-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-181">Boolean</span></span>|<span data-ttu-id="3de7f-182">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3de7f-182">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="3de7f-183">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="3de7f-183">browserBlockJavaScript</span></span>|<span data-ttu-id="3de7f-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-184">Boolean</span></span>|<span data-ttu-id="3de7f-185">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="3de7f-185">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="3de7f-186">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="3de7f-186">browserBlockPlugins</span></span>|<span data-ttu-id="3de7f-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-187">Boolean</span></span>|<span data-ttu-id="3de7f-188">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="3de7f-188">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="3de7f-189">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="3de7f-189">browserBlockPopups</span></span>|<span data-ttu-id="3de7f-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-190">Boolean</span></span>|<span data-ttu-id="3de7f-191">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="3de7f-191">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="3de7f-192">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="3de7f-192">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="3de7f-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-193">Boolean</span></span>|<span data-ttu-id="3de7f-194">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="3de7f-194">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="3de7f-195">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="3de7f-195">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="3de7f-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-196">Boolean</span></span>|<span data-ttu-id="3de7f-197">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="3de7f-197">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="3de7f-198">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="3de7f-198">browserRequireSmartScreen</span></span>|<span data-ttu-id="3de7f-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-199">Boolean</span></span>|<span data-ttu-id="3de7f-200">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="3de7f-200">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="3de7f-201">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="3de7f-201">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="3de7f-202">String</span><span class="sxs-lookup"><span data-stu-id="3de7f-202">String</span></span>|<span data-ttu-id="3de7f-203">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="3de7f-203">The enterprise mode site list location.</span></span> <span data-ttu-id="3de7f-204">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="3de7f-204">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="3de7f-205">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3de7f-205">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="3de7f-206">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3de7f-206">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="3de7f-207">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="3de7f-207">The internet security level.</span></span> <span data-ttu-id="3de7f-208">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="3de7f-208">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="3de7f-209">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3de7f-209">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="3de7f-210">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3de7f-210">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="3de7f-211">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="3de7f-211">The Intranet security level.</span></span> <span data-ttu-id="3de7f-212">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="3de7f-212">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="3de7f-213">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="3de7f-213">browserLoggingReportLocation</span></span>|<span data-ttu-id="3de7f-214">String</span><span class="sxs-lookup"><span data-stu-id="3de7f-214">String</span></span>|<span data-ttu-id="3de7f-215">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="3de7f-215">The logging report location.</span></span>|
|<span data-ttu-id="3de7f-216">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="3de7f-216">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="3de7f-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-217">Boolean</span></span>|<span data-ttu-id="3de7f-218">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="3de7f-218">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="3de7f-219">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="3de7f-219">browserRequireFirewall</span></span>|<span data-ttu-id="3de7f-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-220">Boolean</span></span>|<span data-ttu-id="3de7f-221">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="3de7f-221">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="3de7f-222">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="3de7f-222">browserRequireFraudWarning</span></span>|<span data-ttu-id="3de7f-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="3de7f-223">Boolean</span></span>|<span data-ttu-id="3de7f-224">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="3de7f-224">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="3de7f-225">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3de7f-225">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="3de7f-226">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3de7f-226">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="3de7f-227">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="3de7f-227">The trusted sites security level.</span></span> <span data-ttu-id="3de7f-228">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="3de7f-228">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="3de7f-229">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="3de7f-229">cellularBlockDataRoaming</span></span>|<span data-ttu-id="3de7f-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-230">Boolean</span></span>|<span data-ttu-id="3de7f-231">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3de7f-231">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="3de7f-232">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="3de7f-232">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="3de7f-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-233">Boolean</span></span>|<span data-ttu-id="3de7f-234">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="3de7f-234">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="3de7f-235">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="3de7f-235">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="3de7f-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-236">Boolean</span></span>|<span data-ttu-id="3de7f-237">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="3de7f-237">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="3de7f-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3de7f-238">passwordExpirationDays</span></span>|<span data-ttu-id="3de7f-239">Int32</span><span class="sxs-lookup"><span data-stu-id="3de7f-239">Int32</span></span>|<span data-ttu-id="3de7f-240">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="3de7f-240">Password expiration in days.</span></span>|
|<span data-ttu-id="3de7f-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3de7f-241">passwordMinimumLength</span></span>|<span data-ttu-id="3de7f-242">Int32</span><span class="sxs-lookup"><span data-stu-id="3de7f-242">Int32</span></span>|<span data-ttu-id="3de7f-243">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="3de7f-243">The minimum password length.</span></span>|
|<span data-ttu-id="3de7f-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="3de7f-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="3de7f-245">Int32</span><span class="sxs-lookup"><span data-stu-id="3de7f-245">Int32</span></span>|<span data-ttu-id="3de7f-246">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="3de7f-246">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="3de7f-247">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3de7f-247">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3de7f-248">Int32</span><span class="sxs-lookup"><span data-stu-id="3de7f-248">Int32</span></span>|<span data-ttu-id="3de7f-249">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="3de7f-249">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3de7f-250">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3de7f-250">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3de7f-251">Int32</span><span class="sxs-lookup"><span data-stu-id="3de7f-251">Int32</span></span>|<span data-ttu-id="3de7f-252">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="3de7f-252">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="3de7f-253">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="3de7f-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="3de7f-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3de7f-254">passwordRequiredType</span></span>|[<span data-ttu-id="3de7f-255">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3de7f-255">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3de7f-256">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="3de7f-256">The required password type.</span></span> <span data-ttu-id="3de7f-257">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="3de7f-257">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3de7f-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="3de7f-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="3de7f-259">Int32</span><span class="sxs-lookup"><span data-stu-id="3de7f-259">Int32</span></span>|<span data-ttu-id="3de7f-260">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="3de7f-260">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="3de7f-261">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="3de7f-261">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="3de7f-262">Booliano</span><span class="sxs-lookup"><span data-stu-id="3de7f-262">Boolean</span></span>|<span data-ttu-id="3de7f-263">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="3de7f-263">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="3de7f-264">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="3de7f-264">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="3de7f-265">updateClassification</span><span class="sxs-lookup"><span data-stu-id="3de7f-265">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="3de7f-266">A classificação de atualização mínima para instalar automaticamente.</span><span class="sxs-lookup"><span data-stu-id="3de7f-266">The minimum update classification to install automatically.</span></span> <span data-ttu-id="3de7f-267">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="3de7f-267">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="3de7f-268">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="3de7f-268">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="3de7f-269">updateClassification</span><span class="sxs-lookup"><span data-stu-id="3de7f-269">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="3de7f-270">A classificação de atualização mínima para instalar automaticamente.</span><span class="sxs-lookup"><span data-stu-id="3de7f-270">The minimum update classification to install automatically.</span></span> <span data-ttu-id="3de7f-271">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="3de7f-271">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="3de7f-272">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="3de7f-272">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="3de7f-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="3de7f-273">Boolean</span></span>|<span data-ttu-id="3de7f-274">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="3de7f-274">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="3de7f-275">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="3de7f-275">userAccountControlSettings</span></span>|[<span data-ttu-id="3de7f-276">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="3de7f-276">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="3de7f-277">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="3de7f-277">The user account control settings.</span></span> <span data-ttu-id="3de7f-278">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="3de7f-278">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="3de7f-279">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="3de7f-279">workFoldersUrl</span></span>|<span data-ttu-id="3de7f-280">String</span><span class="sxs-lookup"><span data-stu-id="3de7f-280">String</span></span>|<span data-ttu-id="3de7f-281">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="3de7f-281">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="3de7f-282">Resposta</span><span class="sxs-lookup"><span data-stu-id="3de7f-282">Response</span></span>
<span data-ttu-id="3de7f-283">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3de7f-283">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3de7f-284">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3de7f-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="3de7f-285">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3de7f-285">Request</span></span>
<span data-ttu-id="3de7f-286">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3de7f-286">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3de7f-287">Resposta</span><span class="sxs-lookup"><span data-stu-id="3de7f-287">Response</span></span>
<span data-ttu-id="3de7f-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3de7f-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





