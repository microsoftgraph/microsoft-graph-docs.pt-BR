---
title: Criar androidGeneralDeviceConfiguration
description: Criar um novo objeto androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f529c74d841daff02c508cd50db888f6d4a4f958
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976446"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="67a0b-103">Criar androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="67a0b-103">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="67a0b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67a0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67a0b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67a0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67a0b-106">Criar um novo objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="67a0b-106">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67a0b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67a0b-107">Prerequisites</span></span>
<span data-ttu-id="67a0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67a0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67a0b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67a0b-110">Permission type</span></span>|<span data-ttu-id="67a0b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67a0b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67a0b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67a0b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67a0b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a0b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67a0b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67a0b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67a0b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a0b-115">Not supported.</span></span>|
|<span data-ttu-id="67a0b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67a0b-116">Application</span></span>|<span data-ttu-id="67a0b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67a0b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67a0b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67a0b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="67a0b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67a0b-119">Request headers</span></span>
|<span data-ttu-id="67a0b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67a0b-120">Header</span></span>|<span data-ttu-id="67a0b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="67a0b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67a0b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="67a0b-122">Authorization</span></span>|<span data-ttu-id="67a0b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67a0b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67a0b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67a0b-124">Accept</span></span>|<span data-ttu-id="67a0b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67a0b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67a0b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67a0b-126">Request body</span></span>
<span data-ttu-id="67a0b-127">No corpo da solicitação, forneça uma representação JSON do objeto androidGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="67a0b-127">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="67a0b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="67a0b-128">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="67a0b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67a0b-129">Property</span></span>|<span data-ttu-id="67a0b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="67a0b-130">Type</span></span>|<span data-ttu-id="67a0b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="67a0b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67a0b-132">id</span><span class="sxs-lookup"><span data-stu-id="67a0b-132">id</span></span>|<span data-ttu-id="67a0b-133">String</span><span class="sxs-lookup"><span data-stu-id="67a0b-133">String</span></span>|<span data-ttu-id="67a0b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="67a0b-134">Key of the entity.</span></span> <span data-ttu-id="67a0b-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a0b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67a0b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="67a0b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67a0b-137">DateTimeOffset</span></span>|<span data-ttu-id="67a0b-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="67a0b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="67a0b-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a0b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67a0b-140">roleScopeTagIds</span></span>|<span data-ttu-id="67a0b-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="67a0b-141">String collection</span></span>|<span data-ttu-id="67a0b-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="67a0b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="67a0b-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a0b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="67a0b-144">supportsScopeTags</span></span>|<span data-ttu-id="67a0b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-145">Boolean</span></span>|<span data-ttu-id="67a0b-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="67a0b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="67a0b-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="67a0b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="67a0b-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="67a0b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="67a0b-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="67a0b-149">This property is read-only.</span></span> <span data-ttu-id="67a0b-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a0b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67a0b-151">createdDateTime</span></span>|<span data-ttu-id="67a0b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67a0b-152">DateTimeOffset</span></span>|<span data-ttu-id="67a0b-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-153">DateTime the object was created.</span></span> <span data-ttu-id="67a0b-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a0b-155">descrição</span><span class="sxs-lookup"><span data-stu-id="67a0b-155">description</span></span>|<span data-ttu-id="67a0b-156">String</span><span class="sxs-lookup"><span data-stu-id="67a0b-156">String</span></span>|<span data-ttu-id="67a0b-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67a0b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="67a0b-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a0b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="67a0b-159">displayName</span></span>|<span data-ttu-id="67a0b-160">String</span><span class="sxs-lookup"><span data-stu-id="67a0b-160">String</span></span>|<span data-ttu-id="67a0b-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67a0b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="67a0b-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a0b-163">versão</span><span class="sxs-lookup"><span data-stu-id="67a0b-163">version</span></span>|<span data-ttu-id="67a0b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="67a0b-164">Int32</span></span>|<span data-ttu-id="67a0b-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="67a0b-165">Version of the device configuration.</span></span> <span data-ttu-id="67a0b-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67a0b-167">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="67a0b-167">appsBlockClipboardSharing</span></span>|<span data-ttu-id="67a0b-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-168">Boolean</span></span>|<span data-ttu-id="67a0b-169">Indica se a função de copiar e colar entre aplicativos será bloqueada ou não no compartilhamento de área de transferência.</span><span class="sxs-lookup"><span data-stu-id="67a0b-169">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="67a0b-170">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="67a0b-170">appsBlockCopyPaste</span></span>|<span data-ttu-id="67a0b-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-171">Boolean</span></span>|<span data-ttu-id="67a0b-172">Indica se a função de copiar e colar dentro de aplicativos será bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="67a0b-172">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="67a0b-173">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="67a0b-173">appsBlockYouTube</span></span>|<span data-ttu-id="67a0b-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-174">Boolean</span></span>|<span data-ttu-id="67a0b-175">Indica se o aplicativo YouTube deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-175">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="67a0b-176">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="67a0b-176">bluetoothBlocked</span></span>|<span data-ttu-id="67a0b-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-177">Boolean</span></span>|<span data-ttu-id="67a0b-178">Indica se o Bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-178">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="67a0b-179">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="67a0b-179">cameraBlocked</span></span>|<span data-ttu-id="67a0b-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-180">Boolean</span></span>|<span data-ttu-id="67a0b-181">Indica se o uso da câmera deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-181">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="67a0b-182">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="67a0b-182">cellularBlockDataRoaming</span></span>|<span data-ttu-id="67a0b-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-183">Boolean</span></span>|<span data-ttu-id="67a0b-184">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-184">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="67a0b-185">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="67a0b-185">cellularBlockMessaging</span></span>|<span data-ttu-id="67a0b-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-186">Boolean</span></span>|<span data-ttu-id="67a0b-187">Indica se as mensagens SMS/MMS devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="67a0b-187">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="67a0b-188">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="67a0b-188">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="67a0b-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-189">Boolean</span></span>|<span data-ttu-id="67a0b-190">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-190">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="67a0b-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="67a0b-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="67a0b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-192">Boolean</span></span>|<span data-ttu-id="67a0b-193">Indica se a sincronização de compartilhamento de Internet por Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="67a0b-193">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="67a0b-194">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="67a0b-194">compliantAppsList</span></span>|<span data-ttu-id="67a0b-195">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-195">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="67a0b-196">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="67a0b-196">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="67a0b-197">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="67a0b-197">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="67a0b-198">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="67a0b-198">compliantAppListType</span></span>|[<span data-ttu-id="67a0b-199">appListType</span><span class="sxs-lookup"><span data-stu-id="67a0b-199">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="67a0b-200">Tipo de lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="67a0b-200">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="67a0b-201">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="67a0b-201">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="67a0b-202">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="67a0b-202">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="67a0b-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-203">Boolean</span></span>|<span data-ttu-id="67a0b-204">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-204">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="67a0b-205">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="67a0b-205">locationServicesBlocked</span></span>|<span data-ttu-id="67a0b-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-206">Boolean</span></span>|<span data-ttu-id="67a0b-207">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="67a0b-207">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="67a0b-208">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="67a0b-208">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="67a0b-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-209">Boolean</span></span>|<span data-ttu-id="67a0b-210">Indica se a sincronização automática da conta do Google deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="67a0b-210">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="67a0b-211">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="67a0b-211">googlePlayStoreBlocked</span></span>|<span data-ttu-id="67a0b-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-212">Boolean</span></span>|<span data-ttu-id="67a0b-213">Indica se a Google Play Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="67a0b-213">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="67a0b-214">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="67a0b-214">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="67a0b-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-215">Boolean</span></span>|<span data-ttu-id="67a0b-216">Indica se o botão de suspensão de tela deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="67a0b-216">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="67a0b-217">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="67a0b-217">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="67a0b-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-218">Boolean</span></span>|<span data-ttu-id="67a0b-219">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="67a0b-219">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="67a0b-220">dateAndTimeBlockChanges</span><span class="sxs-lookup"><span data-stu-id="67a0b-220">dateAndTimeBlockChanges</span></span>|<span data-ttu-id="67a0b-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-221">Boolean</span></span>|<span data-ttu-id="67a0b-222">Indica se a data e a hora de alteração serão bloqueadas ou não no modo do KNOX.</span><span class="sxs-lookup"><span data-stu-id="67a0b-222">Indicates whether or not to block changing date and time while in KNOX Mode.</span></span>|
|<span data-ttu-id="67a0b-223">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="67a0b-223">kioskModeApps</span></span>|<span data-ttu-id="67a0b-224">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-224">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="67a0b-225">Uma lista de aplicativos que poderão ser executados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="67a0b-225">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="67a0b-226">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="67a0b-226">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="67a0b-227">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="67a0b-227">nfcBlocked</span></span>|<span data-ttu-id="67a0b-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-228">Boolean</span></span>|<span data-ttu-id="67a0b-229">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="67a0b-229">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="67a0b-230">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="67a0b-230">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="67a0b-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-231">Boolean</span></span>|<span data-ttu-id="67a0b-232">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-232">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="67a0b-233">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="67a0b-233">passwordBlockTrustAgents</span></span>|<span data-ttu-id="67a0b-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-234">Boolean</span></span>|<span data-ttu-id="67a0b-235">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="67a0b-235">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="67a0b-236">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="67a0b-236">passwordExpirationDays</span></span>|<span data-ttu-id="67a0b-237">Int32</span><span class="sxs-lookup"><span data-stu-id="67a0b-237">Int32</span></span>|<span data-ttu-id="67a0b-238">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="67a0b-238">Number of days before the password expires.</span></span> <span data-ttu-id="67a0b-239">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="67a0b-239">Valid values 1 to 365</span></span>|
|<span data-ttu-id="67a0b-240">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="67a0b-240">passwordMinimumLength</span></span>|<span data-ttu-id="67a0b-241">Int32</span><span class="sxs-lookup"><span data-stu-id="67a0b-241">Int32</span></span>|<span data-ttu-id="67a0b-242">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="67a0b-242">Minimum length of passwords.</span></span> <span data-ttu-id="67a0b-243">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="67a0b-243">Valid values 4 to 16</span></span>|
|<span data-ttu-id="67a0b-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="67a0b-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="67a0b-245">Int32</span><span class="sxs-lookup"><span data-stu-id="67a0b-245">Int32</span></span>|<span data-ttu-id="67a0b-246">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="67a0b-246">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="67a0b-247">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="67a0b-247">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="67a0b-248">Int32</span><span class="sxs-lookup"><span data-stu-id="67a0b-248">Int32</span></span>|<span data-ttu-id="67a0b-249">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="67a0b-249">Number of previous passwords to block.</span></span> <span data-ttu-id="67a0b-250">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="67a0b-250">Valid values 0 to 24</span></span>|
|<span data-ttu-id="67a0b-251">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="67a0b-251">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="67a0b-252">Int32</span><span class="sxs-lookup"><span data-stu-id="67a0b-252">Int32</span></span>|<span data-ttu-id="67a0b-253">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="67a0b-253">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="67a0b-254">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="67a0b-254">Valid values 1 to 16</span></span>|
|<span data-ttu-id="67a0b-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="67a0b-255">passwordRequiredType</span></span>|[<span data-ttu-id="67a0b-256">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="67a0b-256">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="67a0b-257">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="67a0b-257">Type of password that is required.</span></span> <span data-ttu-id="67a0b-258">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="67a0b-258">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="67a0b-259">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="67a0b-259">passwordRequired</span></span>|<span data-ttu-id="67a0b-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-260">Boolean</span></span>|<span data-ttu-id="67a0b-261">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="67a0b-261">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="67a0b-262">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="67a0b-262">powerOffBlocked</span></span>|<span data-ttu-id="67a0b-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-263">Boolean</span></span>|<span data-ttu-id="67a0b-264">Indica se o desligamento do dispositivo deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-264">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="67a0b-265">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="67a0b-265">factoryResetBlocked</span></span>|<span data-ttu-id="67a0b-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-266">Boolean</span></span>|<span data-ttu-id="67a0b-267">Indica se o usuário será ou não impedido de executar uma restauração de fábrica.</span><span class="sxs-lookup"><span data-stu-id="67a0b-267">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="67a0b-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="67a0b-268">screenCaptureBlocked</span></span>|<span data-ttu-id="67a0b-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-269">Boolean</span></span>|<span data-ttu-id="67a0b-270">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="67a0b-270">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="67a0b-271">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="67a0b-271">deviceSharingAllowed</span></span>|<span data-ttu-id="67a0b-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-272">Boolean</span></span>|<span data-ttu-id="67a0b-273">Indica se o modo de compartilhamento do dispositivo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="67a0b-273">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="67a0b-274">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="67a0b-274">storageBlockGoogleBackup</span></span>|<span data-ttu-id="67a0b-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-275">Boolean</span></span>|<span data-ttu-id="67a0b-276">Indica se o Backup do Google deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-276">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="67a0b-277">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="67a0b-277">storageBlockRemovableStorage</span></span>|<span data-ttu-id="67a0b-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-278">Boolean</span></span>|<span data-ttu-id="67a0b-279">Indica se o uso do armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-279">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="67a0b-280">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="67a0b-280">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="67a0b-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-281">Boolean</span></span>|<span data-ttu-id="67a0b-282">Indica se a criptografia do dispositivo é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="67a0b-282">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="67a0b-283">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="67a0b-283">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="67a0b-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-284">Boolean</span></span>|<span data-ttu-id="67a0b-285">Indica se a criptografia do armazenamento removível é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="67a0b-285">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="67a0b-286">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="67a0b-286">voiceAssistantBlocked</span></span>|<span data-ttu-id="67a0b-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-287">Boolean</span></span>|<span data-ttu-id="67a0b-288">Indica se o uso do Assistente de voz será ou não bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-288">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="67a0b-289">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="67a0b-289">voiceDialingBlocked</span></span>|<span data-ttu-id="67a0b-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-290">Boolean</span></span>|<span data-ttu-id="67a0b-291">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="67a0b-291">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="67a0b-292">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="67a0b-292">webBrowserBlockPopups</span></span>|<span data-ttu-id="67a0b-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-293">Boolean</span></span>|<span data-ttu-id="67a0b-294">Indica se os pop-ups dentro do navegador da Web devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="67a0b-294">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="67a0b-295">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="67a0b-295">webBrowserBlockAutofill</span></span>|<span data-ttu-id="67a0b-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-296">Boolean</span></span>|<span data-ttu-id="67a0b-297">Indica se o recurso de preenchimento automático do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-297">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="67a0b-298">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="67a0b-298">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="67a0b-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-299">Boolean</span></span>|<span data-ttu-id="67a0b-300">Indica se o JavaScript dentro do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-300">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="67a0b-301">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="67a0b-301">webBrowserBlocked</span></span>|<span data-ttu-id="67a0b-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-302">Boolean</span></span>|<span data-ttu-id="67a0b-303">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-303">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="67a0b-304">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="67a0b-304">webBrowserCookieSettings</span></span>|[<span data-ttu-id="67a0b-305">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="67a0b-305">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="67a0b-306">Configuração de cookies do navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="67a0b-306">Cookie settings within the web browser.</span></span> <span data-ttu-id="67a0b-307">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="67a0b-307">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="67a0b-308">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="67a0b-308">wiFiBlocked</span></span>|<span data-ttu-id="67a0b-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-309">Boolean</span></span>|<span data-ttu-id="67a0b-310">Indica se a sincronização de Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="67a0b-310">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="67a0b-311">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="67a0b-311">appsInstallAllowList</span></span>|<span data-ttu-id="67a0b-312">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-312">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="67a0b-313">Lista de aplicativos que podem ser instalados no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="67a0b-313">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="67a0b-314">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="67a0b-314">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="67a0b-315">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="67a0b-315">appsLaunchBlockList</span></span>|<span data-ttu-id="67a0b-316">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-316">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="67a0b-317">Lista de aplicativos que não podem ser abertos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="67a0b-317">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="67a0b-318">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="67a0b-318">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="67a0b-319">appsHideList</span><span class="sxs-lookup"><span data-stu-id="67a0b-319">appsHideList</span></span>|<span data-ttu-id="67a0b-320">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="67a0b-320">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="67a0b-321">Lista de aplicativos que devem ficar ocultos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="67a0b-321">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="67a0b-322">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="67a0b-322">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="67a0b-323">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="67a0b-323">securityRequireVerifyApps</span></span>|<span data-ttu-id="67a0b-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a0b-324">Boolean</span></span>|<span data-ttu-id="67a0b-325">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="67a0b-325">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="67a0b-326">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a0b-326">Response</span></span>
<span data-ttu-id="67a0b-327">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67a0b-327">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67a0b-328">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67a0b-328">Example</span></span>

### <a name="request"></a><span data-ttu-id="67a0b-329">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67a0b-329">Request</span></span>
<span data-ttu-id="67a0b-330">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67a0b-330">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3161

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="67a0b-331">Resposta</span><span class="sxs-lookup"><span data-stu-id="67a0b-331">Response</span></span>
<span data-ttu-id="67a0b-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67a0b-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3333

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




