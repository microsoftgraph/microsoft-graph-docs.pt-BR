---
title: Criar windows81GeneralConfiguration
description: Criar um novo objeto windows81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2af1c27ac1097f7571aea1782cdd0dc4c99c2bb7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753808"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="ab541-103">Criar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab541-103">Create windows81GeneralConfiguration</span></span>

<span data-ttu-id="ab541-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab541-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab541-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ab541-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab541-106">Criar um novo objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab541-106">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab541-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ab541-107">Prerequisites</span></span>
<span data-ttu-id="ab541-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab541-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab541-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab541-110">Permission type</span></span>|<span data-ttu-id="ab541-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab541-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab541-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab541-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab541-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab541-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ab541-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab541-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab541-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab541-115">Not supported.</span></span>|
|<span data-ttu-id="ab541-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab541-116">Application</span></span>|<span data-ttu-id="ab541-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab541-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab541-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab541-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ab541-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab541-119">Request headers</span></span>
|<span data-ttu-id="ab541-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab541-120">Header</span></span>|<span data-ttu-id="ab541-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ab541-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab541-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab541-122">Authorization</span></span>|<span data-ttu-id="ab541-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab541-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab541-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ab541-124">Accept</span></span>|<span data-ttu-id="ab541-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ab541-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab541-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab541-126">Request body</span></span>
<span data-ttu-id="ab541-127">No corpo da solicitação, forneça uma representação JSON do objeto windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ab541-127">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="ab541-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ab541-128">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="ab541-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab541-129">Property</span></span>|<span data-ttu-id="ab541-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab541-130">Type</span></span>|<span data-ttu-id="ab541-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab541-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab541-132">id</span><span class="sxs-lookup"><span data-stu-id="ab541-132">id</span></span>|<span data-ttu-id="ab541-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab541-133">String</span></span>|<span data-ttu-id="ab541-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ab541-134">Key of the entity.</span></span> <span data-ttu-id="ab541-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab541-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab541-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab541-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ab541-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab541-137">DateTimeOffset</span></span>|<span data-ttu-id="ab541-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ab541-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ab541-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab541-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab541-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab541-140">createdDateTime</span></span>|<span data-ttu-id="ab541-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab541-141">DateTimeOffset</span></span>|<span data-ttu-id="ab541-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ab541-142">DateTime the object was created.</span></span> <span data-ttu-id="ab541-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab541-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab541-144">descrição</span><span class="sxs-lookup"><span data-stu-id="ab541-144">description</span></span>|<span data-ttu-id="ab541-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab541-145">String</span></span>|<span data-ttu-id="ab541-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab541-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ab541-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab541-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab541-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ab541-148">displayName</span></span>|<span data-ttu-id="ab541-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ab541-149">String</span></span>|<span data-ttu-id="ab541-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab541-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ab541-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab541-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab541-152">versão</span><span class="sxs-lookup"><span data-stu-id="ab541-152">version</span></span>|<span data-ttu-id="ab541-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-153">Int32</span></span>|<span data-ttu-id="ab541-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab541-154">Version of the device configuration.</span></span> <span data-ttu-id="ab541-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab541-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab541-156">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="ab541-156">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="ab541-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-157">Boolean</span></span>|<span data-ttu-id="ab541-158">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ab541-158">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="ab541-159">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="ab541-159">applyOnlyToWindows81</span></span>|<span data-ttu-id="ab541-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-160">Boolean</span></span>|<span data-ttu-id="ab541-161">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="ab541-161">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="ab541-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab541-162">This property is read-only.</span></span>|
|<span data-ttu-id="ab541-163">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ab541-163">browserBlockAutofill</span></span>|<span data-ttu-id="ab541-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-164">Boolean</span></span>|<span data-ttu-id="ab541-165">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ab541-165">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="ab541-166">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="ab541-166">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="ab541-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-167">Boolean</span></span>|<span data-ttu-id="ab541-168">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ab541-168">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="ab541-169">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="ab541-169">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="ab541-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-170">Boolean</span></span>|<span data-ttu-id="ab541-171">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ab541-171">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="ab541-172">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="ab541-172">browserBlockJavaScript</span></span>|<span data-ttu-id="ab541-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-173">Boolean</span></span>|<span data-ttu-id="ab541-174">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="ab541-174">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="ab541-175">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="ab541-175">browserBlockPlugins</span></span>|<span data-ttu-id="ab541-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-176">Boolean</span></span>|<span data-ttu-id="ab541-177">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="ab541-177">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="ab541-178">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="ab541-178">browserBlockPopups</span></span>|<span data-ttu-id="ab541-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-179">Boolean</span></span>|<span data-ttu-id="ab541-180">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="ab541-180">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="ab541-181">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="ab541-181">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="ab541-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-182">Boolean</span></span>|<span data-ttu-id="ab541-183">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="ab541-183">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="ab541-184">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="ab541-184">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="ab541-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-185">Boolean</span></span>|<span data-ttu-id="ab541-186">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ab541-186">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="ab541-187">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="ab541-187">browserRequireSmartScreen</span></span>|<span data-ttu-id="ab541-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-188">Boolean</span></span>|<span data-ttu-id="ab541-189">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="ab541-189">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="ab541-190">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="ab541-190">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="ab541-191">String</span><span class="sxs-lookup"><span data-stu-id="ab541-191">String</span></span>|<span data-ttu-id="ab541-192">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="ab541-192">The enterprise mode site list location.</span></span> <span data-ttu-id="ab541-193">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="ab541-193">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="ab541-194">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ab541-194">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="ab541-195">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ab541-195">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="ab541-196">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="ab541-196">The internet security level.</span></span> <span data-ttu-id="ab541-197">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ab541-197">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="ab541-198">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ab541-198">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="ab541-199">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ab541-199">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="ab541-200">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="ab541-200">The Intranet security level.</span></span> <span data-ttu-id="ab541-201">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ab541-201">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="ab541-202">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="ab541-202">browserLoggingReportLocation</span></span>|<span data-ttu-id="ab541-203">String</span><span class="sxs-lookup"><span data-stu-id="ab541-203">String</span></span>|<span data-ttu-id="ab541-204">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="ab541-204">The logging report location.</span></span>|
|<span data-ttu-id="ab541-205">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="ab541-205">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="ab541-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-206">Boolean</span></span>|<span data-ttu-id="ab541-207">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="ab541-207">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="ab541-208">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="ab541-208">browserRequireFirewall</span></span>|<span data-ttu-id="ab541-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-209">Boolean</span></span>|<span data-ttu-id="ab541-210">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="ab541-210">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="ab541-211">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="ab541-211">browserRequireFraudWarning</span></span>|<span data-ttu-id="ab541-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-212">Boolean</span></span>|<span data-ttu-id="ab541-213">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="ab541-213">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="ab541-214">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ab541-214">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="ab541-215">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="ab541-215">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="ab541-216">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="ab541-216">The trusted sites security level.</span></span> <span data-ttu-id="ab541-217">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="ab541-217">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="ab541-218">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="ab541-218">cellularBlockDataRoaming</span></span>|<span data-ttu-id="ab541-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-219">Boolean</span></span>|<span data-ttu-id="ab541-220">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ab541-220">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="ab541-221">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="ab541-221">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="ab541-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-222">Boolean</span></span>|<span data-ttu-id="ab541-223">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ab541-223">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="ab541-224">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="ab541-224">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="ab541-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-225">Boolean</span></span>|<span data-ttu-id="ab541-226">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="ab541-226">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="ab541-227">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ab541-227">passwordExpirationDays</span></span>|<span data-ttu-id="ab541-228">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-228">Int32</span></span>|<span data-ttu-id="ab541-229">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="ab541-229">Password expiration in days.</span></span>|
|<span data-ttu-id="ab541-230">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ab541-230">passwordMinimumLength</span></span>|<span data-ttu-id="ab541-231">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-231">Int32</span></span>|<span data-ttu-id="ab541-232">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="ab541-232">The minimum password length.</span></span>|
|<span data-ttu-id="ab541-233">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ab541-233">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ab541-234">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-234">Int32</span></span>|<span data-ttu-id="ab541-235">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="ab541-235">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ab541-236">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ab541-236">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="ab541-237">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-237">Int32</span></span>|<span data-ttu-id="ab541-238">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="ab541-238">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="ab541-239">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ab541-239">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ab541-240">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-240">Int32</span></span>|<span data-ttu-id="ab541-241">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="ab541-241">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="ab541-242">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="ab541-242">Valid values 0 to 24</span></span>|
|<span data-ttu-id="ab541-243">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="ab541-243">passwordRequiredType</span></span>|[<span data-ttu-id="ab541-244">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ab541-244">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ab541-245">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="ab541-245">The required password type.</span></span> <span data-ttu-id="ab541-246">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ab541-246">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ab541-247">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="ab541-247">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="ab541-248">Int32</span><span class="sxs-lookup"><span data-stu-id="ab541-248">Int32</span></span>|<span data-ttu-id="ab541-249">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="ab541-249">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="ab541-250">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="ab541-250">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="ab541-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-251">Boolean</span></span>|<span data-ttu-id="ab541-252">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="ab541-252">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="ab541-253">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="ab541-253">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="ab541-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab541-254">Boolean</span></span>|<span data-ttu-id="ab541-255">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="ab541-255">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="ab541-256">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="ab541-256">userAccountControlSettings</span></span>|[<span data-ttu-id="ab541-257">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="ab541-257">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="ab541-258">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="ab541-258">The user account control settings.</span></span> <span data-ttu-id="ab541-259">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="ab541-259">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="ab541-260">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="ab541-260">workFoldersUrl</span></span>|<span data-ttu-id="ab541-261">String</span><span class="sxs-lookup"><span data-stu-id="ab541-261">String</span></span>|<span data-ttu-id="ab541-262">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="ab541-262">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="ab541-263">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab541-263">Response</span></span>
<span data-ttu-id="ab541-264">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab541-264">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab541-265">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab541-265">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab541-266">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab541-266">Request</span></span>
<span data-ttu-id="ab541-267">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab541-267">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="ab541-268">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab541-268">Response</span></span>
<span data-ttu-id="ab541-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab541-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




