---
title: Atualizar androidGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto androidGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce4bbbe2074bba753d32a7aa8d293282cd320ded
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757217"
---
# <a name="update-androidgeneraldeviceconfiguration"></a><span data-ttu-id="63ac0-103">Atualizar androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="63ac0-103">Update androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="63ac0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63ac0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63ac0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63ac0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63ac0-106">Atualizar as propriedades de um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63ac0-106">Update the properties of a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63ac0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63ac0-107">Prerequisites</span></span>
<span data-ttu-id="63ac0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63ac0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63ac0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63ac0-110">Permission type</span></span>|<span data-ttu-id="63ac0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63ac0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63ac0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63ac0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63ac0-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63ac0-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="63ac0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63ac0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63ac0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63ac0-115">Not supported.</span></span>|
|<span data-ttu-id="63ac0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63ac0-116">Application</span></span>|<span data-ttu-id="63ac0-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63ac0-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="63ac0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63ac0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="63ac0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63ac0-119">Request headers</span></span>
|<span data-ttu-id="63ac0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63ac0-120">Header</span></span>|<span data-ttu-id="63ac0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="63ac0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63ac0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63ac0-122">Authorization</span></span>|<span data-ttu-id="63ac0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63ac0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63ac0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63ac0-124">Accept</span></span>|<span data-ttu-id="63ac0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63ac0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63ac0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63ac0-126">Request body</span></span>
<span data-ttu-id="63ac0-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63ac0-127">In the request body, supply a JSON representation for the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="63ac0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="63ac0-128">The following table shows the properties that are required when you create the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="63ac0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63ac0-129">Property</span></span>|<span data-ttu-id="63ac0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="63ac0-130">Type</span></span>|<span data-ttu-id="63ac0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="63ac0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63ac0-132">id</span><span class="sxs-lookup"><span data-stu-id="63ac0-132">id</span></span>|<span data-ttu-id="63ac0-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63ac0-133">String</span></span>|<span data-ttu-id="63ac0-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="63ac0-134">Key of the entity.</span></span> <span data-ttu-id="63ac0-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ac0-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63ac0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63ac0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="63ac0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63ac0-137">DateTimeOffset</span></span>|<span data-ttu-id="63ac0-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="63ac0-138">DateTime the object was last modified.</span></span> <span data-ttu-id="63ac0-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ac0-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63ac0-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63ac0-140">createdDateTime</span></span>|<span data-ttu-id="63ac0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63ac0-141">DateTimeOffset</span></span>|<span data-ttu-id="63ac0-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-142">DateTime the object was created.</span></span> <span data-ttu-id="63ac0-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ac0-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63ac0-144">descrição</span><span class="sxs-lookup"><span data-stu-id="63ac0-144">description</span></span>|<span data-ttu-id="63ac0-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63ac0-145">String</span></span>|<span data-ttu-id="63ac0-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63ac0-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="63ac0-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ac0-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63ac0-148">displayName</span><span class="sxs-lookup"><span data-stu-id="63ac0-148">displayName</span></span>|<span data-ttu-id="63ac0-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63ac0-149">String</span></span>|<span data-ttu-id="63ac0-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63ac0-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="63ac0-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ac0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63ac0-152">versão</span><span class="sxs-lookup"><span data-stu-id="63ac0-152">version</span></span>|<span data-ttu-id="63ac0-153">Int32</span><span class="sxs-lookup"><span data-stu-id="63ac0-153">Int32</span></span>|<span data-ttu-id="63ac0-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="63ac0-154">Version of the device configuration.</span></span> <span data-ttu-id="63ac0-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="63ac0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="63ac0-156">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="63ac0-156">appsBlockClipboardSharing</span></span>|<span data-ttu-id="63ac0-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-157">Boolean</span></span>|<span data-ttu-id="63ac0-158">Indica se a função de copiar e colar entre aplicativos será bloqueada ou não no compartilhamento de área de transferência.</span><span class="sxs-lookup"><span data-stu-id="63ac0-158">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="63ac0-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="63ac0-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="63ac0-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-160">Boolean</span></span>|<span data-ttu-id="63ac0-161">Indica se a função de copiar e colar dentro de aplicativos será bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="63ac0-161">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="63ac0-162">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="63ac0-162">appsBlockYouTube</span></span>|<span data-ttu-id="63ac0-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-163">Boolean</span></span>|<span data-ttu-id="63ac0-164">Indica se o aplicativo YouTube deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-164">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="63ac0-165">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="63ac0-165">bluetoothBlocked</span></span>|<span data-ttu-id="63ac0-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-166">Boolean</span></span>|<span data-ttu-id="63ac0-167">Indica se o Bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-167">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="63ac0-168">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="63ac0-168">cameraBlocked</span></span>|<span data-ttu-id="63ac0-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-169">Boolean</span></span>|<span data-ttu-id="63ac0-170">Indica se o uso da câmera deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-170">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="63ac0-171">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="63ac0-171">cellularBlockDataRoaming</span></span>|<span data-ttu-id="63ac0-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-172">Boolean</span></span>|<span data-ttu-id="63ac0-173">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-173">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="63ac0-174">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="63ac0-174">cellularBlockMessaging</span></span>|<span data-ttu-id="63ac0-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-175">Boolean</span></span>|<span data-ttu-id="63ac0-176">Indica se as mensagens SMS/MMS devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="63ac0-176">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="63ac0-177">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="63ac0-177">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="63ac0-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-178">Boolean</span></span>|<span data-ttu-id="63ac0-179">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-179">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="63ac0-180">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="63ac0-180">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="63ac0-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-181">Boolean</span></span>|<span data-ttu-id="63ac0-182">Indica se a sincronização de compartilhamento de Internet por Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="63ac0-182">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="63ac0-183">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="63ac0-183">compliantAppsList</span></span>|<span data-ttu-id="63ac0-184">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="63ac0-184">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="63ac0-185">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="63ac0-185">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="63ac0-186">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="63ac0-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="63ac0-187">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="63ac0-187">compliantAppListType</span></span>|[<span data-ttu-id="63ac0-188">appListType</span><span class="sxs-lookup"><span data-stu-id="63ac0-188">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="63ac0-189">Tipo de lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="63ac0-189">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="63ac0-190">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="63ac0-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="63ac0-191">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="63ac0-191">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="63ac0-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-192">Boolean</span></span>|<span data-ttu-id="63ac0-193">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-193">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="63ac0-194">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="63ac0-194">locationServicesBlocked</span></span>|<span data-ttu-id="63ac0-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-195">Boolean</span></span>|<span data-ttu-id="63ac0-196">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="63ac0-196">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="63ac0-197">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="63ac0-197">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="63ac0-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-198">Boolean</span></span>|<span data-ttu-id="63ac0-199">Indica se a sincronização automática da conta do Google deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="63ac0-199">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="63ac0-200">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="63ac0-200">googlePlayStoreBlocked</span></span>|<span data-ttu-id="63ac0-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-201">Boolean</span></span>|<span data-ttu-id="63ac0-202">Indica se a Google Play Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="63ac0-202">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="63ac0-203">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="63ac0-203">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="63ac0-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-204">Boolean</span></span>|<span data-ttu-id="63ac0-205">Indica se o botão de suspensão de tela deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63ac0-205">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="63ac0-206">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="63ac0-206">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="63ac0-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-207">Boolean</span></span>|<span data-ttu-id="63ac0-208">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63ac0-208">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="63ac0-209">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="63ac0-209">kioskModeApps</span></span>|<span data-ttu-id="63ac0-210">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="63ac0-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="63ac0-211">Uma lista de aplicativos que poderão ser executados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="63ac0-211">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="63ac0-212">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="63ac0-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="63ac0-213">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="63ac0-213">nfcBlocked</span></span>|<span data-ttu-id="63ac0-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-214">Boolean</span></span>|<span data-ttu-id="63ac0-215">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="63ac0-215">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="63ac0-216">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="63ac0-216">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="63ac0-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-217">Boolean</span></span>|<span data-ttu-id="63ac0-218">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-218">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="63ac0-219">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="63ac0-219">passwordBlockTrustAgents</span></span>|<span data-ttu-id="63ac0-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-220">Boolean</span></span>|<span data-ttu-id="63ac0-221">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="63ac0-221">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="63ac0-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="63ac0-222">passwordExpirationDays</span></span>|<span data-ttu-id="63ac0-223">Int32</span><span class="sxs-lookup"><span data-stu-id="63ac0-223">Int32</span></span>|<span data-ttu-id="63ac0-224">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="63ac0-224">Number of days before the password expires.</span></span> <span data-ttu-id="63ac0-225">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="63ac0-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="63ac0-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="63ac0-226">passwordMinimumLength</span></span>|<span data-ttu-id="63ac0-227">Int32</span><span class="sxs-lookup"><span data-stu-id="63ac0-227">Int32</span></span>|<span data-ttu-id="63ac0-228">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="63ac0-228">Minimum length of passwords.</span></span> <span data-ttu-id="63ac0-229">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="63ac0-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="63ac0-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="63ac0-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="63ac0-231">Int32</span><span class="sxs-lookup"><span data-stu-id="63ac0-231">Int32</span></span>|<span data-ttu-id="63ac0-232">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="63ac0-232">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="63ac0-233">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="63ac0-233">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="63ac0-234">Int32</span><span class="sxs-lookup"><span data-stu-id="63ac0-234">Int32</span></span>|<span data-ttu-id="63ac0-235">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="63ac0-235">Number of previous passwords to block.</span></span> <span data-ttu-id="63ac0-236">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="63ac0-236">Valid values 0 to 24</span></span>|
|<span data-ttu-id="63ac0-237">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="63ac0-237">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="63ac0-238">Int32</span><span class="sxs-lookup"><span data-stu-id="63ac0-238">Int32</span></span>|<span data-ttu-id="63ac0-239">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="63ac0-239">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="63ac0-240">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="63ac0-240">Valid values 1 to 16</span></span>|
|<span data-ttu-id="63ac0-241">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="63ac0-241">passwordRequiredType</span></span>|[<span data-ttu-id="63ac0-242">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="63ac0-242">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="63ac0-243">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="63ac0-243">Type of password that is required.</span></span> <span data-ttu-id="63ac0-244">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="63ac0-244">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="63ac0-245">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="63ac0-245">passwordRequired</span></span>|<span data-ttu-id="63ac0-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-246">Boolean</span></span>|<span data-ttu-id="63ac0-247">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="63ac0-247">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="63ac0-248">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="63ac0-248">powerOffBlocked</span></span>|<span data-ttu-id="63ac0-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-249">Boolean</span></span>|<span data-ttu-id="63ac0-250">Indica se o desligamento do dispositivo deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-250">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="63ac0-251">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="63ac0-251">factoryResetBlocked</span></span>|<span data-ttu-id="63ac0-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-252">Boolean</span></span>|<span data-ttu-id="63ac0-253">Indica se o usuário será ou não impedido de executar uma restauração de fábrica.</span><span class="sxs-lookup"><span data-stu-id="63ac0-253">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="63ac0-254">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="63ac0-254">screenCaptureBlocked</span></span>|<span data-ttu-id="63ac0-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-255">Boolean</span></span>|<span data-ttu-id="63ac0-256">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="63ac0-256">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="63ac0-257">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="63ac0-257">deviceSharingAllowed</span></span>|<span data-ttu-id="63ac0-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-258">Boolean</span></span>|<span data-ttu-id="63ac0-259">Indica se o modo de compartilhamento do dispositivo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="63ac0-259">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="63ac0-260">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="63ac0-260">storageBlockGoogleBackup</span></span>|<span data-ttu-id="63ac0-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-261">Boolean</span></span>|<span data-ttu-id="63ac0-262">Indica se o Backup do Google deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-262">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="63ac0-263">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="63ac0-263">storageBlockRemovableStorage</span></span>|<span data-ttu-id="63ac0-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-264">Boolean</span></span>|<span data-ttu-id="63ac0-265">Indica se o uso do armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-265">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="63ac0-266">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="63ac0-266">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="63ac0-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-267">Boolean</span></span>|<span data-ttu-id="63ac0-268">Indica se a criptografia do dispositivo é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="63ac0-268">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="63ac0-269">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="63ac0-269">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="63ac0-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-270">Boolean</span></span>|<span data-ttu-id="63ac0-271">Indica se a criptografia do armazenamento removível é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="63ac0-271">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="63ac0-272">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="63ac0-272">voiceAssistantBlocked</span></span>|<span data-ttu-id="63ac0-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-273">Boolean</span></span>|<span data-ttu-id="63ac0-274">Indica se o uso do Assistente de voz será ou não bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-274">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="63ac0-275">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="63ac0-275">voiceDialingBlocked</span></span>|<span data-ttu-id="63ac0-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-276">Boolean</span></span>|<span data-ttu-id="63ac0-277">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="63ac0-277">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="63ac0-278">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="63ac0-278">webBrowserBlockPopups</span></span>|<span data-ttu-id="63ac0-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-279">Boolean</span></span>|<span data-ttu-id="63ac0-280">Indica se os pop-ups dentro do navegador da Web devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="63ac0-280">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="63ac0-281">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="63ac0-281">webBrowserBlockAutofill</span></span>|<span data-ttu-id="63ac0-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-282">Boolean</span></span>|<span data-ttu-id="63ac0-283">Indica se o recurso de preenchimento automático do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-283">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="63ac0-284">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="63ac0-284">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="63ac0-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-285">Boolean</span></span>|<span data-ttu-id="63ac0-286">Indica se o JavaScript dentro do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-286">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="63ac0-287">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="63ac0-287">webBrowserBlocked</span></span>|<span data-ttu-id="63ac0-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-288">Boolean</span></span>|<span data-ttu-id="63ac0-289">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-289">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="63ac0-290">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="63ac0-290">webBrowserCookieSettings</span></span>|[<span data-ttu-id="63ac0-291">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="63ac0-291">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="63ac0-292">Configuração de cookies do navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="63ac0-292">Cookie settings within the web browser.</span></span> <span data-ttu-id="63ac0-293">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="63ac0-293">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="63ac0-294">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="63ac0-294">wiFiBlocked</span></span>|<span data-ttu-id="63ac0-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-295">Boolean</span></span>|<span data-ttu-id="63ac0-296">Indica se a sincronização de Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="63ac0-296">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="63ac0-297">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="63ac0-297">appsInstallAllowList</span></span>|<span data-ttu-id="63ac0-298">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="63ac0-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="63ac0-299">Lista de aplicativos que podem ser instalados no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="63ac0-299">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="63ac0-300">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="63ac0-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="63ac0-301">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="63ac0-301">appsLaunchBlockList</span></span>|<span data-ttu-id="63ac0-302">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="63ac0-302">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="63ac0-303">Lista de aplicativos que não podem ser abertos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="63ac0-303">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="63ac0-304">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="63ac0-304">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="63ac0-305">appsHideList</span><span class="sxs-lookup"><span data-stu-id="63ac0-305">appsHideList</span></span>|<span data-ttu-id="63ac0-306">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="63ac0-306">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="63ac0-307">Lista de aplicativos que devem ficar ocultos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="63ac0-307">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="63ac0-308">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="63ac0-308">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="63ac0-309">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="63ac0-309">securityRequireVerifyApps</span></span>|<span data-ttu-id="63ac0-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="63ac0-310">Boolean</span></span>|<span data-ttu-id="63ac0-311">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="63ac0-311">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="63ac0-312">Resposta</span><span class="sxs-lookup"><span data-stu-id="63ac0-312">Response</span></span>
<span data-ttu-id="63ac0-313">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63ac0-313">If successful, this method returns a `200 OK` response code and an updated [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63ac0-314">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63ac0-314">Example</span></span>

### <a name="request"></a><span data-ttu-id="63ac0-315">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63ac0-315">Request</span></span>
<span data-ttu-id="63ac0-316">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63ac0-316">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3033

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="63ac0-317">Resposta</span><span class="sxs-lookup"><span data-stu-id="63ac0-317">Response</span></span>
<span data-ttu-id="63ac0-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63ac0-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3205

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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




