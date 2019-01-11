---
title: Criar windows81GeneralConfiguration
description: Criar um novo objeto windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 486b21ac0e420188dac738f9c8c2e53c78dbe30d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863858"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="8d811-103">Criar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d811-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="8d811-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8d811-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d811-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8d811-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d811-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8d811-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d811-107">Criar um novo objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8d811-107">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d811-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d811-108">Prerequisites</span></span>
<span data-ttu-id="8d811-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d811-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d811-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d811-111">Permission type</span></span>|<span data-ttu-id="8d811-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8d811-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d811-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d811-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d811-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d811-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d811-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d811-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d811-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d811-116">Not supported.</span></span>|
|<span data-ttu-id="8d811-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d811-117">Application</span></span>|<span data-ttu-id="8d811-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d811-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d811-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d811-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8d811-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d811-120">Request headers</span></span>
|<span data-ttu-id="8d811-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d811-121">Header</span></span>|<span data-ttu-id="8d811-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8d811-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d811-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d811-123">Authorization</span></span>|<span data-ttu-id="8d811-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d811-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d811-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8d811-125">Accept</span></span>|<span data-ttu-id="8d811-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d811-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d811-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d811-127">Request body</span></span>
<span data-ttu-id="8d811-128">No corpo da solicitação, forneça uma representação JSON do objeto windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8d811-128">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="8d811-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8d811-129">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="8d811-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d811-130">Property</span></span>|<span data-ttu-id="8d811-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d811-131">Type</span></span>|<span data-ttu-id="8d811-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d811-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d811-133">id</span><span class="sxs-lookup"><span data-stu-id="8d811-133">id</span></span>|<span data-ttu-id="8d811-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d811-134">String</span></span>|<span data-ttu-id="8d811-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8d811-135">Key of the entity.</span></span> <span data-ttu-id="8d811-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d811-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d811-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d811-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8d811-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d811-138">DateTimeOffset</span></span>|<span data-ttu-id="8d811-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8d811-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8d811-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d811-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d811-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8d811-141">roleScopeTagIds</span></span>|<span data-ttu-id="8d811-142">String collection</span><span class="sxs-lookup"><span data-stu-id="8d811-142">String collection</span></span>|<span data-ttu-id="8d811-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="8d811-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8d811-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d811-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d811-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8d811-145">supportsScopeTags</span></span>|<span data-ttu-id="8d811-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-146">Boolean</span></span>|<span data-ttu-id="8d811-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="8d811-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8d811-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="8d811-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8d811-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="8d811-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8d811-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8d811-150">This property is read-only.</span></span> <span data-ttu-id="8d811-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d811-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d811-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d811-152">createdDateTime</span></span>|<span data-ttu-id="8d811-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d811-153">DateTimeOffset</span></span>|<span data-ttu-id="8d811-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8d811-154">DateTime the object was created.</span></span> <span data-ttu-id="8d811-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d811-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d811-156">description</span><span class="sxs-lookup"><span data-stu-id="8d811-156">description</span></span>|<span data-ttu-id="8d811-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d811-157">String</span></span>|<span data-ttu-id="8d811-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8d811-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8d811-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d811-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d811-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8d811-160">displayName</span></span>|<span data-ttu-id="8d811-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d811-161">String</span></span>|<span data-ttu-id="8d811-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8d811-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8d811-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d811-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d811-164">version</span><span class="sxs-lookup"><span data-stu-id="8d811-164">version</span></span>|<span data-ttu-id="8d811-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8d811-165">Int32</span></span>|<span data-ttu-id="8d811-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8d811-166">Version of the device configuration.</span></span> <span data-ttu-id="8d811-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8d811-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d811-168">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="8d811-168">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="8d811-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-169">Boolean</span></span>|<span data-ttu-id="8d811-170">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8d811-170">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="8d811-171">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="8d811-171">applyOnlyToWindows81</span></span>|<span data-ttu-id="8d811-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-172">Boolean</span></span>|<span data-ttu-id="8d811-173">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="8d811-173">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="8d811-174">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8d811-174">This property is read-only.</span></span>|
|<span data-ttu-id="8d811-175">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="8d811-175">browserBlockAutofill</span></span>|<span data-ttu-id="8d811-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-176">Boolean</span></span>|<span data-ttu-id="8d811-177">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8d811-177">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="8d811-178">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="8d811-178">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="8d811-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-179">Boolean</span></span>|<span data-ttu-id="8d811-180">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8d811-180">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="8d811-181">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="8d811-181">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="8d811-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-182">Boolean</span></span>|<span data-ttu-id="8d811-183">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8d811-183">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="8d811-184">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="8d811-184">browserBlockJavaScript</span></span>|<span data-ttu-id="8d811-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-185">Boolean</span></span>|<span data-ttu-id="8d811-186">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="8d811-186">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="8d811-187">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="8d811-187">browserBlockPlugins</span></span>|<span data-ttu-id="8d811-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-188">Boolean</span></span>|<span data-ttu-id="8d811-189">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="8d811-189">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="8d811-190">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="8d811-190">browserBlockPopups</span></span>|<span data-ttu-id="8d811-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-191">Boolean</span></span>|<span data-ttu-id="8d811-192">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="8d811-192">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="8d811-193">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="8d811-193">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="8d811-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-194">Boolean</span></span>|<span data-ttu-id="8d811-195">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="8d811-195">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="8d811-196">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="8d811-196">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="8d811-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-197">Boolean</span></span>|<span data-ttu-id="8d811-198">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8d811-198">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="8d811-199">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="8d811-199">browserRequireSmartScreen</span></span>|<span data-ttu-id="8d811-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-200">Boolean</span></span>|<span data-ttu-id="8d811-201">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="8d811-201">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="8d811-202">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="8d811-202">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="8d811-203">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d811-203">String</span></span>|<span data-ttu-id="8d811-204">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="8d811-204">The enterprise mode site list location.</span></span> <span data-ttu-id="8d811-205">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="8d811-205">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="8d811-206">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8d811-206">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="8d811-207">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8d811-207">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="8d811-208">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="8d811-208">The internet security level.</span></span> <span data-ttu-id="8d811-209">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8d811-209">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="8d811-210">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8d811-210">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="8d811-211">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8d811-211">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="8d811-212">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="8d811-212">The Intranet security level.</span></span> <span data-ttu-id="8d811-213">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8d811-213">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="8d811-214">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="8d811-214">browserLoggingReportLocation</span></span>|<span data-ttu-id="8d811-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d811-215">String</span></span>|<span data-ttu-id="8d811-216">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="8d811-216">The logging report location.</span></span>|
|<span data-ttu-id="8d811-217">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="8d811-217">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="8d811-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-218">Boolean</span></span>|<span data-ttu-id="8d811-219">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="8d811-219">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="8d811-220">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="8d811-220">browserRequireFirewall</span></span>|<span data-ttu-id="8d811-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-221">Boolean</span></span>|<span data-ttu-id="8d811-222">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="8d811-222">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="8d811-223">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="8d811-223">browserRequireFraudWarning</span></span>|<span data-ttu-id="8d811-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-224">Boolean</span></span>|<span data-ttu-id="8d811-225">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="8d811-225">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="8d811-226">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8d811-226">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="8d811-227">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8d811-227">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="8d811-228">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="8d811-228">The trusted sites security level.</span></span> <span data-ttu-id="8d811-229">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="8d811-229">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="8d811-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="8d811-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="8d811-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-231">Boolean</span></span>|<span data-ttu-id="8d811-232">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8d811-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="8d811-233">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="8d811-233">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="8d811-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-234">Boolean</span></span>|<span data-ttu-id="8d811-235">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8d811-235">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="8d811-236">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="8d811-236">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="8d811-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-237">Boolean</span></span>|<span data-ttu-id="8d811-238">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="8d811-238">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="8d811-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8d811-239">passwordExpirationDays</span></span>|<span data-ttu-id="8d811-240">Int32</span><span class="sxs-lookup"><span data-stu-id="8d811-240">Int32</span></span>|<span data-ttu-id="8d811-241">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="8d811-241">Password expiration in days.</span></span>|
|<span data-ttu-id="8d811-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8d811-242">passwordMinimumLength</span></span>|<span data-ttu-id="8d811-243">Int32</span><span class="sxs-lookup"><span data-stu-id="8d811-243">Int32</span></span>|<span data-ttu-id="8d811-244">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="8d811-244">The minimum password length.</span></span>|
|<span data-ttu-id="8d811-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8d811-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8d811-246">Int32</span><span class="sxs-lookup"><span data-stu-id="8d811-246">Int32</span></span>|<span data-ttu-id="8d811-247">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="8d811-247">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8d811-248">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8d811-248">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8d811-249">Int32</span><span class="sxs-lookup"><span data-stu-id="8d811-249">Int32</span></span>|<span data-ttu-id="8d811-250">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="8d811-250">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8d811-251">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8d811-251">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8d811-252">Int32</span><span class="sxs-lookup"><span data-stu-id="8d811-252">Int32</span></span>|<span data-ttu-id="8d811-253">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="8d811-253">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="8d811-254">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="8d811-254">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8d811-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8d811-255">passwordRequiredType</span></span>|[<span data-ttu-id="8d811-256">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8d811-256">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8d811-257">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="8d811-257">The required password type.</span></span> <span data-ttu-id="8d811-258">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="8d811-258">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8d811-259">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8d811-259">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8d811-260">Int32</span><span class="sxs-lookup"><span data-stu-id="8d811-260">Int32</span></span>|<span data-ttu-id="8d811-261">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="8d811-261">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="8d811-262">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="8d811-262">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="8d811-263">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-263">Boolean</span></span>|<span data-ttu-id="8d811-264">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="8d811-264">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="8d811-265">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="8d811-265">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="8d811-266">updateClassification</span><span class="sxs-lookup"><span data-stu-id="8d811-266">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="8d811-267">O mínimo de classificação para instalar automaticamente de atualização.</span><span class="sxs-lookup"><span data-stu-id="8d811-267">The minimum update classification to install automatically.</span></span> <span data-ttu-id="8d811-268">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="8d811-268">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="8d811-269">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="8d811-269">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="8d811-270">updateClassification</span><span class="sxs-lookup"><span data-stu-id="8d811-270">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="8d811-271">O mínimo de classificação para instalar automaticamente de atualização.</span><span class="sxs-lookup"><span data-stu-id="8d811-271">The minimum update classification to install automatically.</span></span> <span data-ttu-id="8d811-272">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="8d811-272">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="8d811-273">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="8d811-273">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="8d811-274">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d811-274">Boolean</span></span>|<span data-ttu-id="8d811-275">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="8d811-275">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="8d811-276">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="8d811-276">userAccountControlSettings</span></span>|[<span data-ttu-id="8d811-277">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="8d811-277">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="8d811-278">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="8d811-278">The user account control settings.</span></span> <span data-ttu-id="8d811-279">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="8d811-279">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="8d811-280">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="8d811-280">workFoldersUrl</span></span>|<span data-ttu-id="8d811-281">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d811-281">String</span></span>|<span data-ttu-id="8d811-282">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="8d811-282">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="8d811-283">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d811-283">Response</span></span>
<span data-ttu-id="8d811-284">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d811-284">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d811-285">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d811-285">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d811-286">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d811-286">Request</span></span>
<span data-ttu-id="8d811-287">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d811-287">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="8d811-288">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d811-288">Response</span></span>
<span data-ttu-id="8d811-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d811-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





