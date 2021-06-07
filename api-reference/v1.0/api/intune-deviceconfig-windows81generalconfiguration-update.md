---
title: Atualizar windows81GeneralConfiguration
description: Atualizar as propriedades de um objeto windows81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 658ffad0fcbd900731ca19390705aa0f235eecf2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52747232"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="743b8-103">Atualizar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="743b8-103">Update windows81GeneralConfiguration</span></span>

<span data-ttu-id="743b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="743b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="743b8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="743b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="743b8-106">Atualizar as propriedades de um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="743b8-106">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="743b8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="743b8-107">Prerequisites</span></span>
<span data-ttu-id="743b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="743b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="743b8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="743b8-110">Permission type</span></span>|<span data-ttu-id="743b8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="743b8-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="743b8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="743b8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="743b8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="743b8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="743b8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="743b8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="743b8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="743b8-115">Not supported.</span></span>|
|<span data-ttu-id="743b8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="743b8-116">Application</span></span>|<span data-ttu-id="743b8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="743b8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="743b8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="743b8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="743b8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="743b8-119">Request headers</span></span>
|<span data-ttu-id="743b8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="743b8-120">Header</span></span>|<span data-ttu-id="743b8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="743b8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="743b8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="743b8-122">Authorization</span></span>|<span data-ttu-id="743b8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="743b8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="743b8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="743b8-124">Accept</span></span>|<span data-ttu-id="743b8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="743b8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="743b8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="743b8-126">Request body</span></span>
<span data-ttu-id="743b8-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="743b8-127">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="743b8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="743b8-128">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="743b8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="743b8-129">Property</span></span>|<span data-ttu-id="743b8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="743b8-130">Type</span></span>|<span data-ttu-id="743b8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="743b8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="743b8-132">id</span><span class="sxs-lookup"><span data-stu-id="743b8-132">id</span></span>|<span data-ttu-id="743b8-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="743b8-133">String</span></span>|<span data-ttu-id="743b8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="743b8-134">Key of the entity.</span></span> <span data-ttu-id="743b8-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="743b8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="743b8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="743b8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="743b8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="743b8-137">DateTimeOffset</span></span>|<span data-ttu-id="743b8-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="743b8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="743b8-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="743b8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="743b8-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="743b8-140">createdDateTime</span></span>|<span data-ttu-id="743b8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="743b8-141">DateTimeOffset</span></span>|<span data-ttu-id="743b8-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="743b8-142">DateTime the object was created.</span></span> <span data-ttu-id="743b8-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="743b8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="743b8-144">descrição</span><span class="sxs-lookup"><span data-stu-id="743b8-144">description</span></span>|<span data-ttu-id="743b8-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="743b8-145">String</span></span>|<span data-ttu-id="743b8-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="743b8-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="743b8-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="743b8-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="743b8-148">displayName</span><span class="sxs-lookup"><span data-stu-id="743b8-148">displayName</span></span>|<span data-ttu-id="743b8-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="743b8-149">String</span></span>|<span data-ttu-id="743b8-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="743b8-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="743b8-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="743b8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="743b8-152">versão</span><span class="sxs-lookup"><span data-stu-id="743b8-152">version</span></span>|<span data-ttu-id="743b8-153">Int32</span><span class="sxs-lookup"><span data-stu-id="743b8-153">Int32</span></span>|<span data-ttu-id="743b8-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="743b8-154">Version of the device configuration.</span></span> <span data-ttu-id="743b8-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="743b8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="743b8-156">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="743b8-156">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="743b8-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-157">Boolean</span></span>|<span data-ttu-id="743b8-158">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="743b8-158">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="743b8-159">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="743b8-159">applyOnlyToWindows81</span></span>|<span data-ttu-id="743b8-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-160">Boolean</span></span>|<span data-ttu-id="743b8-161">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="743b8-161">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="743b8-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="743b8-162">This property is read-only.</span></span>|
|<span data-ttu-id="743b8-163">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="743b8-163">browserBlockAutofill</span></span>|<span data-ttu-id="743b8-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-164">Boolean</span></span>|<span data-ttu-id="743b8-165">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="743b8-165">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="743b8-166">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="743b8-166">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="743b8-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-167">Boolean</span></span>|<span data-ttu-id="743b8-168">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="743b8-168">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="743b8-169">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="743b8-169">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="743b8-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-170">Boolean</span></span>|<span data-ttu-id="743b8-171">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="743b8-171">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="743b8-172">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="743b8-172">browserBlockJavaScript</span></span>|<span data-ttu-id="743b8-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-173">Boolean</span></span>|<span data-ttu-id="743b8-174">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="743b8-174">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="743b8-175">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="743b8-175">browserBlockPlugins</span></span>|<span data-ttu-id="743b8-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-176">Boolean</span></span>|<span data-ttu-id="743b8-177">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="743b8-177">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="743b8-178">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="743b8-178">browserBlockPopups</span></span>|<span data-ttu-id="743b8-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-179">Boolean</span></span>|<span data-ttu-id="743b8-180">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="743b8-180">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="743b8-181">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="743b8-181">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="743b8-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-182">Boolean</span></span>|<span data-ttu-id="743b8-183">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="743b8-183">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="743b8-184">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="743b8-184">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="743b8-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-185">Boolean</span></span>|<span data-ttu-id="743b8-186">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="743b8-186">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="743b8-187">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="743b8-187">browserRequireSmartScreen</span></span>|<span data-ttu-id="743b8-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-188">Boolean</span></span>|<span data-ttu-id="743b8-189">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="743b8-189">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="743b8-190">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="743b8-190">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="743b8-191">String</span><span class="sxs-lookup"><span data-stu-id="743b8-191">String</span></span>|<span data-ttu-id="743b8-192">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="743b8-192">The enterprise mode site list location.</span></span> <span data-ttu-id="743b8-193">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="743b8-193">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="743b8-194">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="743b8-194">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="743b8-195">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="743b8-195">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="743b8-196">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="743b8-196">The internet security level.</span></span> <span data-ttu-id="743b8-197">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="743b8-197">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="743b8-198">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="743b8-198">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="743b8-199">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="743b8-199">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="743b8-200">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="743b8-200">The Intranet security level.</span></span> <span data-ttu-id="743b8-201">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="743b8-201">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="743b8-202">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="743b8-202">browserLoggingReportLocation</span></span>|<span data-ttu-id="743b8-203">String</span><span class="sxs-lookup"><span data-stu-id="743b8-203">String</span></span>|<span data-ttu-id="743b8-204">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="743b8-204">The logging report location.</span></span>|
|<span data-ttu-id="743b8-205">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="743b8-205">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="743b8-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-206">Boolean</span></span>|<span data-ttu-id="743b8-207">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="743b8-207">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="743b8-208">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="743b8-208">browserRequireFirewall</span></span>|<span data-ttu-id="743b8-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-209">Boolean</span></span>|<span data-ttu-id="743b8-210">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="743b8-210">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="743b8-211">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="743b8-211">browserRequireFraudWarning</span></span>|<span data-ttu-id="743b8-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-212">Boolean</span></span>|<span data-ttu-id="743b8-213">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="743b8-213">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="743b8-214">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="743b8-214">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="743b8-215">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="743b8-215">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="743b8-216">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="743b8-216">The trusted sites security level.</span></span> <span data-ttu-id="743b8-217">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="743b8-217">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="743b8-218">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="743b8-218">cellularBlockDataRoaming</span></span>|<span data-ttu-id="743b8-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-219">Boolean</span></span>|<span data-ttu-id="743b8-220">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="743b8-220">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="743b8-221">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="743b8-221">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="743b8-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-222">Boolean</span></span>|<span data-ttu-id="743b8-223">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="743b8-223">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="743b8-224">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="743b8-224">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="743b8-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-225">Boolean</span></span>|<span data-ttu-id="743b8-226">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="743b8-226">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="743b8-227">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="743b8-227">passwordExpirationDays</span></span>|<span data-ttu-id="743b8-228">Int32</span><span class="sxs-lookup"><span data-stu-id="743b8-228">Int32</span></span>|<span data-ttu-id="743b8-229">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="743b8-229">Password expiration in days.</span></span>|
|<span data-ttu-id="743b8-230">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="743b8-230">passwordMinimumLength</span></span>|<span data-ttu-id="743b8-231">Int32</span><span class="sxs-lookup"><span data-stu-id="743b8-231">Int32</span></span>|<span data-ttu-id="743b8-232">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="743b8-232">The minimum password length.</span></span>|
|<span data-ttu-id="743b8-233">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="743b8-233">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="743b8-234">Int32</span><span class="sxs-lookup"><span data-stu-id="743b8-234">Int32</span></span>|<span data-ttu-id="743b8-235">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="743b8-235">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="743b8-236">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="743b8-236">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="743b8-237">Int32</span><span class="sxs-lookup"><span data-stu-id="743b8-237">Int32</span></span>|<span data-ttu-id="743b8-238">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="743b8-238">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="743b8-239">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="743b8-239">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="743b8-240">Int32</span><span class="sxs-lookup"><span data-stu-id="743b8-240">Int32</span></span>|<span data-ttu-id="743b8-241">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="743b8-241">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="743b8-242">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="743b8-242">Valid values 0 to 24</span></span>|
|<span data-ttu-id="743b8-243">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="743b8-243">passwordRequiredType</span></span>|[<span data-ttu-id="743b8-244">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="743b8-244">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="743b8-245">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="743b8-245">The required password type.</span></span> <span data-ttu-id="743b8-246">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="743b8-246">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="743b8-247">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="743b8-247">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="743b8-248">Int32</span><span class="sxs-lookup"><span data-stu-id="743b8-248">Int32</span></span>|<span data-ttu-id="743b8-249">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="743b8-249">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="743b8-250">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="743b8-250">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="743b8-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-251">Boolean</span></span>|<span data-ttu-id="743b8-252">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="743b8-252">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="743b8-253">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="743b8-253">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="743b8-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="743b8-254">Boolean</span></span>|<span data-ttu-id="743b8-255">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="743b8-255">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="743b8-256">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="743b8-256">userAccountControlSettings</span></span>|[<span data-ttu-id="743b8-257">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="743b8-257">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="743b8-258">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="743b8-258">The user account control settings.</span></span> <span data-ttu-id="743b8-259">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="743b8-259">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="743b8-260">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="743b8-260">workFoldersUrl</span></span>|<span data-ttu-id="743b8-261">String</span><span class="sxs-lookup"><span data-stu-id="743b8-261">String</span></span>|<span data-ttu-id="743b8-262">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="743b8-262">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="743b8-263">Resposta</span><span class="sxs-lookup"><span data-stu-id="743b8-263">Response</span></span>
<span data-ttu-id="743b8-264">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="743b8-264">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="743b8-265">Exemplo</span><span class="sxs-lookup"><span data-stu-id="743b8-265">Example</span></span>

### <a name="request"></a><span data-ttu-id="743b8-266">Solicitação</span><span class="sxs-lookup"><span data-stu-id="743b8-266">Request</span></span>
<span data-ttu-id="743b8-267">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="743b8-267">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1693

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
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
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="743b8-268">Resposta</span><span class="sxs-lookup"><span data-stu-id="743b8-268">Response</span></span>
<span data-ttu-id="743b8-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="743b8-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```




