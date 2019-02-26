---
title: Atualizar windows81GeneralConfiguration
description: Atualizar as propriedades de um objeto windows81GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 21de1e83d2153bfebdb6e3099a91dde5c7cca1b2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252823"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="b065b-103">Atualizar windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="b065b-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="b065b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b065b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b065b-105">Atualizar as propriedades de um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b065b-105">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b065b-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b065b-106">Prerequisites</span></span>
<span data-ttu-id="b065b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b065b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b065b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b065b-109">Permission type</span></span>|<span data-ttu-id="b065b-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b065b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b065b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b065b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b065b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b065b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b065b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b065b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b065b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b065b-114">Not supported.</span></span>|
|<span data-ttu-id="b065b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b065b-115">Application</span></span>|<span data-ttu-id="b065b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b065b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b065b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b065b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b065b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b065b-118">Request headers</span></span>
|<span data-ttu-id="b065b-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b065b-119">Header</span></span>|<span data-ttu-id="b065b-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b065b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b065b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b065b-121">Authorization</span></span>|<span data-ttu-id="b065b-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b065b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b065b-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b065b-123">Accept</span></span>|<span data-ttu-id="b065b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b065b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b065b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b065b-125">Request body</span></span>
<span data-ttu-id="b065b-126">No corpo da solicitação, forneça uma representação JSON do objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b065b-126">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="b065b-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b065b-127">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="b065b-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b065b-128">Property</span></span>|<span data-ttu-id="b065b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b065b-129">Type</span></span>|<span data-ttu-id="b065b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b065b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b065b-131">id</span><span class="sxs-lookup"><span data-stu-id="b065b-131">id</span></span>|<span data-ttu-id="b065b-132">String</span><span class="sxs-lookup"><span data-stu-id="b065b-132">String</span></span>|<span data-ttu-id="b065b-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b065b-133">Key of the entity.</span></span> <span data-ttu-id="b065b-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b065b-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b065b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b065b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b065b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b065b-136">DateTimeOffset</span></span>|<span data-ttu-id="b065b-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b065b-137">DateTime the object was last modified.</span></span> <span data-ttu-id="b065b-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b065b-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b065b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b065b-139">createdDateTime</span></span>|<span data-ttu-id="b065b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b065b-140">DateTimeOffset</span></span>|<span data-ttu-id="b065b-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b065b-141">DateTime the object was created.</span></span> <span data-ttu-id="b065b-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b065b-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b065b-143">description</span><span class="sxs-lookup"><span data-stu-id="b065b-143">description</span></span>|<span data-ttu-id="b065b-144">String</span><span class="sxs-lookup"><span data-stu-id="b065b-144">String</span></span>|<span data-ttu-id="b065b-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b065b-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b065b-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b065b-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b065b-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b065b-147">displayName</span></span>|<span data-ttu-id="b065b-148">String</span><span class="sxs-lookup"><span data-stu-id="b065b-148">String</span></span>|<span data-ttu-id="b065b-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b065b-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b065b-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b065b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b065b-151">version</span><span class="sxs-lookup"><span data-stu-id="b065b-151">version</span></span>|<span data-ttu-id="b065b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b065b-152">Int32</span></span>|<span data-ttu-id="b065b-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b065b-153">Version of the device configuration.</span></span> <span data-ttu-id="b065b-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b065b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b065b-155">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="b065b-155">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="b065b-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-156">Boolean</span></span>|<span data-ttu-id="b065b-157">Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b065b-157">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="b065b-158">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="b065b-158">applyOnlyToWindows81</span></span>|<span data-ttu-id="b065b-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-159">Boolean</span></span>|<span data-ttu-id="b065b-160">Valor que indica se esta política se aplica somente ao Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="b065b-160">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="b065b-161">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b065b-161">This property is read-only.</span></span>|
|<span data-ttu-id="b065b-162">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b065b-162">browserBlockAutofill</span></span>|<span data-ttu-id="b065b-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-163">Boolean</span></span>|<span data-ttu-id="b065b-164">Indica se o preenchimento automático deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b065b-164">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="b065b-165">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="b065b-165">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="b065b-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-166">Boolean</span></span>|<span data-ttu-id="b065b-167">Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b065b-167">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="b065b-168">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="b065b-168">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="b065b-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-169">Boolean</span></span>|<span data-ttu-id="b065b-170">Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b065b-170">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="b065b-171">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b065b-171">browserBlockJavaScript</span></span>|<span data-ttu-id="b065b-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-172">Boolean</span></span>|<span data-ttu-id="b065b-173">Indica se o usuário será ou não impedido de usar JavaScript.</span><span class="sxs-lookup"><span data-stu-id="b065b-173">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="b065b-174">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="b065b-174">browserBlockPlugins</span></span>|<span data-ttu-id="b065b-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-175">Boolean</span></span>|<span data-ttu-id="b065b-176">Indica se os plug-ins devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="b065b-176">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="b065b-177">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b065b-177">browserBlockPopups</span></span>|<span data-ttu-id="b065b-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-178">Boolean</span></span>|<span data-ttu-id="b065b-179">Indica se janelas pop-ups devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="b065b-179">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="b065b-180">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="b065b-180">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="b065b-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-181">Boolean</span></span>|<span data-ttu-id="b065b-182">Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.</span><span class="sxs-lookup"><span data-stu-id="b065b-182">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="b065b-183">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="b065b-183">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="b065b-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-184">Boolean</span></span>|<span data-ttu-id="b065b-185">Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b065b-185">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="b065b-186">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="b065b-186">browserRequireSmartScreen</span></span>|<span data-ttu-id="b065b-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-187">Boolean</span></span>|<span data-ttu-id="b065b-188">Indica se o usuário deverá ou não usar o Filtro SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="b065b-188">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="b065b-189">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="b065b-189">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="b065b-190">String</span><span class="sxs-lookup"><span data-stu-id="b065b-190">String</span></span>|<span data-ttu-id="b065b-191">O local da lista de sites do modo Empresarial.</span><span class="sxs-lookup"><span data-stu-id="b065b-191">The enterprise mode site list location.</span></span> <span data-ttu-id="b065b-192">Pode ser um arquivo local, rede local ou local http.</span><span class="sxs-lookup"><span data-stu-id="b065b-192">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="b065b-193">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b065b-193">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="b065b-194">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b065b-194">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="b065b-195">O nível de segurança da Internet.</span><span class="sxs-lookup"><span data-stu-id="b065b-195">The internet security level.</span></span> <span data-ttu-id="b065b-196">Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b065b-196">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="b065b-197">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b065b-197">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="b065b-198">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b065b-198">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="b065b-199">O nível de segurança da Intranet.</span><span class="sxs-lookup"><span data-stu-id="b065b-199">The Intranet security level.</span></span> <span data-ttu-id="b065b-200">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b065b-200">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="b065b-201">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="b065b-201">browserLoggingReportLocation</span></span>|<span data-ttu-id="b065b-202">String</span><span class="sxs-lookup"><span data-stu-id="b065b-202">String</span></span>|<span data-ttu-id="b065b-203">O local do relatório de registro em log.</span><span class="sxs-lookup"><span data-stu-id="b065b-203">The logging report location.</span></span>|
|<span data-ttu-id="b065b-204">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="b065b-204">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="b065b-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-205">Boolean</span></span>|<span data-ttu-id="b065b-206">Indica se a alta segurança para sites restritos deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="b065b-206">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="b065b-207">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="b065b-207">browserRequireFirewall</span></span>|<span data-ttu-id="b065b-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-208">Boolean</span></span>|<span data-ttu-id="b065b-209">Indica se um firewall deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="b065b-209">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="b065b-210">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="b065b-210">browserRequireFraudWarning</span></span>|<span data-ttu-id="b065b-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-211">Boolean</span></span>|<span data-ttu-id="b065b-212">Indica se um aviso de fraude deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="b065b-212">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="b065b-213">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b065b-213">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="b065b-214">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="b065b-214">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="b065b-215">O nível de segurança de sites confiáveis.</span><span class="sxs-lookup"><span data-stu-id="b065b-215">The trusted sites security level.</span></span> <span data-ttu-id="b065b-216">Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="b065b-216">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="b065b-217">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="b065b-217">cellularBlockDataRoaming</span></span>|<span data-ttu-id="b065b-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-218">Boolean</span></span>|<span data-ttu-id="b065b-219">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b065b-219">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="b065b-220">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="b065b-220">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="b065b-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-221">Boolean</span></span>|<span data-ttu-id="b065b-222">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b065b-222">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b065b-223">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="b065b-223">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="b065b-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-224">Boolean</span></span>|<span data-ttu-id="b065b-225">Indica se o usuário será ou não impedido de usar senha com imagens ou pin.</span><span class="sxs-lookup"><span data-stu-id="b065b-225">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="b065b-226">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b065b-226">passwordExpirationDays</span></span>|<span data-ttu-id="b065b-227">Int32</span><span class="sxs-lookup"><span data-stu-id="b065b-227">Int32</span></span>|<span data-ttu-id="b065b-228">Expiração da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="b065b-228">Password expiration in days.</span></span>|
|<span data-ttu-id="b065b-229">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b065b-229">passwordMinimumLength</span></span>|<span data-ttu-id="b065b-230">Int32</span><span class="sxs-lookup"><span data-stu-id="b065b-230">Int32</span></span>|<span data-ttu-id="b065b-231">O comprimento mínimo da senha.</span><span class="sxs-lookup"><span data-stu-id="b065b-231">The minimum password length.</span></span>|
|<span data-ttu-id="b065b-232">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b065b-232">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b065b-233">Int32</span><span class="sxs-lookup"><span data-stu-id="b065b-233">Int32</span></span>|<span data-ttu-id="b065b-234">Os minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="b065b-234">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b065b-235">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b065b-235">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b065b-236">Int32</span><span class="sxs-lookup"><span data-stu-id="b065b-236">Int32</span></span>|<span data-ttu-id="b065b-237">O número de conjuntos de caracteres necessários na senha.</span><span class="sxs-lookup"><span data-stu-id="b065b-237">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b065b-238">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b065b-238">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b065b-239">Int32</span><span class="sxs-lookup"><span data-stu-id="b065b-239">Int32</span></span>|<span data-ttu-id="b065b-240">O número de senhas anteriores cujo uso deve ser evitado.</span><span class="sxs-lookup"><span data-stu-id="b065b-240">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="b065b-241">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="b065b-241">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b065b-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b065b-242">passwordRequiredType</span></span>|[<span data-ttu-id="b065b-243">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b065b-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b065b-244">O tipo de senha necessária.</span><span class="sxs-lookup"><span data-stu-id="b065b-244">The required password type.</span></span> <span data-ttu-id="b065b-245">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b065b-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b065b-246">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b065b-246">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b065b-247">Int32</span><span class="sxs-lookup"><span data-stu-id="b065b-247">Int32</span></span>|<span data-ttu-id="b065b-248">O número de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="b065b-248">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="b065b-249">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="b065b-249">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="b065b-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-250">Boolean</span></span>|<span data-ttu-id="b065b-251">Indica se a criptografia é ou não necessária em um dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="b065b-251">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="b065b-252">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="b065b-252">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="b065b-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="b065b-253">Boolean</span></span>|<span data-ttu-id="b065b-254">Indica se as atualizações automáticas devem ou não ser exigidas.</span><span class="sxs-lookup"><span data-stu-id="b065b-254">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="b065b-255">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="b065b-255">userAccountControlSettings</span></span>|[<span data-ttu-id="b065b-256">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="b065b-256">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="b065b-257">As configurações de controle da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="b065b-257">The user account control settings.</span></span> <span data-ttu-id="b065b-258">Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="b065b-258">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="b065b-259">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="b065b-259">workFoldersUrl</span></span>|<span data-ttu-id="b065b-260">String</span><span class="sxs-lookup"><span data-stu-id="b065b-260">String</span></span>|<span data-ttu-id="b065b-261">A URL das pastas de trabalho</span><span class="sxs-lookup"><span data-stu-id="b065b-261">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="b065b-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="b065b-262">Response</span></span>
<span data-ttu-id="b065b-263">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b065b-263">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b065b-264">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b065b-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="b065b-265">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b065b-265">Request</span></span>
<span data-ttu-id="b065b-266">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b065b-266">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b065b-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="b065b-267">Response</span></span>
<span data-ttu-id="b065b-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b065b-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



