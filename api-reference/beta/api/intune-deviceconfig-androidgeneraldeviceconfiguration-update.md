---
title: Atualizar androidGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto androidGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c6a1b44dcba6ad54f7c389de99d7cb1729bbcdc3
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534488"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="d4ea8-103">Atualizar androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4ea8-103">Update androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="d4ea8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4ea8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4ea8-106">Atualizar as propriedades de um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4ea8-106">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4ea8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4ea8-107">Prerequisites</span></span>
<span data-ttu-id="d4ea8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4ea8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4ea8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4ea8-110">Permission type</span></span>|<span data-ttu-id="d4ea8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4ea8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4ea8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4ea8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4ea8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4ea8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-115">Not supported.</span></span>|
|<span data-ttu-id="d4ea8-116">Application</span><span class="sxs-lookup"><span data-stu-id="d4ea8-116">Application</span></span>|<span data-ttu-id="d4ea8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4ea8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4ea8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4ea8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d4ea8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4ea8-119">Request headers</span></span>
|<span data-ttu-id="d4ea8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4ea8-120">Header</span></span>|<span data-ttu-id="d4ea8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d4ea8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4ea8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4ea8-122">Authorization</span></span>|<span data-ttu-id="d4ea8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4ea8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4ea8-124">Accept</span></span>|<span data-ttu-id="d4ea8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4ea8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4ea8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4ea8-126">Request body</span></span>
<span data-ttu-id="d4ea8-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4ea8-127">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="d4ea8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d4ea8-128">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="d4ea8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4ea8-129">Property</span></span>|<span data-ttu-id="d4ea8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4ea8-130">Type</span></span>|<span data-ttu-id="d4ea8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4ea8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4ea8-132">id</span><span class="sxs-lookup"><span data-stu-id="d4ea8-132">id</span></span>|<span data-ttu-id="d4ea8-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4ea8-133">String</span></span>|<span data-ttu-id="d4ea8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-134">Key of the entity.</span></span> <span data-ttu-id="d4ea8-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4ea8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4ea8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d4ea8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4ea8-137">DateTimeOffset</span></span>|<span data-ttu-id="d4ea8-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d4ea8-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4ea8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d4ea8-140">roleScopeTagIds</span></span>|<span data-ttu-id="d4ea8-141">String collection</span><span class="sxs-lookup"><span data-stu-id="d4ea8-141">String collection</span></span>|<span data-ttu-id="d4ea8-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d4ea8-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4ea8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d4ea8-144">supportsScopeTags</span></span>|<span data-ttu-id="d4ea8-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-145">Boolean</span></span>|<span data-ttu-id="d4ea8-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d4ea8-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d4ea8-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d4ea8-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-149">This property is read-only.</span></span> <span data-ttu-id="d4ea8-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4ea8-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d4ea8-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d4ea8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d4ea8-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d4ea8-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d4ea8-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4ea8-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d4ea8-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d4ea8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d4ea8-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d4ea8-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d4ea8-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4ea8-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d4ea8-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d4ea8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d4ea8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d4ea8-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d4ea8-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4ea8-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4ea8-163">createdDateTime</span></span>|<span data-ttu-id="d4ea8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4ea8-164">DateTimeOffset</span></span>|<span data-ttu-id="d4ea8-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-165">DateTime the object was created.</span></span> <span data-ttu-id="d4ea8-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4ea8-167">description</span><span class="sxs-lookup"><span data-stu-id="d4ea8-167">description</span></span>|<span data-ttu-id="d4ea8-168">String</span><span class="sxs-lookup"><span data-stu-id="d4ea8-168">String</span></span>|<span data-ttu-id="d4ea8-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d4ea8-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4ea8-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d4ea8-171">displayName</span></span>|<span data-ttu-id="d4ea8-172">String</span><span class="sxs-lookup"><span data-stu-id="d4ea8-172">String</span></span>|<span data-ttu-id="d4ea8-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d4ea8-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4ea8-175">versão</span><span class="sxs-lookup"><span data-stu-id="d4ea8-175">version</span></span>|<span data-ttu-id="d4ea8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d4ea8-176">Int32</span></span>|<span data-ttu-id="d4ea8-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-177">Version of the device configuration.</span></span> <span data-ttu-id="d4ea8-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d4ea8-179">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="d4ea8-179">appsBlockClipboardSharing</span></span>|<span data-ttu-id="d4ea8-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-180">Boolean</span></span>|<span data-ttu-id="d4ea8-181">Indica se a função de copiar e colar entre aplicativos será bloqueada ou não no compartilhamento de área de transferência.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-181">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="d4ea8-182">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="d4ea8-182">appsBlockCopyPaste</span></span>|<span data-ttu-id="d4ea8-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-183">Boolean</span></span>|<span data-ttu-id="d4ea8-184">Indica se a função de copiar e colar dentro de aplicativos será bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-184">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="d4ea8-185">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="d4ea8-185">appsBlockYouTube</span></span>|<span data-ttu-id="d4ea8-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-186">Boolean</span></span>|<span data-ttu-id="d4ea8-187">Indica se o aplicativo YouTube deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-187">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="d4ea8-188">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="d4ea8-188">bluetoothBlocked</span></span>|<span data-ttu-id="d4ea8-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-189">Boolean</span></span>|<span data-ttu-id="d4ea8-190">Indica se o Bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-190">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="d4ea8-191">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="d4ea8-191">cameraBlocked</span></span>|<span data-ttu-id="d4ea8-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-192">Boolean</span></span>|<span data-ttu-id="d4ea8-193">Indica se o uso da câmera deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-193">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="d4ea8-194">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="d4ea8-194">cellularBlockDataRoaming</span></span>|<span data-ttu-id="d4ea8-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-195">Boolean</span></span>|<span data-ttu-id="d4ea8-196">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-196">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="d4ea8-197">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="d4ea8-197">cellularBlockMessaging</span></span>|<span data-ttu-id="d4ea8-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-198">Boolean</span></span>|<span data-ttu-id="d4ea8-199">Indica se as mensagens SMS/MMS devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-199">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="d4ea8-200">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="d4ea8-200">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="d4ea8-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-201">Boolean</span></span>|<span data-ttu-id="d4ea8-202">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-202">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="d4ea8-203">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="d4ea8-203">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="d4ea8-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-204">Boolean</span></span>|<span data-ttu-id="d4ea8-205">Indica se a sincronização de compartilhamento de Internet por Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-205">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="d4ea8-206">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="d4ea8-206">compliantAppsList</span></span>|<span data-ttu-id="d4ea8-207">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d4ea8-208">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="d4ea8-208">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="d4ea8-209">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-209">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d4ea8-210">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="d4ea8-210">compliantAppListType</span></span>|[<span data-ttu-id="d4ea8-211">appListType</span><span class="sxs-lookup"><span data-stu-id="d4ea8-211">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d4ea8-212">Tipo de lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-212">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="d4ea8-213">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-213">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d4ea8-214">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="d4ea8-214">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="d4ea8-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-215">Boolean</span></span>|<span data-ttu-id="d4ea8-216">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-216">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="d4ea8-217">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="d4ea8-217">locationServicesBlocked</span></span>|<span data-ttu-id="d4ea8-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-218">Boolean</span></span>|<span data-ttu-id="d4ea8-219">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-219">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="d4ea8-220">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="d4ea8-220">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="d4ea8-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-221">Boolean</span></span>|<span data-ttu-id="d4ea8-222">Indica se a sincronização automática da conta do Google deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-222">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="d4ea8-223">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d4ea8-223">googlePlayStoreBlocked</span></span>|<span data-ttu-id="d4ea8-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4ea8-224">Boolean</span></span>|<span data-ttu-id="d4ea8-225">Indica se a Google Play Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-225">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="d4ea8-226">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="d4ea8-226">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="d4ea8-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-227">Boolean</span></span>|<span data-ttu-id="d4ea8-228">Indica se o botão de suspensão de tela deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-228">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="d4ea8-229">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="d4ea8-229">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="d4ea8-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-230">Boolean</span></span>|<span data-ttu-id="d4ea8-231">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-231">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="d4ea8-232">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="d4ea8-232">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="d4ea8-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-233">Boolean</span></span>|<span data-ttu-id="d4ea8-234">Indica se a data e a hora de alteração serão bloqueadas ou não no modo do KNOX.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-234">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="d4ea8-235">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="d4ea8-235">kioskModeApps</span></span>|<span data-ttu-id="d4ea8-236">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-236">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d4ea8-237">Uma lista de aplicativos que poderão ser executados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-237">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="d4ea8-238">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-238">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d4ea8-239">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="d4ea8-239">nfcBlocked</span></span>|<span data-ttu-id="d4ea8-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-240">Boolean</span></span>|<span data-ttu-id="d4ea8-241">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-241">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="d4ea8-242">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d4ea8-242">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="d4ea8-243">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-243">Boolean</span></span>|<span data-ttu-id="d4ea8-244">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-244">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="d4ea8-245">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="d4ea8-245">passwordBlockTrustAgents</span></span>|<span data-ttu-id="d4ea8-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-246">Boolean</span></span>|<span data-ttu-id="d4ea8-247">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-247">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="d4ea8-248">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d4ea8-248">passwordExpirationDays</span></span>|<span data-ttu-id="d4ea8-249">Int32</span><span class="sxs-lookup"><span data-stu-id="d4ea8-249">Int32</span></span>|<span data-ttu-id="d4ea8-250">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-250">Number of days before the password expires.</span></span> <span data-ttu-id="d4ea8-251">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="d4ea8-251">Valid values 1 to 365</span></span>|
|<span data-ttu-id="d4ea8-252">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d4ea8-252">passwordMinimumLength</span></span>|<span data-ttu-id="d4ea8-253">Int32</span><span class="sxs-lookup"><span data-stu-id="d4ea8-253">Int32</span></span>|<span data-ttu-id="d4ea8-254">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-254">Minimum length of passwords.</span></span> <span data-ttu-id="d4ea8-255">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="d4ea8-255">Valid values 4 to 16</span></span>|
|<span data-ttu-id="d4ea8-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d4ea8-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d4ea8-257">Int32</span><span class="sxs-lookup"><span data-stu-id="d4ea8-257">Int32</span></span>|<span data-ttu-id="d4ea8-258">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-258">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d4ea8-259">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d4ea8-259">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d4ea8-260">Int32</span><span class="sxs-lookup"><span data-stu-id="d4ea8-260">Int32</span></span>|<span data-ttu-id="d4ea8-261">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-261">Number of previous passwords to block.</span></span> <span data-ttu-id="d4ea8-262">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="d4ea8-262">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d4ea8-263">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="d4ea8-263">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="d4ea8-264">Int32</span><span class="sxs-lookup"><span data-stu-id="d4ea8-264">Int32</span></span>|<span data-ttu-id="d4ea8-265">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-265">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="d4ea8-266">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="d4ea8-266">Valid values 1 to 16</span></span>|
|<span data-ttu-id="d4ea8-267">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d4ea8-267">passwordRequiredType</span></span>|[<span data-ttu-id="d4ea8-268">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d4ea8-268">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="d4ea8-269">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-269">Type of password that is required.</span></span> <span data-ttu-id="d4ea8-270">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-270">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="d4ea8-271">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d4ea8-271">passwordRequired</span></span>|<span data-ttu-id="d4ea8-272">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-272">Boolean</span></span>|<span data-ttu-id="d4ea8-273">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-273">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="d4ea8-274">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="d4ea8-274">powerOffBlocked</span></span>|<span data-ttu-id="d4ea8-275">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-275">Boolean</span></span>|<span data-ttu-id="d4ea8-276">Indica se o desligamento do dispositivo deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-276">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="d4ea8-277">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="d4ea8-277">factoryResetBlocked</span></span>|<span data-ttu-id="d4ea8-278">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-278">Boolean</span></span>|<span data-ttu-id="d4ea8-279">Indica se o usuário será ou não impedido de executar uma restauração de fábrica.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-279">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="d4ea8-280">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="d4ea8-280">screenCaptureBlocked</span></span>|<span data-ttu-id="d4ea8-281">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-281">Boolean</span></span>|<span data-ttu-id="d4ea8-282">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-282">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="d4ea8-283">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="d4ea8-283">deviceSharingAllowed</span></span>|<span data-ttu-id="d4ea8-284">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-284">Boolean</span></span>|<span data-ttu-id="d4ea8-285">Indica se o modo de compartilhamento do dispositivo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-285">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="d4ea8-286">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="d4ea8-286">storageBlockGoogleBackup</span></span>|<span data-ttu-id="d4ea8-287">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-287">Boolean</span></span>|<span data-ttu-id="d4ea8-288">Indica se o Backup do Google deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-288">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="d4ea8-289">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="d4ea8-289">storageBlockRemovableStorage</span></span>|<span data-ttu-id="d4ea8-290">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-290">Boolean</span></span>|<span data-ttu-id="d4ea8-291">Indica se o uso do armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-291">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="d4ea8-292">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="d4ea8-292">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="d4ea8-293">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-293">Boolean</span></span>|<span data-ttu-id="d4ea8-294">Indica se a criptografia do dispositivo é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-294">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="d4ea8-295">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="d4ea8-295">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="d4ea8-296">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-296">Boolean</span></span>|<span data-ttu-id="d4ea8-297">Indica se a criptografia do armazenamento removível é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-297">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="d4ea8-298">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="d4ea8-298">voiceAssistantBlocked</span></span>|<span data-ttu-id="d4ea8-299">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-299">Boolean</span></span>|<span data-ttu-id="d4ea8-300">Indica se o uso do Assistente de voz será ou não bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-300">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="d4ea8-301">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="d4ea8-301">voiceDialingBlocked</span></span>|<span data-ttu-id="d4ea8-302">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-302">Boolean</span></span>|<span data-ttu-id="d4ea8-303">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-303">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="d4ea8-304">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="d4ea8-304">webBrowserBlockPopups</span></span>|<span data-ttu-id="d4ea8-305">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-305">Boolean</span></span>|<span data-ttu-id="d4ea8-306">Indica se os pop-ups dentro do navegador da Web devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-306">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="d4ea8-307">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="d4ea8-307">webBrowserBlockAutofill</span></span>|<span data-ttu-id="d4ea8-308">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-308">Boolean</span></span>|<span data-ttu-id="d4ea8-309">Indica se o recurso de preenchimento automático do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-309">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="d4ea8-310">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="d4ea8-310">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="d4ea8-311">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-311">Boolean</span></span>|<span data-ttu-id="d4ea8-312">Indica se o JavaScript dentro do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-312">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="d4ea8-313">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="d4ea8-313">webBrowserBlocked</span></span>|<span data-ttu-id="d4ea8-314">Booliano</span><span class="sxs-lookup"><span data-stu-id="d4ea8-314">Boolean</span></span>|<span data-ttu-id="d4ea8-315">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-315">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="d4ea8-316">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d4ea8-316">webBrowserCookieSettings</span></span>|[<span data-ttu-id="d4ea8-317">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d4ea8-317">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="d4ea8-318">Configuração de cookies do navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-318">Cookie settings within the web browser.</span></span> <span data-ttu-id="d4ea8-319">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-319">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="d4ea8-320">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="d4ea8-320">wiFiBlocked</span></span>|<span data-ttu-id="d4ea8-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4ea8-321">Boolean</span></span>|<span data-ttu-id="d4ea8-322">Indica se a sincronização de Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-322">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="d4ea8-323">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="d4ea8-323">appsInstallAllowList</span></span>|<span data-ttu-id="d4ea8-324">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-324">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d4ea8-325">Lista de aplicativos que podem ser instalados no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-325">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="d4ea8-326">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-326">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d4ea8-327">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="d4ea8-327">appsLaunchBlockList</span></span>|<span data-ttu-id="d4ea8-328">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-328">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d4ea8-329">Lista de aplicativos que não podem ser abertos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-329">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="d4ea8-330">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-330">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d4ea8-331">appsHideList</span><span class="sxs-lookup"><span data-stu-id="d4ea8-331">appsHideList</span></span>|<span data-ttu-id="d4ea8-332">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d4ea8-332">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d4ea8-333">Lista de aplicativos que devem ficar ocultos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-333">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="d4ea8-334">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-334">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d4ea8-335">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="d4ea8-335">securityRequireVerifyApps</span></span>|<span data-ttu-id="d4ea8-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4ea8-336">Boolean</span></span>|<span data-ttu-id="d4ea8-337">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-337">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="d4ea8-338">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4ea8-338">Response</span></span>
<span data-ttu-id="d4ea8-339">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-339">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4ea8-340">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4ea8-340">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4ea8-341">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4ea8-341">Request</span></span>
<span data-ttu-id="d4ea8-342">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-342">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3934

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

### <a name="response"></a><span data-ttu-id="d4ea8-343">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4ea8-343">Response</span></span>
<span data-ttu-id="d4ea8-p125">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4ea8-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4106

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






