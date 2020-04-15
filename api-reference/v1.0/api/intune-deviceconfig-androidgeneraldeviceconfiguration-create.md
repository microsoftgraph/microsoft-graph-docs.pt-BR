---
title: Criar androidGeneralDeviceConfiguration
description: Criar um novo objeto androidGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 942fb299ca42a5d60947bb6b2261950b4a21dd2a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474653"
---
# <a name="create-androidgeneraldeviceconfiguration"></a><span data-ttu-id="05c04-103">Criar androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="05c04-103">Create androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="05c04-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05c04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05c04-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="05c04-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05c04-106">Criar um novo objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="05c04-106">Create a new [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05c04-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="05c04-107">Prerequisites</span></span>
<span data-ttu-id="05c04-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05c04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05c04-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05c04-110">Permission type</span></span>|<span data-ttu-id="05c04-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="05c04-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05c04-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05c04-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05c04-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05c04-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05c04-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05c04-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05c04-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05c04-115">Not supported.</span></span>|
|<span data-ttu-id="05c04-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05c04-116">Application</span></span>|<span data-ttu-id="05c04-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05c04-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05c04-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05c04-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="05c04-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05c04-119">Request headers</span></span>
|<span data-ttu-id="05c04-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="05c04-120">Header</span></span>|<span data-ttu-id="05c04-121">Valor</span><span class="sxs-lookup"><span data-stu-id="05c04-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05c04-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="05c04-122">Authorization</span></span>|<span data-ttu-id="05c04-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="05c04-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05c04-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="05c04-124">Accept</span></span>|<span data-ttu-id="05c04-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05c04-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05c04-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05c04-126">Request body</span></span>
<span data-ttu-id="05c04-127">No corpo da solicitação, forneça uma representação JSON do objeto androidGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="05c04-127">In the request body, supply a JSON representation for the androidGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="05c04-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="05c04-128">The following table shows the properties that are required when you create the androidGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="05c04-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05c04-129">Property</span></span>|<span data-ttu-id="05c04-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="05c04-130">Type</span></span>|<span data-ttu-id="05c04-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="05c04-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05c04-132">id</span><span class="sxs-lookup"><span data-stu-id="05c04-132">id</span></span>|<span data-ttu-id="05c04-133">String</span><span class="sxs-lookup"><span data-stu-id="05c04-133">String</span></span>|<span data-ttu-id="05c04-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="05c04-134">Key of the entity.</span></span> <span data-ttu-id="05c04-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05c04-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05c04-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05c04-136">lastModifiedDateTime</span></span>|<span data-ttu-id="05c04-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05c04-137">DateTimeOffset</span></span>|<span data-ttu-id="05c04-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="05c04-138">DateTime the object was last modified.</span></span> <span data-ttu-id="05c04-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05c04-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05c04-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05c04-140">createdDateTime</span></span>|<span data-ttu-id="05c04-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05c04-141">DateTimeOffset</span></span>|<span data-ttu-id="05c04-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="05c04-142">DateTime the object was created.</span></span> <span data-ttu-id="05c04-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05c04-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05c04-144">description</span><span class="sxs-lookup"><span data-stu-id="05c04-144">description</span></span>|<span data-ttu-id="05c04-145">String</span><span class="sxs-lookup"><span data-stu-id="05c04-145">String</span></span>|<span data-ttu-id="05c04-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05c04-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="05c04-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05c04-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05c04-148">displayName</span><span class="sxs-lookup"><span data-stu-id="05c04-148">displayName</span></span>|<span data-ttu-id="05c04-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="05c04-149">String</span></span>|<span data-ttu-id="05c04-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05c04-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="05c04-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05c04-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05c04-152">versão</span><span class="sxs-lookup"><span data-stu-id="05c04-152">version</span></span>|<span data-ttu-id="05c04-153">Int32</span><span class="sxs-lookup"><span data-stu-id="05c04-153">Int32</span></span>|<span data-ttu-id="05c04-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="05c04-154">Version of the device configuration.</span></span> <span data-ttu-id="05c04-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="05c04-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05c04-156">appsBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="05c04-156">appsBlockClipboardSharing</span></span>|<span data-ttu-id="05c04-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-157">Boolean</span></span>|<span data-ttu-id="05c04-158">Indica se a função de copiar e colar entre aplicativos será bloqueada ou não no compartilhamento de área de transferência.</span><span class="sxs-lookup"><span data-stu-id="05c04-158">Indicates whether or not to block clipboard sharing to copy and paste between applications.</span></span>|
|<span data-ttu-id="05c04-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="05c04-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="05c04-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-160">Boolean</span></span>|<span data-ttu-id="05c04-161">Indica se a função de copiar e colar dentro de aplicativos será bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="05c04-161">Indicates whether or not to block copy and paste within applications.</span></span>|
|<span data-ttu-id="05c04-162">appsBlockYouTube</span><span class="sxs-lookup"><span data-stu-id="05c04-162">appsBlockYouTube</span></span>|<span data-ttu-id="05c04-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-163">Boolean</span></span>|<span data-ttu-id="05c04-164">Indica se o aplicativo YouTube deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-164">Indicates whether or not to block the YouTube app.</span></span>|
|<span data-ttu-id="05c04-165">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="05c04-165">bluetoothBlocked</span></span>|<span data-ttu-id="05c04-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-166">Boolean</span></span>|<span data-ttu-id="05c04-167">Indica se o Bluetooth deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-167">Indicates whether or not to block Bluetooth.</span></span>|
|<span data-ttu-id="05c04-168">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="05c04-168">cameraBlocked</span></span>|<span data-ttu-id="05c04-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-169">Boolean</span></span>|<span data-ttu-id="05c04-170">Indica se o uso da câmera deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-170">Indicates whether or not to block the use of the camera.</span></span>|
|<span data-ttu-id="05c04-171">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="05c04-171">cellularBlockDataRoaming</span></span>|<span data-ttu-id="05c04-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-172">Boolean</span></span>|<span data-ttu-id="05c04-173">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-173">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="05c04-174">cellularBlockMessaging</span><span class="sxs-lookup"><span data-stu-id="05c04-174">cellularBlockMessaging</span></span>|<span data-ttu-id="05c04-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-175">Boolean</span></span>|<span data-ttu-id="05c04-176">Indica se as mensagens SMS/MMS devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="05c04-176">Indicates whether or not to block SMS/MMS messaging.</span></span>|
|<span data-ttu-id="05c04-177">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="05c04-177">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="05c04-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-178">Boolean</span></span>|<span data-ttu-id="05c04-179">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-179">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="05c04-180">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="05c04-180">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="05c04-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-181">Boolean</span></span>|<span data-ttu-id="05c04-182">Indica se a sincronização de compartilhamento de Internet por Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="05c04-182">Indicates whether or not to block syncing Wi-Fi tethering.</span></span>|
|<span data-ttu-id="05c04-183">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="05c04-183">compliantAppsList</span></span>|<span data-ttu-id="05c04-184">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="05c04-184">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="05c04-185">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="05c04-185">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="05c04-186">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="05c04-186">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="05c04-187">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="05c04-187">compliantAppListType</span></span>|[<span data-ttu-id="05c04-188">appListType</span><span class="sxs-lookup"><span data-stu-id="05c04-188">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="05c04-189">Tipo de lista que está em CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="05c04-189">Type of list that is in the CompliantAppsList.</span></span> <span data-ttu-id="05c04-190">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="05c04-190">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="05c04-191">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="05c04-191">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="05c04-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-192">Boolean</span></span>|<span data-ttu-id="05c04-193">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-193">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="05c04-194">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="05c04-194">locationServicesBlocked</span></span>|<span data-ttu-id="05c04-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-195">Boolean</span></span>|<span data-ttu-id="05c04-196">Indica se os serviços de localização devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="05c04-196">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="05c04-197">googleAccountBlockAutoSync</span><span class="sxs-lookup"><span data-stu-id="05c04-197">googleAccountBlockAutoSync</span></span>|<span data-ttu-id="05c04-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-198">Boolean</span></span>|<span data-ttu-id="05c04-199">Indica se a sincronização automática da conta do Google deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="05c04-199">Indicates whether or not to block Google account auto sync.</span></span>|
|<span data-ttu-id="05c04-200">googlePlayStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="05c04-200">googlePlayStoreBlocked</span></span>|<span data-ttu-id="05c04-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-201">Boolean</span></span>|<span data-ttu-id="05c04-202">Indica se a Google Play Store deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="05c04-202">Indicates whether or not to block the Google Play store.</span></span>|
|<span data-ttu-id="05c04-203">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="05c04-203">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="05c04-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-204">Boolean</span></span>|<span data-ttu-id="05c04-205">Indica se o botão de suspensão de tela deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="05c04-205">Indicates whether or not to block the screen sleep button while in Kiosk Mode.</span></span>|
|<span data-ttu-id="05c04-206">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="05c04-206">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="05c04-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-207">Boolean</span></span>|<span data-ttu-id="05c04-208">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="05c04-208">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="05c04-209">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="05c04-209">kioskModeApps</span></span>|<span data-ttu-id="05c04-210">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="05c04-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="05c04-211">Uma lista de aplicativos que poderão ser executados quando o dispositivo estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="05c04-211">A list of apps that will be allowed to run when the device is in Kiosk Mode.</span></span> <span data-ttu-id="05c04-212">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="05c04-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="05c04-213">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="05c04-213">nfcBlocked</span></span>|<span data-ttu-id="05c04-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-214">Boolean</span></span>|<span data-ttu-id="05c04-215">Indica se a comunicação a curta distância deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="05c04-215">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="05c04-216">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="05c04-216">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="05c04-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-217">Boolean</span></span>|<span data-ttu-id="05c04-218">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-218">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="05c04-219">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="05c04-219">passwordBlockTrustAgents</span></span>|<span data-ttu-id="05c04-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="05c04-220">Boolean</span></span>|<span data-ttu-id="05c04-221">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="05c04-221">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="05c04-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="05c04-222">passwordExpirationDays</span></span>|<span data-ttu-id="05c04-223">Int32</span><span class="sxs-lookup"><span data-stu-id="05c04-223">Int32</span></span>|<span data-ttu-id="05c04-224">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="05c04-224">Number of days before the password expires.</span></span> <span data-ttu-id="05c04-225">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="05c04-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="05c04-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="05c04-226">passwordMinimumLength</span></span>|<span data-ttu-id="05c04-227">Int32</span><span class="sxs-lookup"><span data-stu-id="05c04-227">Int32</span></span>|<span data-ttu-id="05c04-228">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="05c04-228">Minimum length of passwords.</span></span> <span data-ttu-id="05c04-229">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="05c04-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="05c04-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="05c04-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="05c04-231">Int32</span><span class="sxs-lookup"><span data-stu-id="05c04-231">Int32</span></span>|<span data-ttu-id="05c04-232">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="05c04-232">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="05c04-233">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="05c04-233">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="05c04-234">Int32</span><span class="sxs-lookup"><span data-stu-id="05c04-234">Int32</span></span>|<span data-ttu-id="05c04-235">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="05c04-235">Number of previous passwords to block.</span></span> <span data-ttu-id="05c04-236">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="05c04-236">Valid values 0 to 24</span></span>|
|<span data-ttu-id="05c04-237">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="05c04-237">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="05c04-238">Int32</span><span class="sxs-lookup"><span data-stu-id="05c04-238">Int32</span></span>|<span data-ttu-id="05c04-239">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="05c04-239">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="05c04-240">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="05c04-240">Valid values 1 to 16</span></span>|
|<span data-ttu-id="05c04-241">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="05c04-241">passwordRequiredType</span></span>|[<span data-ttu-id="05c04-242">androidRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="05c04-242">androidRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidrequiredpasswordtype.md)|<span data-ttu-id="05c04-243">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="05c04-243">Type of password that is required.</span></span> <span data-ttu-id="05c04-244">Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span><span class="sxs-lookup"><span data-stu-id="05c04-244">Possible values are: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.</span></span>|
|<span data-ttu-id="05c04-245">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="05c04-245">passwordRequired</span></span>|<span data-ttu-id="05c04-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-246">Boolean</span></span>|<span data-ttu-id="05c04-247">Indica se uma senha deve ou não ser exigida.</span><span class="sxs-lookup"><span data-stu-id="05c04-247">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="05c04-248">powerOffBlocked</span><span class="sxs-lookup"><span data-stu-id="05c04-248">powerOffBlocked</span></span>|<span data-ttu-id="05c04-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-249">Boolean</span></span>|<span data-ttu-id="05c04-250">Indica se o desligamento do dispositivo deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-250">Indicates whether or not to block powering off the device.</span></span>|
|<span data-ttu-id="05c04-251">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="05c04-251">factoryResetBlocked</span></span>|<span data-ttu-id="05c04-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-252">Boolean</span></span>|<span data-ttu-id="05c04-253">Indica se o usuário será ou não impedido de executar uma restauração de fábrica.</span><span class="sxs-lookup"><span data-stu-id="05c04-253">Indicates whether or not to block user performing a factory reset.</span></span>|
|<span data-ttu-id="05c04-254">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="05c04-254">screenCaptureBlocked</span></span>|<span data-ttu-id="05c04-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-255">Boolean</span></span>|<span data-ttu-id="05c04-256">Indica se capturas de tela devem ou não ser bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="05c04-256">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="05c04-257">deviceSharingAllowed</span><span class="sxs-lookup"><span data-stu-id="05c04-257">deviceSharingAllowed</span></span>|<span data-ttu-id="05c04-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-258">Boolean</span></span>|<span data-ttu-id="05c04-259">Indica se o modo de compartilhamento do dispositivo deve ou não ser permitido.</span><span class="sxs-lookup"><span data-stu-id="05c04-259">Indicates whether or not to allow device sharing mode.</span></span>|
|<span data-ttu-id="05c04-260">storageBlockGoogleBackup</span><span class="sxs-lookup"><span data-stu-id="05c04-260">storageBlockGoogleBackup</span></span>|<span data-ttu-id="05c04-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-261">Boolean</span></span>|<span data-ttu-id="05c04-262">Indica se o Backup do Google deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-262">Indicates whether or not to block Google Backup.</span></span>|
|<span data-ttu-id="05c04-263">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="05c04-263">storageBlockRemovableStorage</span></span>|<span data-ttu-id="05c04-264">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-264">Boolean</span></span>|<span data-ttu-id="05c04-265">Indica se o uso do armazenamento removível deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-265">Indicates whether or not to block removable storage usage.</span></span>|
|<span data-ttu-id="05c04-266">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="05c04-266">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="05c04-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-267">Boolean</span></span>|<span data-ttu-id="05c04-268">Indica se a criptografia do dispositivo é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="05c04-268">Indicates whether or not to require device encryption.</span></span>|
|<span data-ttu-id="05c04-269">storageRequireRemovableStorageEncryption</span><span class="sxs-lookup"><span data-stu-id="05c04-269">storageRequireRemovableStorageEncryption</span></span>|<span data-ttu-id="05c04-270">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-270">Boolean</span></span>|<span data-ttu-id="05c04-271">Indica se a criptografia do armazenamento removível é ou não necessária.</span><span class="sxs-lookup"><span data-stu-id="05c04-271">Indicates whether or not to require removable storage encryption.</span></span>|
|<span data-ttu-id="05c04-272">voiceAssistantBlocked</span><span class="sxs-lookup"><span data-stu-id="05c04-272">voiceAssistantBlocked</span></span>|<span data-ttu-id="05c04-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-273">Boolean</span></span>|<span data-ttu-id="05c04-274">Indica se o uso do Assistente de voz será ou não bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-274">Indicates whether or not to block the use of the Voice Assistant.</span></span>|
|<span data-ttu-id="05c04-275">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="05c04-275">voiceDialingBlocked</span></span>|<span data-ttu-id="05c04-276">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-276">Boolean</span></span>|<span data-ttu-id="05c04-277">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="05c04-277">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="05c04-278">webBrowserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="05c04-278">webBrowserBlockPopups</span></span>|<span data-ttu-id="05c04-279">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-279">Boolean</span></span>|<span data-ttu-id="05c04-280">Indica se os pop-ups dentro do navegador da Web devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="05c04-280">Indicates whether or not to block popups within the web browser.</span></span>|
|<span data-ttu-id="05c04-281">webBrowserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="05c04-281">webBrowserBlockAutofill</span></span>|<span data-ttu-id="05c04-282">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-282">Boolean</span></span>|<span data-ttu-id="05c04-283">Indica se o recurso de preenchimento automático do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-283">Indicates whether or not to block the web browser's auto fill feature.</span></span>|
|<span data-ttu-id="05c04-284">webBrowserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="05c04-284">webBrowserBlockJavaScript</span></span>|<span data-ttu-id="05c04-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-285">Boolean</span></span>|<span data-ttu-id="05c04-286">Indica se o JavaScript dentro do navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-286">Indicates whether or not to block JavaScript within the web browser.</span></span>|
|<span data-ttu-id="05c04-287">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="05c04-287">webBrowserBlocked</span></span>|<span data-ttu-id="05c04-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-288">Boolean</span></span>|<span data-ttu-id="05c04-289">Indica se o navegador da Web deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="05c04-289">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="05c04-290">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="05c04-290">webBrowserCookieSettings</span></span>|[<span data-ttu-id="05c04-291">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="05c04-291">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="05c04-292">Configuração de cookies do navegador da Web.</span><span class="sxs-lookup"><span data-stu-id="05c04-292">Cookie settings within the web browser.</span></span> <span data-ttu-id="05c04-293">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="05c04-293">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="05c04-294">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="05c04-294">wiFiBlocked</span></span>|<span data-ttu-id="05c04-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="05c04-295">Boolean</span></span>|<span data-ttu-id="05c04-296">Indica se a sincronização de Wi-Fi deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="05c04-296">Indicates whether or not to block syncing Wi-Fi.</span></span>|
|<span data-ttu-id="05c04-297">appsInstallAllowList</span><span class="sxs-lookup"><span data-stu-id="05c04-297">appsInstallAllowList</span></span>|<span data-ttu-id="05c04-298">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="05c04-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="05c04-299">Lista de aplicativos que podem ser instalados no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="05c04-299">List of apps which can be installed on the KNOX device.</span></span> <span data-ttu-id="05c04-300">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="05c04-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="05c04-301">appsLaunchBlockList</span><span class="sxs-lookup"><span data-stu-id="05c04-301">appsLaunchBlockList</span></span>|<span data-ttu-id="05c04-302">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="05c04-302">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="05c04-303">Lista de aplicativos que não podem ser abertos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="05c04-303">List of apps which are blocked from being launched on the KNOX device.</span></span> <span data-ttu-id="05c04-304">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="05c04-304">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="05c04-305">appsHideList</span><span class="sxs-lookup"><span data-stu-id="05c04-305">appsHideList</span></span>|<span data-ttu-id="05c04-306">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="05c04-306">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="05c04-307">Lista de aplicativos que devem ficar ocultos no dispositivo KNOX.</span><span class="sxs-lookup"><span data-stu-id="05c04-307">List of apps to be hidden on the KNOX device.</span></span> <span data-ttu-id="05c04-308">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="05c04-308">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="05c04-309">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="05c04-309">securityRequireVerifyApps</span></span>|<span data-ttu-id="05c04-310">Booliano</span><span class="sxs-lookup"><span data-stu-id="05c04-310">Boolean</span></span>|<span data-ttu-id="05c04-311">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="05c04-311">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="05c04-312">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c04-312">Response</span></span>
<span data-ttu-id="05c04-313">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05c04-313">If successful, this method returns a `201 Created` response code and a [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05c04-314">Exemplo</span><span class="sxs-lookup"><span data-stu-id="05c04-314">Example</span></span>

### <a name="request"></a><span data-ttu-id="05c04-315">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05c04-315">Request</span></span>
<span data-ttu-id="05c04-316">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="05c04-316">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05c04-317">Resposta</span><span class="sxs-lookup"><span data-stu-id="05c04-317">Response</span></span>
<span data-ttu-id="05c04-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05c04-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






