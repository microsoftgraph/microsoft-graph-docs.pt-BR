---
title: Criar windows81GeneralConfiguration
description: Criar um novo objeto windows81GeneralConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f07f477436cbff75b72fea1d080012e184a835f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409339"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="b28c4-103">Criar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="b28c4-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="b28c4-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b28c4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b28c4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b28c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b28c4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b28c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b28c4-107">Criar um novo objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b28c4-107">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b28c4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b28c4-108">Prerequisites</span></span>
<span data-ttu-id="b28c4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b28c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b28c4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b28c4-111">Permission type</span></span>|<span data-ttu-id="b28c4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b28c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b28c4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b28c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b28c4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b28c4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b28c4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b28c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b28c4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b28c4-116">Not supported.</span></span>|
|<span data-ttu-id="b28c4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b28c4-117">Application</span></span>|<span data-ttu-id="b28c4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b28c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b28c4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b28c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b28c4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b28c4-120">Request headers</span></span>
|<span data-ttu-id="b28c4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b28c4-121">Header</span></span>|<span data-ttu-id="b28c4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b28c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b28c4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b28c4-123">Authorization</span></span>|<span data-ttu-id="b28c4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b28c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b28c4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b28c4-125">Accept</span></span>|<span data-ttu-id="b28c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b28c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b28c4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b28c4-127">Request body</span></span>
<span data-ttu-id="b28c4-128">No corpo da solicitação, forneça uma representação JSON do objeto windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b28c4-128">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="b28c4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b28c4-129">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="b28c4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b28c4-130">Property</span></span>|<span data-ttu-id="b28c4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b28c4-131">Type</span></span>|<span data-ttu-id="b28c4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b28c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b28c4-133">id</span><span class="sxs-lookup"><span data-stu-id="b28c4-133">id</span></span>|<span data-ttu-id="b28c4-134">String</span><span class="sxs-lookup"><span data-stu-id="b28c4-134">String</span></span>|<span data-ttu-id="b28c4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b28c4-135">Key of the entity.</span></span> <span data-ttu-id="b28c4-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b28c4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b28c4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b28c4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b28c4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28c4-138">DateTimeOffset</span></span>|<span data-ttu-id="b28c4-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b28c4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b28c4-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b28c4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b28c4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b28c4-141">roleScopeTagIds</span></span>|<span data-ttu-id="b28c4-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b28c4-142">String collection</span></span>|<span data-ttu-id="b28c4-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="b28c4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b28c4-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b28c4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b28c4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b28c4-145">supportsScopeTags</span></span>|<span data-ttu-id="b28c4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-146">Boolean</span></span>|<span data-ttu-id="b28c4-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b28c4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b28c4-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b28c4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b28c4-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="b28c4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b28c4-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c4-150">This property is read-only.</span></span> <span data-ttu-id="b28c4-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b28c4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b28c4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b28c4-152">createdDateTime</span></span>|<span data-ttu-id="b28c4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b28c4-153">DateTimeOffset</span></span>|<span data-ttu-id="b28c4-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b28c4-154">DateTime the object was created.</span></span> <span data-ttu-id="b28c4-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b28c4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b28c4-156">description</span><span class="sxs-lookup"><span data-stu-id="b28c4-156">description</span></span>|<span data-ttu-id="b28c4-157">String</span><span class="sxs-lookup"><span data-stu-id="b28c4-157">String</span></span>|<span data-ttu-id="b28c4-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b28c4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b28c4-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b28c4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b28c4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b28c4-160">displayName</span></span>|<span data-ttu-id="b28c4-161">String</span><span class="sxs-lookup"><span data-stu-id="b28c4-161">String</span></span>|<span data-ttu-id="b28c4-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b28c4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b28c4-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b28c4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b28c4-164">version</span><span class="sxs-lookup"><span data-stu-id="b28c4-164">version</span></span>|<span data-ttu-id="b28c4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b28c4-165">Int32</span></span>|<span data-ttu-id="b28c4-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b28c4-166">Version of the device configuration.</span></span> <span data-ttu-id="b28c4-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b28c4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b28c4-168">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="b28c4-168">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="b28c4-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-169">Boolean</span></span>|<span data-ttu-id="b28c4-170">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b28c4-170">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="b28c4-171">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="b28c4-171">applyOnlyToWindows81</span></span>|<span data-ttu-id="b28c4-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-172">Boolean</span></span>|<span data-ttu-id="b28c4-173">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="b28c4-173">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="b28c4-174">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b28c4-174">This property is read-only.</span></span>|
|<span data-ttu-id="b28c4-175">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b28c4-175">browserBlockAutofill</span></span>|<span data-ttu-id="b28c4-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-176">Boolean</span></span>|<span data-ttu-id="b28c4-177">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b28c4-177">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="b28c4-178">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="b28c4-178">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="b28c4-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-179">Boolean</span></span>|<span data-ttu-id="b28c4-180">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b28c4-180">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="b28c4-181">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="b28c4-181">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="b28c4-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-182">Boolean</span></span>|<span data-ttu-id="b28c4-183">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b28c4-183">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="b28c4-184">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b28c4-184">browserBlockJavaScript</span></span>|<span data-ttu-id="b28c4-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-185">Boolean</span></span>|<span data-ttu-id="b28c4-186">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="b28c4-186">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="b28c4-187">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="b28c4-187">browserBlockPlugins</span></span>|<span data-ttu-id="b28c4-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-188">Boolean</span></span>|<span data-ttu-id="b28c4-189">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="b28c4-189">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="b28c4-190">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b28c4-190">browserBlockPopups</span></span>|<span data-ttu-id="b28c4-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-191">Boolean</span></span>|<span data-ttu-id="b28c4-192">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="b28c4-192">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="b28c4-193">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="b28c4-193">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="b28c4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-194">Boolean</span></span>|<span data-ttu-id="b28c4-195">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="b28c4-195">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="b28c4-196">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="b28c4-196">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="b28c4-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-197">Boolean</span></span>|<span data-ttu-id="b28c4-198">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b28c4-198">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="b28c4-199">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="b28c4-199">browserRequireSmartScreen</span></span>|<span data-ttu-id="b28c4-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-200">Boolean</span></span>|<span data-ttu-id="b28c4-201">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="b28c4-201">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="b28c4-202">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="b28c4-202">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="b28c4-203">String</span><span class="sxs-lookup"><span data-stu-id="b28c4-203">String</span></span>|<span data-ttu-id="b28c4-204">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="b28c4-204">The enterprise mode site list location.</span></span> <span data-ttu-id="b28c4-205">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="b28c4-205">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="b28c4-206">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b28c4-206">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="b28c4-207">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b28c4-207">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="b28c4-208">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="b28c4-208">The internet security level.</span></span> <span data-ttu-id="b28c4-209">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b28c4-209">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="b28c4-210">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b28c4-210">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="b28c4-211">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b28c4-211">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="b28c4-212">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="b28c4-212">The Intranet security level.</span></span> <span data-ttu-id="b28c4-213">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b28c4-213">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="b28c4-214">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="b28c4-214">browserLoggingReportLocation</span></span>|<span data-ttu-id="b28c4-215">String</span><span class="sxs-lookup"><span data-stu-id="b28c4-215">String</span></span>|<span data-ttu-id="b28c4-216">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="b28c4-216">The logging report location.</span></span>|
|<span data-ttu-id="b28c4-217">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="b28c4-217">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="b28c4-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-218">Boolean</span></span>|<span data-ttu-id="b28c4-219">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="b28c4-219">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="b28c4-220">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="b28c4-220">browserRequireFirewall</span></span>|<span data-ttu-id="b28c4-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-221">Boolean</span></span>|<span data-ttu-id="b28c4-222">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="b28c4-222">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="b28c4-223">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="b28c4-223">browserRequireFraudWarning</span></span>|<span data-ttu-id="b28c4-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-224">Boolean</span></span>|<span data-ttu-id="b28c4-225">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="b28c4-225">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="b28c4-226">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b28c4-226">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="b28c4-227">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b28c4-227">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="b28c4-228">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="b28c4-228">The trusted sites security level.</span></span> <span data-ttu-id="b28c4-229">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b28c4-229">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="b28c4-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="b28c4-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="b28c4-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-231">Boolean</span></span>|<span data-ttu-id="b28c4-232">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b28c4-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="b28c4-233">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="b28c4-233">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="b28c4-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-234">Boolean</span></span>|<span data-ttu-id="b28c4-235">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b28c4-235">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b28c4-236">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="b28c4-236">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="b28c4-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-237">Boolean</span></span>|<span data-ttu-id="b28c4-238">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="b28c4-238">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="b28c4-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b28c4-239">passwordExpirationDays</span></span>|<span data-ttu-id="b28c4-240">Int32</span><span class="sxs-lookup"><span data-stu-id="b28c4-240">Int32</span></span>|<span data-ttu-id="b28c4-241">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="b28c4-241">Password expiration in days.</span></span>|
|<span data-ttu-id="b28c4-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b28c4-242">passwordMinimumLength</span></span>|<span data-ttu-id="b28c4-243">Int32</span><span class="sxs-lookup"><span data-stu-id="b28c4-243">Int32</span></span>|<span data-ttu-id="b28c4-244">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="b28c4-244">The minimum password length.</span></span>|
|<span data-ttu-id="b28c4-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b28c4-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b28c4-246">Int32</span><span class="sxs-lookup"><span data-stu-id="b28c4-246">Int32</span></span>|<span data-ttu-id="b28c4-247">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="b28c4-247">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b28c4-248">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b28c4-248">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b28c4-249">Int32</span><span class="sxs-lookup"><span data-stu-id="b28c4-249">Int32</span></span>|<span data-ttu-id="b28c4-250">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="b28c4-250">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b28c4-251">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b28c4-251">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b28c4-252">Int32</span><span class="sxs-lookup"><span data-stu-id="b28c4-252">Int32</span></span>|<span data-ttu-id="b28c4-253">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="b28c4-253">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="b28c4-254">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="b28c4-254">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b28c4-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b28c4-255">passwordRequiredType</span></span>|[<span data-ttu-id="b28c4-256">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b28c4-256">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b28c4-257">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="b28c4-257">The required password type.</span></span> <span data-ttu-id="b28c4-258">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b28c4-258">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b28c4-259">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b28c4-259">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b28c4-260">Int32</span><span class="sxs-lookup"><span data-stu-id="b28c4-260">Int32</span></span>|<span data-ttu-id="b28c4-261">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="b28c4-261">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="b28c4-262">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="b28c4-262">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="b28c4-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-263">Boolean</span></span>|<span data-ttu-id="b28c4-264">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="b28c4-264">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="b28c4-265">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="b28c4-265">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="b28c4-266">updateClassification</span><span class="sxs-lookup"><span data-stu-id="b28c4-266">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="b28c4-267">O mínimo de classificação para instalar automaticamente de atualização.</span><span class="sxs-lookup"><span data-stu-id="b28c4-267">The minimum update classification to install automatically.</span></span> <span data-ttu-id="b28c4-268">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="b28c4-268">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="b28c4-269">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="b28c4-269">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="b28c4-270">updateClassification</span><span class="sxs-lookup"><span data-stu-id="b28c4-270">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="b28c4-271">O mínimo de classificação para instalar automaticamente de atualização.</span><span class="sxs-lookup"><span data-stu-id="b28c4-271">The minimum update classification to install automatically.</span></span> <span data-ttu-id="b28c4-272">Os valores possíveis são: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="b28c4-272">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="b28c4-273">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="b28c4-273">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="b28c4-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="b28c4-274">Boolean</span></span>|<span data-ttu-id="b28c4-275">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="b28c4-275">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="b28c4-276">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="b28c4-276">userAccountControlSettings</span></span>|[<span data-ttu-id="b28c4-277">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="b28c4-277">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="b28c4-278">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="b28c4-278">The user account control settings.</span></span> <span data-ttu-id="b28c4-279">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="b28c4-279">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="b28c4-280">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="b28c4-280">workFoldersUrl</span></span>|<span data-ttu-id="b28c4-281">String</span><span class="sxs-lookup"><span data-stu-id="b28c4-281">String</span></span>|<span data-ttu-id="b28c4-282">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="b28c4-282">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="b28c4-283">Resposta</span><span class="sxs-lookup"><span data-stu-id="b28c4-283">Response</span></span>
<span data-ttu-id="b28c4-284">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b28c4-284">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b28c4-285">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b28c4-285">Example</span></span>

### <a name="request"></a><span data-ttu-id="b28c4-286">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b28c4-286">Request</span></span>
<span data-ttu-id="b28c4-287">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b28c4-287">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b28c4-288">Resposta</span><span class="sxs-lookup"><span data-stu-id="b28c4-288">Response</span></span>
<span data-ttu-id="b28c4-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b28c4-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




