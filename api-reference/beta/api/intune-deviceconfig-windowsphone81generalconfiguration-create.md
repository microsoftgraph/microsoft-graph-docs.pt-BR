---
title: Criar windowsPhone81GeneralConfiguration
description: Criar um novo objeto windowsPhone81GeneralConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7f28e854d113e205481529a212fa0e90e0056f15
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42734348"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="986b6-103">Criar windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="986b6-103">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="986b6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="986b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="986b6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="986b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="986b6-106">Criar um novo objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="986b6-106">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="986b6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="986b6-107">Prerequisites</span></span>
<span data-ttu-id="986b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="986b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="986b6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="986b6-110">Permission type</span></span>|<span data-ttu-id="986b6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="986b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="986b6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="986b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="986b6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="986b6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="986b6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="986b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="986b6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="986b6-115">Not supported.</span></span>|
|<span data-ttu-id="986b6-116">Application</span><span class="sxs-lookup"><span data-stu-id="986b6-116">Application</span></span>|<span data-ttu-id="986b6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="986b6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="986b6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="986b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="986b6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="986b6-119">Request headers</span></span>
|<span data-ttu-id="986b6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="986b6-120">Header</span></span>|<span data-ttu-id="986b6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="986b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="986b6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="986b6-122">Authorization</span></span>|<span data-ttu-id="986b6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="986b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="986b6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="986b6-124">Accept</span></span>|<span data-ttu-id="986b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="986b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="986b6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="986b6-126">Request body</span></span>
<span data-ttu-id="986b6-127">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="986b6-127">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="986b6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="986b6-128">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="986b6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="986b6-129">Property</span></span>|<span data-ttu-id="986b6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="986b6-130">Type</span></span>|<span data-ttu-id="986b6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="986b6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="986b6-132">id</span><span class="sxs-lookup"><span data-stu-id="986b6-132">id</span></span>|<span data-ttu-id="986b6-133">String</span><span class="sxs-lookup"><span data-stu-id="986b6-133">String</span></span>|<span data-ttu-id="986b6-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="986b6-134">Key of the entity.</span></span> <span data-ttu-id="986b6-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="986b6-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="986b6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="986b6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="986b6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="986b6-137">DateTimeOffset</span></span>|<span data-ttu-id="986b6-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="986b6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="986b6-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="986b6-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="986b6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="986b6-140">roleScopeTagIds</span></span>|<span data-ttu-id="986b6-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="986b6-141">String collection</span></span>|<span data-ttu-id="986b6-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="986b6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="986b6-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="986b6-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="986b6-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="986b6-144">supportsScopeTags</span></span>|<span data-ttu-id="986b6-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-145">Boolean</span></span>|<span data-ttu-id="986b6-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="986b6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="986b6-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="986b6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="986b6-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="986b6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="986b6-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="986b6-149">This property is read-only.</span></span> <span data-ttu-id="986b6-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="986b6-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="986b6-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="986b6-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="986b6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="986b6-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="986b6-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="986b6-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="986b6-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="986b6-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="986b6-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="986b6-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="986b6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="986b6-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="986b6-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="986b6-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="986b6-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="986b6-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="986b6-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="986b6-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="986b6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="986b6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="986b6-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="986b6-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="986b6-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="986b6-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="986b6-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="986b6-163">createdDateTime</span></span>|<span data-ttu-id="986b6-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="986b6-164">DateTimeOffset</span></span>|<span data-ttu-id="986b6-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="986b6-165">DateTime the object was created.</span></span> <span data-ttu-id="986b6-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="986b6-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="986b6-167">description</span><span class="sxs-lookup"><span data-stu-id="986b6-167">description</span></span>|<span data-ttu-id="986b6-168">String</span><span class="sxs-lookup"><span data-stu-id="986b6-168">String</span></span>|<span data-ttu-id="986b6-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="986b6-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="986b6-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="986b6-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="986b6-171">displayName</span><span class="sxs-lookup"><span data-stu-id="986b6-171">displayName</span></span>|<span data-ttu-id="986b6-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="986b6-172">String</span></span>|<span data-ttu-id="986b6-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="986b6-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="986b6-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="986b6-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="986b6-175">versão</span><span class="sxs-lookup"><span data-stu-id="986b6-175">version</span></span>|<span data-ttu-id="986b6-176">Int32</span><span class="sxs-lookup"><span data-stu-id="986b6-176">Int32</span></span>|<span data-ttu-id="986b6-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="986b6-177">Version of the device configuration.</span></span> <span data-ttu-id="986b6-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="986b6-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="986b6-179">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="986b6-179">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="986b6-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-180">Boolean</span></span>|<span data-ttu-id="986b6-181">Valor que indica se esta política se aplica somente ao Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="986b6-181">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="986b6-182">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="986b6-182">This property is read-only.</span></span>|
|<span data-ttu-id="986b6-183">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="986b6-183">appsBlockCopyPaste</span></span>|<span data-ttu-id="986b6-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-184">Boolean</span></span>|<span data-ttu-id="986b6-185">Indica se a função copiar/colar deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="986b6-185">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="986b6-186">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="986b6-186">bluetoothBlocked</span></span>|<span data-ttu-id="986b6-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-187">Boolean</span></span>|<span data-ttu-id="986b6-188">Indica se o bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="986b6-188">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="986b6-189">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="986b6-189">cameraBlocked</span></span>|<span data-ttu-id="986b6-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-190">Boolean</span></span>|<span data-ttu-id="986b6-191">Indica se a câmera deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="986b6-191">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="986b6-192">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="986b6-192">cellularBlockWifiTethering</span></span>|<span data-ttu-id="986b6-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-193">Boolean</span></span>|<span data-ttu-id="986b6-194">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="986b6-194">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="986b6-195">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="986b6-195">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="986b6-196">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="986b6-196">compliantAppsList</span></span>|<span data-ttu-id="986b6-197">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="986b6-197">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="986b6-198">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="986b6-198">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="986b6-199">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="986b6-199">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="986b6-200">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="986b6-200">compliantAppListType</span></span>|[<span data-ttu-id="986b6-201">appListType</span><span class="sxs-lookup"><span data-stu-id="986b6-201">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="986b6-202">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="986b6-202">List that is in the AppComplianceList.</span></span> <span data-ttu-id="986b6-203">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="986b6-203">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="986b6-204">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="986b6-204">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="986b6-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-205">Boolean</span></span>|<span data-ttu-id="986b6-206">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="986b6-206">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="986b6-207">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="986b6-207">emailBlockAddingAccounts</span></span>|<span data-ttu-id="986b6-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-208">Boolean</span></span>|<span data-ttu-id="986b6-209">Indica se as contas de email personalizadas devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="986b6-209">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="986b6-210">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="986b6-210">locationServicesBlocked</span></span>|<span data-ttu-id="986b6-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-211">Boolean</span></span>|<span data-ttu-id="986b6-212">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="986b6-212">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="986b6-213">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="986b6-213">microsoftAccountBlocked</span></span>|<span data-ttu-id="986b6-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-214">Boolean</span></span>|<span data-ttu-id="986b6-215">Indica se o uso de uma conta da Microsoft deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="986b6-215">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="986b6-216">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="986b6-216">nfcBlocked</span></span>|<span data-ttu-id="986b6-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-217">Boolean</span></span>|<span data-ttu-id="986b6-218">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="986b6-218">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="986b6-219">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="986b6-219">passwordBlockSimple</span></span>|<span data-ttu-id="986b6-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-220">Boolean</span></span>|<span data-ttu-id="986b6-221">Indica se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="986b6-221">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="986b6-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="986b6-222">passwordExpirationDays</span></span>|<span data-ttu-id="986b6-223">Int32</span><span class="sxs-lookup"><span data-stu-id="986b6-223">Int32</span></span>|<span data-ttu-id="986b6-224">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="986b6-224">Number of days before the password expires.</span></span>|
|<span data-ttu-id="986b6-225">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="986b6-225">passwordMinimumLength</span></span>|<span data-ttu-id="986b6-226">Int32</span><span class="sxs-lookup"><span data-stu-id="986b6-226">Int32</span></span>|<span data-ttu-id="986b6-227">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="986b6-227">Minimum length of passwords.</span></span>|
|<span data-ttu-id="986b6-228">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="986b6-228">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="986b6-229">Int32</span><span class="sxs-lookup"><span data-stu-id="986b6-229">Int32</span></span>|<span data-ttu-id="986b6-230">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="986b6-230">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="986b6-231">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="986b6-231">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="986b6-232">Int32</span><span class="sxs-lookup"><span data-stu-id="986b6-232">Int32</span></span>|<span data-ttu-id="986b6-233">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="986b6-233">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="986b6-234">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="986b6-234">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="986b6-235">Int32</span><span class="sxs-lookup"><span data-stu-id="986b6-235">Int32</span></span>|<span data-ttu-id="986b6-236">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="986b6-236">Number of previous passwords to block.</span></span> <span data-ttu-id="986b6-237">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="986b6-237">Valid values 0 to 24</span></span>|
|<span data-ttu-id="986b6-238">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="986b6-238">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="986b6-239">Int32</span><span class="sxs-lookup"><span data-stu-id="986b6-239">Int32</span></span>|<span data-ttu-id="986b6-240">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="986b6-240">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="986b6-241">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="986b6-241">passwordRequiredType</span></span>|[<span data-ttu-id="986b6-242">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="986b6-242">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="986b6-243">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="986b6-243">Password type that is required.</span></span> <span data-ttu-id="986b6-244">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="986b6-244">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="986b6-245">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="986b6-245">passwordRequired</span></span>|<span data-ttu-id="986b6-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-246">Boolean</span></span>|<span data-ttu-id="986b6-247">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="986b6-247">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="986b6-248">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="986b6-248">screenCaptureBlocked</span></span>|<span data-ttu-id="986b6-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-249">Boolean</span></span>|<span data-ttu-id="986b6-250">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="986b6-250">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="986b6-251">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="986b6-251">storageBlockRemovableStorage</span></span>|<span data-ttu-id="986b6-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-252">Boolean</span></span>|<span data-ttu-id="986b6-253">Indica se o armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="986b6-253">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="986b6-254">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="986b6-254">storageRequireEncryption</span></span>|<span data-ttu-id="986b6-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-255">Boolean</span></span>|<span data-ttu-id="986b6-256">Indica se a criptografia é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="986b6-256">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="986b6-257">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="986b6-257">webBrowserBlocked</span></span>|<span data-ttu-id="986b6-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-258">Boolean</span></span>|<span data-ttu-id="986b6-259">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="986b6-259">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="986b6-260">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="986b6-260">wifiBlocked</span></span>|<span data-ttu-id="986b6-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-261">Boolean</span></span>|<span data-ttu-id="986b6-262">Indica se o Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="986b6-262">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="986b6-263">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="986b6-263">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="986b6-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-264">Boolean</span></span>|<span data-ttu-id="986b6-265">Indica se a conexão automática a hotspots Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="986b6-265">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="986b6-266">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="986b6-266">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="986b6-267">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="986b6-267">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="986b6-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-268">Boolean</span></span>|<span data-ttu-id="986b6-269">Indica se os relatórios de hotspot Wi-Fi devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="986b6-269">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="986b6-270">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="986b6-270">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="986b6-271">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="986b6-271">windowsStoreBlocked</span></span>|<span data-ttu-id="986b6-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="986b6-272">Boolean</span></span>|<span data-ttu-id="986b6-273">Indica se a Windows Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="986b6-273">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="986b6-274">Resposta</span><span class="sxs-lookup"><span data-stu-id="986b6-274">Response</span></span>
<span data-ttu-id="986b6-275">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="986b6-275">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="986b6-276">Exemplo</span><span class="sxs-lookup"><span data-stu-id="986b6-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="986b6-277">Solicitação</span><span class="sxs-lookup"><span data-stu-id="986b6-277">Request</span></span>
<span data-ttu-id="986b6-278">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="986b6-278">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2326

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="986b6-279">Resposta</span><span class="sxs-lookup"><span data-stu-id="986b6-279">Response</span></span>
<span data-ttu-id="986b6-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="986b6-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2498

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```




