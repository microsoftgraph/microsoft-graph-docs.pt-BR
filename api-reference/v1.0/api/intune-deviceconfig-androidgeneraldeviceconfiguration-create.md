---
title: Criar androidGeneralDeviceConfiguration
description: Criar um novo objeto androidGeneralDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: 67bbdf997c2157c7e3161ee1c37a7cdf47ac2d25
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353750"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="fe83d-103">Criar androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="fe83d-103">Create androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="fe83d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fe83d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe83d-105">Criar um novo objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fe83d-105">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe83d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe83d-106">Prerequisites</span></span>
<span data-ttu-id="fe83d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe83d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe83d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe83d-109">Permission type</span></span>|<span data-ttu-id="fe83d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe83d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe83d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe83d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fe83d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe83d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe83d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe83d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe83d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe83d-114">Not supported.</span></span>|
|<span data-ttu-id="fe83d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe83d-115">Application</span></span>|<span data-ttu-id="fe83d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe83d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe83d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe83d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fe83d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe83d-118">Request headers</span></span>
|<span data-ttu-id="fe83d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe83d-119">Header</span></span>|<span data-ttu-id="fe83d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fe83d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe83d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe83d-121">Authorization</span></span>|<span data-ttu-id="fe83d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe83d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe83d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fe83d-123">Accept</span></span>|<span data-ttu-id="fe83d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fe83d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe83d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe83d-125">Request body</span></span>
<span data-ttu-id="fe83d-126">No corpo da solicitação, forneça uma representação JSON do objeto androidGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fe83d-126">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="fe83d-127">A tabela a seguir mostra as propriedades que são necessárias ao criar androidGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fe83d-127">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="fe83d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe83d-128">Property</span></span>|<span data-ttu-id="fe83d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe83d-129">Type</span></span>|<span data-ttu-id="fe83d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe83d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe83d-131">id</span><span class="sxs-lookup"><span data-stu-id="fe83d-131">id</span></span>|<span data-ttu-id="fe83d-132">String</span><span class="sxs-lookup"><span data-stu-id="fe83d-132">String</span></span>|<span data-ttu-id="fe83d-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fe83d-133">Key of the entity.</span></span> <span data-ttu-id="fe83d-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe83d-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe83d-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe83d-135">lastModifiedDateTime</span></span>|<span data-ttu-id="fe83d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe83d-136">DateTimeOffset</span></span>|<span data-ttu-id="fe83d-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="fe83d-137">DateTime the object was last modified.</span></span> <span data-ttu-id="fe83d-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe83d-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe83d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe83d-139">createdDateTime</span></span>|<span data-ttu-id="fe83d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe83d-140">DateTimeOffset</span></span>|<span data-ttu-id="fe83d-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-141">DateTime the object was created.</span></span> <span data-ttu-id="fe83d-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe83d-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe83d-143">description</span><span class="sxs-lookup"><span data-stu-id="fe83d-143">description</span></span>|<span data-ttu-id="fe83d-144">String</span><span class="sxs-lookup"><span data-stu-id="fe83d-144">String</span></span>|<span data-ttu-id="fe83d-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fe83d-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fe83d-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe83d-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe83d-147">displayName</span><span class="sxs-lookup"><span data-stu-id="fe83d-147">displayName</span></span>|<span data-ttu-id="fe83d-148">String</span><span class="sxs-lookup"><span data-stu-id="fe83d-148">String</span></span>|<span data-ttu-id="fe83d-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fe83d-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fe83d-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe83d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe83d-151">version</span><span class="sxs-lookup"><span data-stu-id="fe83d-151">version</span></span>|<span data-ttu-id="fe83d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="fe83d-152">Int32</span></span>|<span data-ttu-id="fe83d-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fe83d-153">Version of the device configuration.</span></span> <span data-ttu-id="fe83d-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fe83d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fe83d-155">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="fe83d-155">appsBlockClipboardSharing</span></span>|<span data-ttu-id="fe83d-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-156">Boolean</span></span>|<span data-ttu-id="fe83d-157">Indica se a função de copiar e colar entre aplicativos será bloqueada ou não no compartilhamento de área de transferência.</span><span class="sxs-lookup"><span data-stu-id="fe83d-157">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="fe83d-158">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="fe83d-158">appsBlockCopyPaste</span></span>|<span data-ttu-id="fe83d-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-159">Boolean</span></span>|<span data-ttu-id="fe83d-160">Indica se a função de copiar e colar dentro de aplicativos será bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="fe83d-160">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="fe83d-161">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="fe83d-161">appsBlockYouTube</span></span>|<span data-ttu-id="fe83d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-162">Boolean</span></span>|<span data-ttu-id="fe83d-163">Indica se o aplicativo YouTube deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-163">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="fe83d-164">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="fe83d-164">bluetoothBlocked</span></span>|<span data-ttu-id="fe83d-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-165">Boolean</span></span>|<span data-ttu-id="fe83d-166">Indica se o Bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-166">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="fe83d-167">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="fe83d-167">cameraBlocked</span></span>|<span data-ttu-id="fe83d-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-168">Boolean</span></span>|<span data-ttu-id="fe83d-169">Indica se o uso da câmera deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-169">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="fe83d-170">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="fe83d-170">cellularBlockDataRoaming</span></span>|<span data-ttu-id="fe83d-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-171">Boolean</span></span>|<span data-ttu-id="fe83d-172">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-172">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="fe83d-173">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="fe83d-173">cellularBlockMessaging</span></span>|<span data-ttu-id="fe83d-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-174">Boolean</span></span>|<span data-ttu-id="fe83d-175">Indica se as mensagens SMS/MMS devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="fe83d-175">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="fe83d-176">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="fe83d-176">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="fe83d-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-177">Boolean</span></span>|<span data-ttu-id="fe83d-178">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-178">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="fe83d-179">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="fe83d-179">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="fe83d-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-180">Boolean</span></span>|<span data-ttu-id="fe83d-181">Indica se a sincronização de compartilhamento de Internet por Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="fe83d-181">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="fe83d-182">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="fe83d-182">compliantAppsList</span></span>|<span data-ttu-id="fe83d-183">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="fe83d-183">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="fe83d-184">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="fe83d-184">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="fe83d-185">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="fe83d-185">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="fe83d-186">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="fe83d-186">compliantAppListType</span></span>|[<span data-ttu-id="fe83d-187">appListType</span><span class="sxs-lookup"><span data-stu-id="fe83d-187">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="fe83d-188">Tipo de lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="fe83d-188">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="fe83d-189">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="fe83d-189">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="fe83d-190">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="fe83d-190">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="fe83d-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-191">Boolean</span></span>|<span data-ttu-id="fe83d-192">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-192">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="fe83d-193">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="fe83d-193">locationServicesBlocked</span></span>|<span data-ttu-id="fe83d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-194">Boolean</span></span>|<span data-ttu-id="fe83d-195">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="fe83d-195">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="fe83d-196">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="fe83d-196">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="fe83d-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-197">Boolean</span></span>|<span data-ttu-id="fe83d-198">Indica se a sincronização automática da conta do Google deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="fe83d-198">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="fe83d-199">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="fe83d-199">googlePlayStoreBlocked</span></span>|<span data-ttu-id="fe83d-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-200">Boolean</span></span>|<span data-ttu-id="fe83d-201">Indica se a Google Play Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="fe83d-201">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="fe83d-202">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="fe83d-202">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="fe83d-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-203">Boolean</span></span>|<span data-ttu-id="fe83d-204">Indica se o botão de suspensão de tela deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="fe83d-204">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="fe83d-205">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="fe83d-205">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="fe83d-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-206">Boolean</span></span>|<span data-ttu-id="fe83d-207">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="fe83d-207">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="fe83d-208">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="fe83d-208">kioskModeApps</span></span>|<span data-ttu-id="fe83d-209">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="fe83d-209">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="fe83d-210">Uma lista de aplicativos que poderão ser executados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="fe83d-210">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="fe83d-211">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fe83d-211">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fe83d-212">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="fe83d-212">nfcBlocked</span></span>|<span data-ttu-id="fe83d-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-213">Boolean</span></span>|<span data-ttu-id="fe83d-214">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="fe83d-214">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="fe83d-215">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="fe83d-215">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="fe83d-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-216">Boolean</span></span>|<span data-ttu-id="fe83d-217">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-217">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="fe83d-218">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="fe83d-218">passwordBlockTrustAgents</span></span>|<span data-ttu-id="fe83d-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-219">Boolean</span></span>|<span data-ttu-id="fe83d-220">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="fe83d-220">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="fe83d-221">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fe83d-221">passwordExpirationDays</span></span>|<span data-ttu-id="fe83d-222">Int32</span><span class="sxs-lookup"><span data-stu-id="fe83d-222">Int32</span></span>|<span data-ttu-id="fe83d-223">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="fe83d-223">Number of days before the password expires.</span></span> <span data-ttu-id="fe83d-224">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="fe83d-224">Valid values 1 to 365</span></span>|
|<span data-ttu-id="fe83d-225">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fe83d-225">passwordMinimumLength</span></span>|<span data-ttu-id="fe83d-226">Int32</span><span class="sxs-lookup"><span data-stu-id="fe83d-226">Int32</span></span>|<span data-ttu-id="fe83d-227">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="fe83d-227">Minimum length of passwords.</span></span> <span data-ttu-id="fe83d-228">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="fe83d-228">Valid values 4 to 16</span></span>|
|<span data-ttu-id="fe83d-229">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="fe83d-229">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="fe83d-230">Int32</span><span class="sxs-lookup"><span data-stu-id="fe83d-230">Int32</span></span>|<span data-ttu-id="fe83d-231">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="fe83d-231">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="fe83d-232">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="fe83d-232">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="fe83d-233">Int32</span><span class="sxs-lookup"><span data-stu-id="fe83d-233">Int32</span></span>|<span data-ttu-id="fe83d-234">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="fe83d-234">Number of previous passwords to block.</span></span> <span data-ttu-id="fe83d-235">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="fe83d-235">Valid values 0 to 24</span></span>|
|<span data-ttu-id="fe83d-236">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="fe83d-236">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="fe83d-237">Int32</span><span class="sxs-lookup"><span data-stu-id="fe83d-237">Int32</span></span>|<span data-ttu-id="fe83d-238">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="fe83d-238">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="fe83d-239">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="fe83d-239">Valid values 4 to 11</span></span>|
|<span data-ttu-id="fe83d-240">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="fe83d-240">passwordRequiredType</span></span>|[<span data-ttu-id="fe83d-241">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="fe83d-241">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="fe83d-242">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="fe83d-242">Type of password that is required.</span></span> <span data-ttu-id="fe83d-243">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="fe83d-243">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="fe83d-244">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="fe83d-244">passwordRequired</span></span>|<span data-ttu-id="fe83d-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-245">Boolean</span></span>|<span data-ttu-id="fe83d-246">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="fe83d-246">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="fe83d-247">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="fe83d-247">powerOffBlocked</span></span>|<span data-ttu-id="fe83d-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-248">Boolean</span></span>|<span data-ttu-id="fe83d-249">Indica se o desligamento do dispositivo deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-249">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="fe83d-250">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="fe83d-250">factoryResetBlocked</span></span>|<span data-ttu-id="fe83d-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-251">Boolean</span></span>|<span data-ttu-id="fe83d-252">Indica se o usuário será ou não impedido de executar uma restauração de fábrica.</span><span class="sxs-lookup"><span data-stu-id="fe83d-252">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="fe83d-253">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="fe83d-253">screenCaptureBlocked</span></span>|<span data-ttu-id="fe83d-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-254">Boolean</span></span>|<span data-ttu-id="fe83d-255">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="fe83d-255">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="fe83d-256">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="fe83d-256">deviceSharingAllowed</span></span>|<span data-ttu-id="fe83d-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-257">Boolean</span></span>|<span data-ttu-id="fe83d-258">Indica se o modo de compartilhamento do dispositivo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="fe83d-258">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="fe83d-259">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="fe83d-259">storageBlockGoogleBackup</span></span>|<span data-ttu-id="fe83d-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-260">Boolean</span></span>|<span data-ttu-id="fe83d-261">Indica se o Backup do Google deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-261">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="fe83d-262">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="fe83d-262">storageBlockRemovableStorage</span></span>|<span data-ttu-id="fe83d-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-263">Boolean</span></span>|<span data-ttu-id="fe83d-264">Indica se o uso do armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-264">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="fe83d-265">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="fe83d-265">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="fe83d-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-266">Boolean</span></span>|<span data-ttu-id="fe83d-267">Indica se a criptografia do dispositivo é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="fe83d-267">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="fe83d-268">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="fe83d-268">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="fe83d-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-269">Boolean</span></span>|<span data-ttu-id="fe83d-270">Indica se a criptografia do armazenamento removível é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="fe83d-270">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="fe83d-271">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="fe83d-271">voiceAssistantBlocked</span></span>|<span data-ttu-id="fe83d-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-272">Boolean</span></span>|<span data-ttu-id="fe83d-273">Indica se o uso do Assistente de voz será ou não bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-273">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="fe83d-274">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="fe83d-274">voiceDialingBlocked</span></span>|<span data-ttu-id="fe83d-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-275">Boolean</span></span>|<span data-ttu-id="fe83d-276">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="fe83d-276">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="fe83d-277">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="fe83d-277">webBrowserBlockPopups</span></span>|<span data-ttu-id="fe83d-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-278">Boolean</span></span>|<span data-ttu-id="fe83d-279">Indica se os pop-ups dentro do navegador da Web devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="fe83d-279">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="fe83d-280">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="fe83d-280">webBrowserBlockAutofill</span></span>|<span data-ttu-id="fe83d-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-281">Boolean</span></span>|<span data-ttu-id="fe83d-282">Indica se o recurso de preenchimento automático do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-282">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="fe83d-283">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="fe83d-283">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="fe83d-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-284">Boolean</span></span>|<span data-ttu-id="fe83d-285">Indica se o JavaScript dentro do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-285">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="fe83d-286">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="fe83d-286">webBrowserBlocked</span></span>|<span data-ttu-id="fe83d-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-287">Boolean</span></span>|<span data-ttu-id="fe83d-288">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-288">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="fe83d-289">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="fe83d-289">webBrowserCookieSettings</span></span>|[<span data-ttu-id="fe83d-290">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="fe83d-290">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="fe83d-291">Configuração de cookies do navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="fe83d-291">Cookie settings within the web browser.</span></span> <span data-ttu-id="fe83d-292">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="fe83d-292">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="fe83d-293">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="fe83d-293">wiFiBlocked</span></span>|<span data-ttu-id="fe83d-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-294">Boolean</span></span>|<span data-ttu-id="fe83d-295">Indica se a sincronização de Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="fe83d-295">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="fe83d-296">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="fe83d-296">appsInstallAllowList</span></span>|<span data-ttu-id="fe83d-297">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="fe83d-297">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="fe83d-298">Lista de aplicativos que podem ser instalados no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="fe83d-298">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="fe83d-299">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fe83d-299">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fe83d-300">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="fe83d-300">appsLaunchBlockList</span></span>|<span data-ttu-id="fe83d-301">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="fe83d-301">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="fe83d-302">Lista de aplicativos que não podem ser abertos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="fe83d-302">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="fe83d-303">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fe83d-303">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fe83d-304">appsHideList</span><span class="sxs-lookup"><span data-stu-id="fe83d-304">appsHideList</span></span>|<span data-ttu-id="fe83d-305">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="fe83d-305">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="fe83d-306">Lista de aplicativos que devem ficar ocultos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="fe83d-306">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="fe83d-307">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="fe83d-307">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="fe83d-308">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="fe83d-308">securityRequireVerifyApps</span></span>|<span data-ttu-id="fe83d-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe83d-309">Boolean</span></span>|<span data-ttu-id="fe83d-310">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="fe83d-310">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="fe83d-311">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe83d-311">Response</span></span>
<span data-ttu-id="fe83d-312">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe83d-312">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe83d-313">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe83d-313">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe83d-314">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe83d-314">Request</span></span>
<span data-ttu-id="fe83d-315">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe83d-315">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="fe83d-316">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe83d-316">Response</span></span>
<span data-ttu-id="fe83d-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe83d-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



