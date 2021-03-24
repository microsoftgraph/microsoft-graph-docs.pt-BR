---
title: Criar windowsPhone81GeneralConfiguration
description: Criar um novo objeto windowsPhone81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 072cc57fb2282a41ab6b6bbbaeeea49220c435a1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127260"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="4f2d6-103">Criar windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4f2d6-103">Create windowsPhone81GeneralConfiguration</span></span>

<span data-ttu-id="4f2d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f2d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f2d6-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f2d6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f2d6-107">Criar um novo objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f2d6-107">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f2d6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f2d6-108">Prerequisites</span></span>
<span data-ttu-id="4f2d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f2d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f2d6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f2d6-111">Permission type</span></span>|<span data-ttu-id="4f2d6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f2d6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f2d6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f2d6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f2d6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f2d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-116">Not supported.</span></span>|
|<span data-ttu-id="4f2d6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f2d6-117">Application</span></span>|<span data-ttu-id="4f2d6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f2d6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f2d6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f2d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4f2d6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f2d6-120">Request headers</span></span>
|<span data-ttu-id="4f2d6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f2d6-121">Header</span></span>|<span data-ttu-id="4f2d6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4f2d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f2d6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f2d6-123">Authorization</span></span>|<span data-ttu-id="4f2d6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f2d6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f2d6-125">Accept</span></span>|<span data-ttu-id="4f2d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f2d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f2d6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f2d6-127">Request body</span></span>
<span data-ttu-id="4f2d6-128">No corpo da solicitação, forneça uma representação JSON do objeto windowsPhone81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-128">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="4f2d6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windowsPhone81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-129">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="4f2d6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f2d6-130">Property</span></span>|<span data-ttu-id="4f2d6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f2d6-131">Type</span></span>|<span data-ttu-id="4f2d6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f2d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f2d6-133">id</span><span class="sxs-lookup"><span data-stu-id="4f2d6-133">id</span></span>|<span data-ttu-id="4f2d6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f2d6-134">String</span></span>|<span data-ttu-id="4f2d6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-135">Key of the entity.</span></span> <span data-ttu-id="4f2d6-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f2d6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f2d6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4f2d6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f2d6-138">DateTimeOffset</span></span>|<span data-ttu-id="4f2d6-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4f2d6-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f2d6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f2d6-141">roleScopeTagIds</span></span>|<span data-ttu-id="4f2d6-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f2d6-142">String collection</span></span>|<span data-ttu-id="4f2d6-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4f2d6-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f2d6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4f2d6-145">supportsScopeTags</span></span>|<span data-ttu-id="4f2d6-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="4f2d6-146">Boolean</span></span>|<span data-ttu-id="4f2d6-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4f2d6-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4f2d6-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4f2d6-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-150">This property is read-only.</span></span> <span data-ttu-id="4f2d6-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f2d6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4f2d6-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4f2d6-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4f2d6-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4f2d6-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4f2d6-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f2d6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4f2d6-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4f2d6-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4f2d6-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4f2d6-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4f2d6-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f2d6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4f2d6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4f2d6-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4f2d6-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4f2d6-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4f2d6-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f2d6-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f2d6-164">createdDateTime</span></span>|<span data-ttu-id="4f2d6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f2d6-165">DateTimeOffset</span></span>|<span data-ttu-id="4f2d6-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-166">DateTime the object was created.</span></span> <span data-ttu-id="4f2d6-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f2d6-168">descrição</span><span class="sxs-lookup"><span data-stu-id="4f2d6-168">description</span></span>|<span data-ttu-id="4f2d6-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f2d6-169">String</span></span>|<span data-ttu-id="4f2d6-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4f2d6-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f2d6-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4f2d6-172">displayName</span></span>|<span data-ttu-id="4f2d6-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f2d6-173">String</span></span>|<span data-ttu-id="4f2d6-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4f2d6-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f2d6-176">versão</span><span class="sxs-lookup"><span data-stu-id="4f2d6-176">version</span></span>|<span data-ttu-id="4f2d6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4f2d6-177">Int32</span></span>|<span data-ttu-id="4f2d6-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-178">Version of the device configuration.</span></span> <span data-ttu-id="4f2d6-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f2d6-180">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="4f2d6-180">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="4f2d6-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-181">Boolean</span></span>|<span data-ttu-id="4f2d6-182">Valor que indica se esta política se aplica somente ao Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-182">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="4f2d6-183">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-183">This property is read-only.</span></span>|
|<span data-ttu-id="4f2d6-184">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="4f2d6-184">appsBlockCopyPaste</span></span>|<span data-ttu-id="4f2d6-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-185">Boolean</span></span>|<span data-ttu-id="4f2d6-186">Indica se a função copiar/colar deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-186">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="4f2d6-187">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="4f2d6-187">bluetoothBlocked</span></span>|<span data-ttu-id="4f2d6-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-188">Boolean</span></span>|<span data-ttu-id="4f2d6-189">Indica se o bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-189">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="4f2d6-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4f2d6-190">cameraBlocked</span></span>|<span data-ttu-id="4f2d6-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-191">Boolean</span></span>|<span data-ttu-id="4f2d6-192">Indica se a câmera deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-192">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="4f2d6-193">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="4f2d6-193">cellularBlockWifiTethering</span></span>|<span data-ttu-id="4f2d6-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-194">Boolean</span></span>|<span data-ttu-id="4f2d6-195">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-195">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="4f2d6-196">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-196">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4f2d6-197">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="4f2d6-197">compliantAppsList</span></span>|<span data-ttu-id="4f2d6-198">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4f2d6-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4f2d6-199">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="4f2d6-199">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="4f2d6-200">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4f2d6-201">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="4f2d6-201">compliantAppListType</span></span>|[<span data-ttu-id="4f2d6-202">appListType</span><span class="sxs-lookup"><span data-stu-id="4f2d6-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="4f2d6-203">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-203">List that is in the AppComplianceList.</span></span> <span data-ttu-id="4f2d6-204">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="4f2d6-205">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="4f2d6-205">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="4f2d6-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-206">Boolean</span></span>|<span data-ttu-id="4f2d6-207">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-207">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4f2d6-208">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="4f2d6-208">emailBlockAddingAccounts</span></span>|<span data-ttu-id="4f2d6-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-209">Boolean</span></span>|<span data-ttu-id="4f2d6-210">Indica se as contas de email personalizadas devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-210">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="4f2d6-211">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="4f2d6-211">locationServicesBlocked</span></span>|<span data-ttu-id="4f2d6-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-212">Boolean</span></span>|<span data-ttu-id="4f2d6-213">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-213">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="4f2d6-214">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="4f2d6-214">microsoftAccountBlocked</span></span>|<span data-ttu-id="4f2d6-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-215">Boolean</span></span>|<span data-ttu-id="4f2d6-216">Indica se o uso de uma conta da Microsoft deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-216">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="4f2d6-217">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="4f2d6-217">nfcBlocked</span></span>|<span data-ttu-id="4f2d6-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-218">Boolean</span></span>|<span data-ttu-id="4f2d6-219">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-219">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="4f2d6-220">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4f2d6-220">passwordBlockSimple</span></span>|<span data-ttu-id="4f2d6-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-221">Boolean</span></span>|<span data-ttu-id="4f2d6-222">Indica se a sincronização do calendário deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-222">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="4f2d6-223">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4f2d6-223">passwordExpirationDays</span></span>|<span data-ttu-id="4f2d6-224">Int32</span><span class="sxs-lookup"><span data-stu-id="4f2d6-224">Int32</span></span>|<span data-ttu-id="4f2d6-225">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-225">Number of days before the password expires.</span></span>|
|<span data-ttu-id="4f2d6-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4f2d6-226">passwordMinimumLength</span></span>|<span data-ttu-id="4f2d6-227">Int32</span><span class="sxs-lookup"><span data-stu-id="4f2d6-227">Int32</span></span>|<span data-ttu-id="4f2d6-228">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-228">Minimum length of passwords.</span></span>|
|<span data-ttu-id="4f2d6-229">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4f2d6-229">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4f2d6-230">Int32</span><span class="sxs-lookup"><span data-stu-id="4f2d6-230">Int32</span></span>|<span data-ttu-id="4f2d6-231">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-231">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="4f2d6-232">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4f2d6-232">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4f2d6-233">Int32</span><span class="sxs-lookup"><span data-stu-id="4f2d6-233">Int32</span></span>|<span data-ttu-id="4f2d6-234">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-234">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="4f2d6-235">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4f2d6-235">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4f2d6-236">Int32</span><span class="sxs-lookup"><span data-stu-id="4f2d6-236">Int32</span></span>|<span data-ttu-id="4f2d6-237">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-237">Number of previous passwords to block.</span></span> <span data-ttu-id="4f2d6-238">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="4f2d6-238">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4f2d6-239">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4f2d6-239">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4f2d6-240">Int32</span><span class="sxs-lookup"><span data-stu-id="4f2d6-240">Int32</span></span>|<span data-ttu-id="4f2d6-241">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-241">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="4f2d6-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4f2d6-242">passwordRequiredType</span></span>|[<span data-ttu-id="4f2d6-243">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4f2d6-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4f2d6-244">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-244">Password type that is required.</span></span> <span data-ttu-id="4f2d6-245">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4f2d6-246">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4f2d6-246">passwordRequired</span></span>|<span data-ttu-id="4f2d6-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-247">Boolean</span></span>|<span data-ttu-id="4f2d6-248">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-248">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="4f2d6-249">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4f2d6-249">screenCaptureBlocked</span></span>|<span data-ttu-id="4f2d6-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-250">Boolean</span></span>|<span data-ttu-id="4f2d6-251">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-251">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="4f2d6-252">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="4f2d6-252">storageBlockRemovableStorage</span></span>|<span data-ttu-id="4f2d6-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-253">Boolean</span></span>|<span data-ttu-id="4f2d6-254">Indica se o armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-254">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="4f2d6-255">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4f2d6-255">storageRequireEncryption</span></span>|<span data-ttu-id="4f2d6-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-256">Boolean</span></span>|<span data-ttu-id="4f2d6-257">Indica se a criptografia é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-257">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="4f2d6-258">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="4f2d6-258">webBrowserBlocked</span></span>|<span data-ttu-id="4f2d6-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-259">Boolean</span></span>|<span data-ttu-id="4f2d6-260">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-260">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="4f2d6-261">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="4f2d6-261">wifiBlocked</span></span>|<span data-ttu-id="4f2d6-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-262">Boolean</span></span>|<span data-ttu-id="4f2d6-263">Indica se o Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-263">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="4f2d6-264">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="4f2d6-264">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="4f2d6-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-265">Boolean</span></span>|<span data-ttu-id="4f2d6-266">Indica se a conexão automática a hotspots Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-266">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="4f2d6-267">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-267">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4f2d6-268">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="4f2d6-268">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="4f2d6-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-269">Boolean</span></span>|<span data-ttu-id="4f2d6-270">Indica se os relatórios de hotspot Wi-Fi devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-270">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="4f2d6-271">Não terá impacto se o Wi-Fi estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-271">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4f2d6-272">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="4f2d6-272">windowsStoreBlocked</span></span>|<span data-ttu-id="4f2d6-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2d6-273">Boolean</span></span>|<span data-ttu-id="4f2d6-274">Indica se a Windows Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-274">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="4f2d6-275">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f2d6-275">Response</span></span>
<span data-ttu-id="4f2d6-276">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-276">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f2d6-277">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f2d6-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f2d6-278">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f2d6-278">Request</span></span>
<span data-ttu-id="4f2d6-279">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f2d6-280">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f2d6-280">Response</span></span>
<span data-ttu-id="4f2d6-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f2d6-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




