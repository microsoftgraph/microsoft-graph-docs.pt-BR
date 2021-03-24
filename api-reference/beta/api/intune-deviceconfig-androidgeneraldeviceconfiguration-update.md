---
title: Atualizar androidGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto androidGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8db51e97f79ac6e8dbe32236dd80d3dcff3307b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51138033"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="35884-103">Atualizar androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="35884-103">Update androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="35884-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35884-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35884-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35884-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35884-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35884-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35884-107">Atualizar as propriedades de um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35884-107">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35884-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="35884-108">Prerequisites</span></span>
<span data-ttu-id="35884-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35884-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35884-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35884-111">Permission type</span></span>|<span data-ttu-id="35884-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35884-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35884-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35884-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35884-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35884-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35884-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35884-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35884-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35884-116">Not supported.</span></span>|
|<span data-ttu-id="35884-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35884-117">Application</span></span>|<span data-ttu-id="35884-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35884-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35884-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35884-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="35884-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35884-120">Request headers</span></span>
|<span data-ttu-id="35884-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35884-121">Header</span></span>|<span data-ttu-id="35884-122">Valor</span><span class="sxs-lookup"><span data-stu-id="35884-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35884-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="35884-123">Authorization</span></span>|<span data-ttu-id="35884-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35884-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35884-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="35884-125">Accept</span></span>|<span data-ttu-id="35884-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35884-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35884-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35884-127">Request body</span></span>
<span data-ttu-id="35884-128">No corpo da solicitação, forneça uma representação JSON do objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35884-128">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="35884-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="35884-129">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="35884-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35884-130">Property</span></span>|<span data-ttu-id="35884-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="35884-131">Type</span></span>|<span data-ttu-id="35884-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="35884-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35884-133">id</span><span class="sxs-lookup"><span data-stu-id="35884-133">id</span></span>|<span data-ttu-id="35884-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35884-134">String</span></span>|<span data-ttu-id="35884-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="35884-135">Key of the entity.</span></span> <span data-ttu-id="35884-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35884-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35884-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35884-137">lastModifiedDateTime</span></span>|<span data-ttu-id="35884-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35884-138">DateTimeOffset</span></span>|<span data-ttu-id="35884-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="35884-139">DateTime the object was last modified.</span></span> <span data-ttu-id="35884-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35884-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35884-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35884-141">roleScopeTagIds</span></span>|<span data-ttu-id="35884-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="35884-142">String collection</span></span>|<span data-ttu-id="35884-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="35884-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="35884-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35884-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35884-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="35884-145">supportsScopeTags</span></span>|<span data-ttu-id="35884-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="35884-146">Boolean</span></span>|<span data-ttu-id="35884-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="35884-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="35884-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="35884-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="35884-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="35884-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="35884-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35884-150">This property is read-only.</span></span> <span data-ttu-id="35884-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35884-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35884-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="35884-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="35884-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="35884-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="35884-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="35884-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="35884-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35884-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35884-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="35884-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="35884-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="35884-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="35884-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="35884-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="35884-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35884-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35884-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="35884-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="35884-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="35884-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="35884-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="35884-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="35884-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35884-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35884-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35884-164">createdDateTime</span></span>|<span data-ttu-id="35884-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35884-165">DateTimeOffset</span></span>|<span data-ttu-id="35884-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="35884-166">DateTime the object was created.</span></span> <span data-ttu-id="35884-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35884-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35884-168">descrição</span><span class="sxs-lookup"><span data-stu-id="35884-168">description</span></span>|<span data-ttu-id="35884-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35884-169">String</span></span>|<span data-ttu-id="35884-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35884-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="35884-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35884-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35884-172">displayName</span><span class="sxs-lookup"><span data-stu-id="35884-172">displayName</span></span>|<span data-ttu-id="35884-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35884-173">String</span></span>|<span data-ttu-id="35884-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35884-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="35884-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35884-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35884-176">versão</span><span class="sxs-lookup"><span data-stu-id="35884-176">version</span></span>|<span data-ttu-id="35884-177">Int32</span><span class="sxs-lookup"><span data-stu-id="35884-177">Int32</span></span>|<span data-ttu-id="35884-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="35884-178">Version of the device configuration.</span></span> <span data-ttu-id="35884-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="35884-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="35884-180">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="35884-180">appsBlockClipboardSharing</span></span>|<span data-ttu-id="35884-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-181">Boolean</span></span>|<span data-ttu-id="35884-182">Indica se a função de copiar e colar entre aplicativos será bloqueada ou não no compartilhamento de área de transferência.</span><span class="sxs-lookup"><span data-stu-id="35884-182">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="35884-183">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="35884-183">appsBlockCopyPaste</span></span>|<span data-ttu-id="35884-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-184">Boolean</span></span>|<span data-ttu-id="35884-185">Indica se a função de copiar e colar dentro de aplicativos será bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="35884-185">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="35884-186">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="35884-186">appsBlockYouTube</span></span>|<span data-ttu-id="35884-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-187">Boolean</span></span>|<span data-ttu-id="35884-188">Indica se o aplicativo YouTube deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-188">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="35884-189">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="35884-189">bluetoothBlocked</span></span>|<span data-ttu-id="35884-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-190">Boolean</span></span>|<span data-ttu-id="35884-191">Indica se o Bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-191">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="35884-192">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="35884-192">cameraBlocked</span></span>|<span data-ttu-id="35884-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-193">Boolean</span></span>|<span data-ttu-id="35884-194">Indica se o uso da câmera deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-194">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="35884-195">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="35884-195">cellularBlockDataRoaming</span></span>|<span data-ttu-id="35884-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-196">Boolean</span></span>|<span data-ttu-id="35884-197">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-197">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="35884-198">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="35884-198">cellularBlockMessaging</span></span>|<span data-ttu-id="35884-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-199">Boolean</span></span>|<span data-ttu-id="35884-200">Indica se as mensagens SMS/MMS devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="35884-200">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="35884-201">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="35884-201">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="35884-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-202">Boolean</span></span>|<span data-ttu-id="35884-203">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-203">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="35884-204">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="35884-204">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="35884-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-205">Boolean</span></span>|<span data-ttu-id="35884-206">Indica se a sincronização de compartilhamento de Internet por Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="35884-206">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="35884-207">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="35884-207">compliantAppsList</span></span>|<span data-ttu-id="35884-208">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="35884-208">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="35884-209">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="35884-209">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="35884-210">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="35884-210">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="35884-211">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="35884-211">compliantAppListType</span></span>|[<span data-ttu-id="35884-212">appListType</span><span class="sxs-lookup"><span data-stu-id="35884-212">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="35884-213">Tipo de lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="35884-213">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="35884-214">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="35884-214">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="35884-215">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="35884-215">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="35884-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-216">Boolean</span></span>|<span data-ttu-id="35884-217">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-217">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="35884-218">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="35884-218">locationServicesBlocked</span></span>|<span data-ttu-id="35884-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-219">Boolean</span></span>|<span data-ttu-id="35884-220">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="35884-220">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="35884-221">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="35884-221">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="35884-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-222">Boolean</span></span>|<span data-ttu-id="35884-223">Indica se a sincronização automática da conta do Google deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="35884-223">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="35884-224">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="35884-224">googlePlayStoreBlocked</span></span>|<span data-ttu-id="35884-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-225">Boolean</span></span>|<span data-ttu-id="35884-226">Indica se a Google Play Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="35884-226">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="35884-227">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="35884-227">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="35884-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-228">Boolean</span></span>|<span data-ttu-id="35884-229">Indica se o botão de suspensão de tela deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="35884-229">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="35884-230">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="35884-230">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="35884-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-231">Boolean</span></span>|<span data-ttu-id="35884-232">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="35884-232">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="35884-233">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="35884-233">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="35884-234">Booleano</span><span class="sxs-lookup"><span data-stu-id="35884-234">Boolean</span></span>|<span data-ttu-id="35884-235">Indica se é ou não para bloquear a alteração de data e hora enquanto estiver no modo KNOX.</span><span class="sxs-lookup"><span data-stu-id="35884-235">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="35884-236">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="35884-236">kioskModeApps</span></span>|<span data-ttu-id="35884-237">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="35884-237">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="35884-238">Uma lista de aplicativos que poderão ser executados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="35884-238">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="35884-239">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="35884-239">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="35884-240">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="35884-240">nfcBlocked</span></span>|<span data-ttu-id="35884-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-241">Boolean</span></span>|<span data-ttu-id="35884-242">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="35884-242">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="35884-243">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="35884-243">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="35884-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-244">Boolean</span></span>|<span data-ttu-id="35884-245">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-245">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="35884-246">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="35884-246">passwordBlockTrustAgents</span></span>|<span data-ttu-id="35884-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-247">Boolean</span></span>|<span data-ttu-id="35884-248">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="35884-248">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="35884-249">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="35884-249">passwordExpirationDays</span></span>|<span data-ttu-id="35884-250">Int32</span><span class="sxs-lookup"><span data-stu-id="35884-250">Int32</span></span>|<span data-ttu-id="35884-251">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="35884-251">Number of days before the password expires.</span></span> <span data-ttu-id="35884-252">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="35884-252">Valid values 1 to 365</span></span>|
|<span data-ttu-id="35884-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="35884-253">passwordMinimumLength</span></span>|<span data-ttu-id="35884-254">Int32</span><span class="sxs-lookup"><span data-stu-id="35884-254">Int32</span></span>|<span data-ttu-id="35884-255">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="35884-255">Minimum length of passwords.</span></span> <span data-ttu-id="35884-256">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="35884-256">Valid values 4 to 16</span></span>|
|<span data-ttu-id="35884-257">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="35884-257">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="35884-258">Int32</span><span class="sxs-lookup"><span data-stu-id="35884-258">Int32</span></span>|<span data-ttu-id="35884-259">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="35884-259">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="35884-260">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="35884-260">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="35884-261">Int32</span><span class="sxs-lookup"><span data-stu-id="35884-261">Int32</span></span>|<span data-ttu-id="35884-262">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="35884-262">Number of previous passwords to block.</span></span> <span data-ttu-id="35884-263">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="35884-263">Valid values 0 to 24</span></span>|
|<span data-ttu-id="35884-264">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="35884-264">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="35884-265">Int32</span><span class="sxs-lookup"><span data-stu-id="35884-265">Int32</span></span>|<span data-ttu-id="35884-266">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="35884-266">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="35884-267">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="35884-267">Valid values 1 to 16</span></span>|
|<span data-ttu-id="35884-268">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="35884-268">passwordRequiredType</span></span>|[<span data-ttu-id="35884-269">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="35884-269">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="35884-270">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="35884-270">Type of password that is required.</span></span> <span data-ttu-id="35884-271">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="35884-271">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="35884-272">requiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="35884-272">requiredPasswordComplexity</span></span>|[<span data-ttu-id="35884-273">androidRequiredPasswordComplexity</span><span class="sxs-lookup"><span data-stu-id="35884-273">androidRequiredPasswordComplexity</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordcomplexity.md)|<span data-ttu-id="35884-274">Indica a complexidade de senha necessária no Android.</span><span class="sxs-lookup"><span data-stu-id="35884-274">Indicates the required password complexity on Android.</span></span> <span data-ttu-id="35884-275">Um deles: NONE, LOW, MEDIUM, HIGH.</span><span class="sxs-lookup"><span data-stu-id="35884-275">One of: NONE, LOW, MEDIUM, HIGH.</span></span> <span data-ttu-id="35884-276">Esta é uma API direcionada ao Android 11+.</span><span class="sxs-lookup"><span data-stu-id="35884-276">This is an API targeted to Android 11+.</span></span> <span data-ttu-id="35884-277">Os valores possíveis são: `none`, `low`, `medium`, `high`.</span><span class="sxs-lookup"><span data-stu-id="35884-277">Possible values are: `none`, `low`, `medium`, `high`.</span></span>|
|<span data-ttu-id="35884-278">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="35884-278">passwordRequired</span></span>|<span data-ttu-id="35884-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-279">Boolean</span></span>|<span data-ttu-id="35884-280">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="35884-280">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="35884-281">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="35884-281">powerOffBlocked</span></span>|<span data-ttu-id="35884-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-282">Boolean</span></span>|<span data-ttu-id="35884-283">Indica se o desligamento do dispositivo deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-283">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="35884-284">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="35884-284">factoryResetBlocked</span></span>|<span data-ttu-id="35884-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-285">Boolean</span></span>|<span data-ttu-id="35884-286">Indica se o usuário será ou não impedido de executar uma restauração de fábrica.</span><span class="sxs-lookup"><span data-stu-id="35884-286">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="35884-287">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="35884-287">screenCaptureBlocked</span></span>|<span data-ttu-id="35884-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-288">Boolean</span></span>|<span data-ttu-id="35884-289">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="35884-289">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="35884-290">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="35884-290">deviceSharingAllowed</span></span>|<span data-ttu-id="35884-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-291">Boolean</span></span>|<span data-ttu-id="35884-292">Indica se o modo de compartilhamento do dispositivo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="35884-292">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="35884-293">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="35884-293">storageBlockGoogleBackup</span></span>|<span data-ttu-id="35884-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-294">Boolean</span></span>|<span data-ttu-id="35884-295">Indica se o Backup do Google deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-295">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="35884-296">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="35884-296">storageBlockRemovableStorage</span></span>|<span data-ttu-id="35884-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-297">Boolean</span></span>|<span data-ttu-id="35884-298">Indica se o uso do armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-298">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="35884-299">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="35884-299">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="35884-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-300">Boolean</span></span>|<span data-ttu-id="35884-301">Indica se a criptografia do dispositivo é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="35884-301">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="35884-302">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="35884-302">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="35884-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-303">Boolean</span></span>|<span data-ttu-id="35884-304">Indica se a criptografia do armazenamento removível é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="35884-304">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="35884-305">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="35884-305">voiceAssistantBlocked</span></span>|<span data-ttu-id="35884-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-306">Boolean</span></span>|<span data-ttu-id="35884-307">Indica se o uso do Assistente de voz será ou não bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-307">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="35884-308">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="35884-308">voiceDialingBlocked</span></span>|<span data-ttu-id="35884-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-309">Boolean</span></span>|<span data-ttu-id="35884-310">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="35884-310">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="35884-311">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="35884-311">webBrowserBlockPopups</span></span>|<span data-ttu-id="35884-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-312">Boolean</span></span>|<span data-ttu-id="35884-313">Indica se os pop-ups dentro do navegador da Web devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="35884-313">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="35884-314">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="35884-314">webBrowserBlockAutofill</span></span>|<span data-ttu-id="35884-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-315">Boolean</span></span>|<span data-ttu-id="35884-316">Indica se o recurso de preenchimento automático do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-316">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="35884-317">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="35884-317">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="35884-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-318">Boolean</span></span>|<span data-ttu-id="35884-319">Indica se o JavaScript dentro do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-319">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="35884-320">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="35884-320">webBrowserBlocked</span></span>|<span data-ttu-id="35884-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-321">Boolean</span></span>|<span data-ttu-id="35884-322">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="35884-322">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="35884-323">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="35884-323">webBrowserCookieSettings</span></span>|[<span data-ttu-id="35884-324">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="35884-324">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="35884-325">Configuração de cookies do navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="35884-325">Cookie settings within the web browser.</span></span> <span data-ttu-id="35884-326">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="35884-326">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="35884-327">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="35884-327">wiFiBlocked</span></span>|<span data-ttu-id="35884-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-328">Boolean</span></span>|<span data-ttu-id="35884-329">Indica se a sincronização de Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="35884-329">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="35884-330">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="35884-330">appsInstallAllowList</span></span>|<span data-ttu-id="35884-331">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="35884-331">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="35884-332">Lista de aplicativos que podem ser instalados no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="35884-332">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="35884-333">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="35884-333">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="35884-334">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="35884-334">appsLaunchBlockList</span></span>|<span data-ttu-id="35884-335">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="35884-335">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="35884-336">Lista de aplicativos que não podem ser abertos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="35884-336">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="35884-337">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="35884-337">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="35884-338">appsHideList</span><span class="sxs-lookup"><span data-stu-id="35884-338">appsHideList</span></span>|<span data-ttu-id="35884-339">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="35884-339">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="35884-340">Lista de aplicativos que devem ficar ocultos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="35884-340">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="35884-341">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="35884-341">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="35884-342">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="35884-342">securityRequireVerifyApps</span></span>|<span data-ttu-id="35884-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="35884-343">Boolean</span></span>|<span data-ttu-id="35884-344">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="35884-344">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="35884-345">Resposta</span><span class="sxs-lookup"><span data-stu-id="35884-345">Response</span></span>
<span data-ttu-id="35884-346">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35884-346">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35884-347">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35884-347">Example</span></span>

### <a name="request"></a><span data-ttu-id="35884-348">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35884-348">Request</span></span>
<span data-ttu-id="35884-349">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35884-349">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3974

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
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
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
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
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "requiredPasswordComplexity": "low",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="35884-350">Resposta</span><span class="sxs-lookup"><span data-stu-id="35884-350">Response</span></span>
<span data-ttu-id="35884-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35884-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4146

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
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
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
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
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "dateAndTimeBlockChanges": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
  "requiredPasswordComplexity": "low",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```




