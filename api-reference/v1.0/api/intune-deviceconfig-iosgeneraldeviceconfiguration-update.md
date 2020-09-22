---
title: Atualizar iosGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec04dfc86a64c9ec8e8c89b2dfa6a63b2af23148
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979081"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="166cd-103">Atualizar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="166cd-103">Update iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="166cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="166cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="166cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="166cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="166cd-106">Atualizar as propriedades de um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="166cd-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="166cd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="166cd-107">Prerequisites</span></span>
<span data-ttu-id="166cd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="166cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="166cd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="166cd-110">Permission type</span></span>|<span data-ttu-id="166cd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="166cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="166cd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="166cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="166cd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="166cd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="166cd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="166cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="166cd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="166cd-115">Not supported.</span></span>|
|<span data-ttu-id="166cd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="166cd-116">Application</span></span>|<span data-ttu-id="166cd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="166cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="166cd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="166cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="166cd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="166cd-119">Request headers</span></span>
|<span data-ttu-id="166cd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="166cd-120">Header</span></span>|<span data-ttu-id="166cd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="166cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="166cd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="166cd-122">Authorization</span></span>|<span data-ttu-id="166cd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="166cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="166cd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="166cd-124">Accept</span></span>|<span data-ttu-id="166cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="166cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="166cd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="166cd-126">Request body</span></span>
<span data-ttu-id="166cd-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="166cd-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="166cd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="166cd-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="166cd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="166cd-129">Property</span></span>|<span data-ttu-id="166cd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="166cd-130">Type</span></span>|<span data-ttu-id="166cd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="166cd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="166cd-132">id</span><span class="sxs-lookup"><span data-stu-id="166cd-132">id</span></span>|<span data-ttu-id="166cd-133">String</span><span class="sxs-lookup"><span data-stu-id="166cd-133">String</span></span>|<span data-ttu-id="166cd-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="166cd-134">Key of the entity.</span></span> <span data-ttu-id="166cd-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="166cd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="166cd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="166cd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="166cd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="166cd-137">DateTimeOffset</span></span>|<span data-ttu-id="166cd-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="166cd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="166cd-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="166cd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="166cd-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="166cd-140">createdDateTime</span></span>|<span data-ttu-id="166cd-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="166cd-141">DateTimeOffset</span></span>|<span data-ttu-id="166cd-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="166cd-142">DateTime the object was created.</span></span> <span data-ttu-id="166cd-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="166cd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="166cd-144">description</span><span class="sxs-lookup"><span data-stu-id="166cd-144">description</span></span>|<span data-ttu-id="166cd-145">String</span><span class="sxs-lookup"><span data-stu-id="166cd-145">String</span></span>|<span data-ttu-id="166cd-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="166cd-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="166cd-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="166cd-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="166cd-148">displayName</span><span class="sxs-lookup"><span data-stu-id="166cd-148">displayName</span></span>|<span data-ttu-id="166cd-149">String</span><span class="sxs-lookup"><span data-stu-id="166cd-149">String</span></span>|<span data-ttu-id="166cd-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="166cd-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="166cd-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="166cd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="166cd-152">versão</span><span class="sxs-lookup"><span data-stu-id="166cd-152">version</span></span>|<span data-ttu-id="166cd-153">Int32</span><span class="sxs-lookup"><span data-stu-id="166cd-153">Int32</span></span>|<span data-ttu-id="166cd-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="166cd-154">Version of the device configuration.</span></span> <span data-ttu-id="166cd-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="166cd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="166cd-156">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="166cd-156">accountBlockModification</span></span>|<span data-ttu-id="166cd-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-157">Boolean</span></span>|<span data-ttu-id="166cd-158">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-158">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="166cd-159">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="166cd-159">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="166cd-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-160">Boolean</span></span>|<span data-ttu-id="166cd-161">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-161">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="166cd-162">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-162">airDropBlocked</span></span>|<span data-ttu-id="166cd-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-163">Boolean</span></span>|<span data-ttu-id="166cd-164">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-164">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="166cd-165">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="166cd-165">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="166cd-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-166">Boolean</span></span>|<span data-ttu-id="166cd-167">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-167">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="166cd-168">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="166cd-168">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="166cd-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-169">Boolean</span></span>|<span data-ttu-id="166cd-170">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="166cd-170">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="166cd-171">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="166cd-171">appleWatchBlockPairing</span></span>|<span data-ttu-id="166cd-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-172">Boolean</span></span>|<span data-ttu-id="166cd-173">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-173">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="166cd-174">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="166cd-174">appleWatchForceWristDetection</span></span>|<span data-ttu-id="166cd-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-175">Boolean</span></span>|<span data-ttu-id="166cd-176">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-176">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="166cd-177">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-177">appleNewsBlocked</span></span>|<span data-ttu-id="166cd-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-178">Boolean</span></span>|<span data-ttu-id="166cd-179">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-179">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="166cd-180">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="166cd-180">appsSingleAppModeList</span></span>|<span data-ttu-id="166cd-181">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="166cd-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="166cd-182">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="166cd-182">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="166cd-183">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-183">Supervised only.</span></span> <span data-ttu-id="166cd-184">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="166cd-184">iOS 7.0 and later.</span></span> <span data-ttu-id="166cd-185">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="166cd-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="166cd-186">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="166cd-186">appsVisibilityList</span></span>|<span data-ttu-id="166cd-187">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="166cd-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="166cd-188">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-188">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="166cd-189">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="166cd-189">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="166cd-190">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="166cd-190">appsVisibilityListType</span></span>|[<span data-ttu-id="166cd-191">appListType</span><span class="sxs-lookup"><span data-stu-id="166cd-191">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="166cd-192">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="166cd-192">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="166cd-193">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="166cd-193">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="166cd-194">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="166cd-194">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="166cd-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-195">Boolean</span></span>|<span data-ttu-id="166cd-196">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-196">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="166cd-197">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-197">appStoreBlocked</span></span>|<span data-ttu-id="166cd-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-198">Boolean</span></span>|<span data-ttu-id="166cd-199">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="166cd-199">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="166cd-200">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="166cd-200">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="166cd-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-201">Boolean</span></span>|<span data-ttu-id="166cd-202">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="166cd-202">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="166cd-203">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="166cd-203">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="166cd-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-204">Boolean</span></span>|<span data-ttu-id="166cd-205">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="166cd-205">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="166cd-206">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-206">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="166cd-207">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="166cd-207">appStoreRequirePassword</span></span>|<span data-ttu-id="166cd-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-208">Boolean</span></span>|<span data-ttu-id="166cd-209">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="166cd-209">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="166cd-210">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="166cd-210">bluetoothBlockModification</span></span>|<span data-ttu-id="166cd-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-211">Boolean</span></span>|<span data-ttu-id="166cd-212">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-212">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="166cd-213">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-213">cameraBlocked</span></span>|<span data-ttu-id="166cd-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-214">Boolean</span></span>|<span data-ttu-id="166cd-215">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="166cd-215">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="166cd-216">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="166cd-216">cellularBlockDataRoaming</span></span>|<span data-ttu-id="166cd-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-217">Boolean</span></span>|<span data-ttu-id="166cd-218">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="166cd-218">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="166cd-219">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="166cd-219">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="166cd-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-220">Boolean</span></span>|<span data-ttu-id="166cd-221">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="166cd-221">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="166cd-222">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="166cd-222">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="166cd-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-223">Boolean</span></span>|<span data-ttu-id="166cd-224">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-224">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="166cd-225">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="166cd-225">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="166cd-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-226">Boolean</span></span>|<span data-ttu-id="166cd-227">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="166cd-227">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="166cd-228">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="166cd-228">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="166cd-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-229">Boolean</span></span>|<span data-ttu-id="166cd-230">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="166cd-230">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="166cd-231">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="166cd-231">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="166cd-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-232">Boolean</span></span>|<span data-ttu-id="166cd-233">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="166cd-233">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="166cd-234">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="166cd-234">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="166cd-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-235">Boolean</span></span>|<span data-ttu-id="166cd-236">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-236">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="166cd-237">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="166cd-237">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="166cd-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-238">Boolean</span></span>|<span data-ttu-id="166cd-239">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-239">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="166cd-240">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="166cd-240">compliantAppsList</span></span>|<span data-ttu-id="166cd-241">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="166cd-241">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="166cd-242">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="166cd-242">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="166cd-243">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="166cd-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="166cd-244">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="166cd-244">compliantAppListType</span></span>|[<span data-ttu-id="166cd-245">appListType</span><span class="sxs-lookup"><span data-stu-id="166cd-245">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="166cd-246">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="166cd-246">List that is in the AppComplianceList.</span></span> <span data-ttu-id="166cd-247">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="166cd-247">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="166cd-248">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="166cd-248">configurationProfileBlockChanges</span></span>|<span data-ttu-id="166cd-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-249">Boolean</span></span>|<span data-ttu-id="166cd-250">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-250">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="166cd-251">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-251">definitionLookupBlocked</span></span>|<span data-ttu-id="166cd-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-252">Boolean</span></span>|<span data-ttu-id="166cd-253">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-253">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="166cd-254">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="166cd-254">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="166cd-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-255">Boolean</span></span>|<span data-ttu-id="166cd-256">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-256">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="166cd-257">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="166cd-257">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="166cd-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-258">Boolean</span></span>|<span data-ttu-id="166cd-259">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-259">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="166cd-260">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="166cd-260">deviceBlockNameModification</span></span>|<span data-ttu-id="166cd-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-261">Boolean</span></span>|<span data-ttu-id="166cd-262">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-262">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="166cd-263">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="166cd-263">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="166cd-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-264">Boolean</span></span>|<span data-ttu-id="166cd-265">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="166cd-265">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="166cd-266">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="166cd-266">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="166cd-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-267">Boolean</span></span>|<span data-ttu-id="166cd-268">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-268">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="166cd-269">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="166cd-269">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="166cd-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-270">Boolean</span></span>|<span data-ttu-id="166cd-271">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="166cd-271">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="166cd-272">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="166cd-272">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="166cd-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-273">Boolean</span></span>|<span data-ttu-id="166cd-274">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="166cd-274">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="166cd-275">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="166cd-275">emailInDomainSuffixes</span></span>|<span data-ttu-id="166cd-276">String collection</span><span class="sxs-lookup"><span data-stu-id="166cd-276">String collection</span></span>|<span data-ttu-id="166cd-277">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="166cd-277">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="166cd-278">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="166cd-278">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="166cd-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-279">Boolean</span></span>|<span data-ttu-id="166cd-280">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="166cd-280">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="166cd-281">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="166cd-281">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="166cd-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-282">Boolean</span></span>|<span data-ttu-id="166cd-283">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="166cd-283">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="166cd-284">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-284">faceTimeBlocked</span></span>|<span data-ttu-id="166cd-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-285">Boolean</span></span>|<span data-ttu-id="166cd-286">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="166cd-286">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="166cd-287">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-287">findMyFriendsBlocked</span></span>|<span data-ttu-id="166cd-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-288">Boolean</span></span>|<span data-ttu-id="166cd-289">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-289">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="166cd-290">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="166cd-290">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="166cd-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-291">Boolean</span></span>|<span data-ttu-id="166cd-292">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="166cd-292">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="166cd-293">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="166cd-293">gamingBlockMultiplayer</span></span>|<span data-ttu-id="166cd-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-294">Boolean</span></span>|<span data-ttu-id="166cd-295">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="166cd-295">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="166cd-296">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-296">gameCenterBlocked</span></span>|<span data-ttu-id="166cd-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-297">Boolean</span></span>|<span data-ttu-id="166cd-298">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-298">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="166cd-299">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-299">hostPairingBlocked</span></span>|<span data-ttu-id="166cd-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-300">Boolean</span></span>|<span data-ttu-id="166cd-301">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-301">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="166cd-302">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-302">iBooksStoreBlocked</span></span>|<span data-ttu-id="166cd-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-303">Boolean</span></span>|<span data-ttu-id="166cd-304">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-304">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="166cd-305">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="166cd-305">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="166cd-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-306">Boolean</span></span>|<span data-ttu-id="166cd-307">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="166cd-307">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="166cd-308">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="166cd-308">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="166cd-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-309">Boolean</span></span>|<span data-ttu-id="166cd-310">Indica se o usuário será ou não impedido de continuar o trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="166cd-310">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="166cd-311">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="166cd-311">iCloudBlockBackup</span></span>|<span data-ttu-id="166cd-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-312">Boolean</span></span>|<span data-ttu-id="166cd-313">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="166cd-313">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="166cd-314">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="166cd-314">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="166cd-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-315">Boolean</span></span>|<span data-ttu-id="166cd-316">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="166cd-316">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="166cd-317">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="166cd-317">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="166cd-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-318">Boolean</span></span>|<span data-ttu-id="166cd-319">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="166cd-319">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="166cd-320">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="166cd-320">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="166cd-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-321">Boolean</span></span>|<span data-ttu-id="166cd-322">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="166cd-322">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="166cd-323">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="166cd-323">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="166cd-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-324">Boolean</span></span>|<span data-ttu-id="166cd-325">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="166cd-325">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="166cd-326">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="166cd-326">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="166cd-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-327">Boolean</span></span>|<span data-ttu-id="166cd-328">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="166cd-328">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="166cd-329">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="166cd-329">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="166cd-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-330">Boolean</span></span>|<span data-ttu-id="166cd-331">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="166cd-331">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="166cd-332">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="166cd-332">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="166cd-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-333">Boolean</span></span>|<span data-ttu-id="166cd-334">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="166cd-334">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="166cd-335">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="166cd-335">iTunesBlockMusicService</span></span>|<span data-ttu-id="166cd-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-336">Boolean</span></span>|<span data-ttu-id="166cd-337">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-337">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="166cd-338">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="166cd-338">iTunesBlockRadio</span></span>|<span data-ttu-id="166cd-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-339">Boolean</span></span>|<span data-ttu-id="166cd-340">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-340">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="166cd-341">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="166cd-341">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="166cd-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-342">Boolean</span></span>|<span data-ttu-id="166cd-343">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-343">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="166cd-344">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="166cd-344">keyboardBlockDictation</span></span>|<span data-ttu-id="166cd-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-345">Boolean</span></span>|<span data-ttu-id="166cd-346">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-346">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="166cd-347">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="166cd-347">keyboardBlockPredictive</span></span>|<span data-ttu-id="166cd-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-348">Boolean</span></span>|<span data-ttu-id="166cd-349">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-349">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="166cd-350">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="166cd-350">keyboardBlockShortcuts</span></span>|<span data-ttu-id="166cd-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-351">Boolean</span></span>|<span data-ttu-id="166cd-352">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-352">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="166cd-353">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="166cd-353">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="166cd-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-354">Boolean</span></span>|<span data-ttu-id="166cd-355">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-355">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="166cd-356">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="166cd-356">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="166cd-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-357">Boolean</span></span>|<span data-ttu-id="166cd-358">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-358">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-359">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="166cd-359">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="166cd-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-360">Boolean</span></span>|<span data-ttu-id="166cd-361">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-361">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-362">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="166cd-362">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="166cd-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-363">Boolean</span></span>|<span data-ttu-id="166cd-364">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-364">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-365">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="166cd-365">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="166cd-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-366">Boolean</span></span>|<span data-ttu-id="166cd-367">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-367">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-368">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="166cd-368">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="166cd-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-369">Boolean</span></span>|<span data-ttu-id="166cd-370">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-370">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-371">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="166cd-371">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="166cd-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-372">Boolean</span></span>|<span data-ttu-id="166cd-373">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-373">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-374">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="166cd-374">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="166cd-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-375">Boolean</span></span>|<span data-ttu-id="166cd-376">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-376">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-377">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="166cd-377">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="166cd-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-378">Boolean</span></span>|<span data-ttu-id="166cd-379">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-379">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-380">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="166cd-380">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="166cd-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-381">Boolean</span></span>|<span data-ttu-id="166cd-382">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-382">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-383">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="166cd-383">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="166cd-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-384">Boolean</span></span>|<span data-ttu-id="166cd-385">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-385">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-386">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="166cd-386">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="166cd-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-387">Boolean</span></span>|<span data-ttu-id="166cd-388">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-388">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-389">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="166cd-389">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="166cd-390">String</span><span class="sxs-lookup"><span data-stu-id="166cd-390">String</span></span>|<span data-ttu-id="166cd-391">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-391">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="166cd-392">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="166cd-392">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="166cd-393">Propriedadekioskmodebuiltinappid</span><span class="sxs-lookup"><span data-stu-id="166cd-393">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="166cd-394">String</span><span class="sxs-lookup"><span data-stu-id="166cd-394">String</span></span>|<span data-ttu-id="166cd-395">ID para aplicativos internos a serem usados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-395">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="166cd-396">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidos.</span><span class="sxs-lookup"><span data-stu-id="166cd-396">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="166cd-397">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="166cd-397">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="166cd-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-398">Boolean</span></span>|<span data-ttu-id="166cd-399">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-399">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-400">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="166cd-400">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="166cd-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-401">Boolean</span></span>|<span data-ttu-id="166cd-402">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-402">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-403">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="166cd-403">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="166cd-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-404">Boolean</span></span>|<span data-ttu-id="166cd-405">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-405">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-406">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="166cd-406">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="166cd-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-407">Boolean</span></span>|<span data-ttu-id="166cd-408">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-408">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-409">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="166cd-409">kioskModeRequireZoom</span></span>|<span data-ttu-id="166cd-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-410">Boolean</span></span>|<span data-ttu-id="166cd-411">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-411">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="166cd-412">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="166cd-412">kioskModeManagedAppId</span></span>|<span data-ttu-id="166cd-413">String</span><span class="sxs-lookup"><span data-stu-id="166cd-413">String</span></span>|<span data-ttu-id="166cd-414">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="166cd-414">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="166cd-415">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="166cd-415">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="166cd-416">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="166cd-416">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="166cd-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-417">Boolean</span></span>|<span data-ttu-id="166cd-418">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="166cd-418">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="166cd-419">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="166cd-419">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="166cd-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-420">Boolean</span></span>|<span data-ttu-id="166cd-421">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="166cd-421">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="166cd-422">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="166cd-422">lockScreenBlockPassbook</span></span>|<span data-ttu-id="166cd-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-423">Boolean</span></span>|<span data-ttu-id="166cd-424">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="166cd-424">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="166cd-425">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="166cd-425">lockScreenBlockTodayView</span></span>|<span data-ttu-id="166cd-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-426">Boolean</span></span>|<span data-ttu-id="166cd-427">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="166cd-427">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="166cd-428">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="166cd-428">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="166cd-429">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="166cd-429">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="166cd-430">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="166cd-430">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="166cd-431">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="166cd-431">mediaContentRatingCanada</span></span>|[<span data-ttu-id="166cd-432">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="166cd-432">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="166cd-433">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="166cd-433">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="166cd-434">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="166cd-434">mediaContentRatingFrance</span></span>|[<span data-ttu-id="166cd-435">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="166cd-435">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="166cd-436">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="166cd-436">Media content rating settings for France</span></span>|
|<span data-ttu-id="166cd-437">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="166cd-437">mediaContentRatingGermany</span></span>|[<span data-ttu-id="166cd-438">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="166cd-438">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="166cd-439">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="166cd-439">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="166cd-440">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="166cd-440">mediaContentRatingIreland</span></span>|[<span data-ttu-id="166cd-441">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="166cd-441">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="166cd-442">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="166cd-442">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="166cd-443">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="166cd-443">mediaContentRatingJapan</span></span>|[<span data-ttu-id="166cd-444">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="166cd-444">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="166cd-445">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="166cd-445">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="166cd-446">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="166cd-446">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="166cd-447">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="166cd-447">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="166cd-448">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="166cd-448">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="166cd-449">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="166cd-449">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="166cd-450">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="166cd-450">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="166cd-451">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="166cd-451">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="166cd-452">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="166cd-452">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="166cd-453">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="166cd-453">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="166cd-454">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="166cd-454">Media content rating settings for United States</span></span>|
|<span data-ttu-id="166cd-455">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="166cd-455">networkUsageRules</span></span>|<span data-ttu-id="166cd-456">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="166cd-456">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="166cd-457">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="166cd-457">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="166cd-458">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="166cd-458">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="166cd-459">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="166cd-459">mediaContentRatingApps</span></span>|[<span data-ttu-id="166cd-460">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="166cd-460">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="166cd-461">Configurações de classificação de conteúdo de mídia para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="166cd-461">Media content rating settings for Apps.</span></span> <span data-ttu-id="166cd-462">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="166cd-462">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="166cd-463">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-463">messagesBlocked</span></span>|<span data-ttu-id="166cd-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-464">Boolean</span></span>|<span data-ttu-id="166cd-465">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-465">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="166cd-466">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="166cd-466">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="166cd-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-467">Boolean</span></span>|<span data-ttu-id="166cd-468">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-468">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="166cd-469">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="166cd-469">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="166cd-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-470">Boolean</span></span>|<span data-ttu-id="166cd-471">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="166cd-471">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="166cd-472">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="166cd-472">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="166cd-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-473">Boolean</span></span>|<span data-ttu-id="166cd-474">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-474">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="166cd-475">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="166cd-475">passcodeBlockModification</span></span>|<span data-ttu-id="166cd-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-476">Boolean</span></span>|<span data-ttu-id="166cd-477">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-477">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="166cd-478">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="166cd-478">passcodeBlockSimple</span></span>|<span data-ttu-id="166cd-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-479">Boolean</span></span>|<span data-ttu-id="166cd-480">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="166cd-480">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="166cd-481">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="166cd-481">passcodeExpirationDays</span></span>|<span data-ttu-id="166cd-482">Int32</span><span class="sxs-lookup"><span data-stu-id="166cd-482">Int32</span></span>|<span data-ttu-id="166cd-483">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="166cd-483">Number of days before the passcode expires.</span></span> <span data-ttu-id="166cd-484">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="166cd-484">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="166cd-485">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="166cd-485">passcodeMinimumLength</span></span>|<span data-ttu-id="166cd-486">Int32</span><span class="sxs-lookup"><span data-stu-id="166cd-486">Int32</span></span>|<span data-ttu-id="166cd-487">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="166cd-487">Minimum length of passcode.</span></span> <span data-ttu-id="166cd-488">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="166cd-488">Valid values 4 to 14</span></span>|
|<span data-ttu-id="166cd-489">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="166cd-489">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="166cd-490">Int32</span><span class="sxs-lookup"><span data-stu-id="166cd-490">Int32</span></span>|<span data-ttu-id="166cd-491">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="166cd-491">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="166cd-492">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="166cd-492">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="166cd-493">Int32</span><span class="sxs-lookup"><span data-stu-id="166cd-493">Int32</span></span>|<span data-ttu-id="166cd-494">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="166cd-494">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="166cd-495">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="166cd-495">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="166cd-496">Int32</span><span class="sxs-lookup"><span data-stu-id="166cd-496">Int32</span></span>|<span data-ttu-id="166cd-497">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="166cd-497">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="166cd-498">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="166cd-498">Valid values 0 to 4</span></span>|
|<span data-ttu-id="166cd-499">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="166cd-499">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="166cd-500">Int32</span><span class="sxs-lookup"><span data-stu-id="166cd-500">Int32</span></span>|<span data-ttu-id="166cd-501">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="166cd-501">Number of previous passcodes to block.</span></span> <span data-ttu-id="166cd-502">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="166cd-502">Valid values 1 to 24</span></span>|
|<span data-ttu-id="166cd-503">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="166cd-503">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="166cd-504">Int32</span><span class="sxs-lookup"><span data-stu-id="166cd-504">Int32</span></span>|<span data-ttu-id="166cd-505">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="166cd-505">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="166cd-506">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="166cd-506">Valid values 4 to 11</span></span>|
|<span data-ttu-id="166cd-507">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="166cd-507">passcodeRequiredType</span></span>|[<span data-ttu-id="166cd-508">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="166cd-508">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="166cd-509">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="166cd-509">Type of passcode that is required.</span></span> <span data-ttu-id="166cd-510">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="166cd-510">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="166cd-511">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="166cd-511">passcodeRequired</span></span>|<span data-ttu-id="166cd-512">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-512">Boolean</span></span>|<span data-ttu-id="166cd-513">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="166cd-513">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="166cd-514">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-514">podcastsBlocked</span></span>|<span data-ttu-id="166cd-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-515">Boolean</span></span>|<span data-ttu-id="166cd-516">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-516">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="166cd-517">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="166cd-517">safariBlockAutofill</span></span>|<span data-ttu-id="166cd-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-518">Boolean</span></span>|<span data-ttu-id="166cd-519">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="166cd-519">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="166cd-520">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="166cd-520">safariBlockJavaScript</span></span>|<span data-ttu-id="166cd-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-521">Boolean</span></span>|<span data-ttu-id="166cd-522">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="166cd-522">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="166cd-523">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="166cd-523">safariBlockPopups</span></span>|<span data-ttu-id="166cd-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-524">Boolean</span></span>|<span data-ttu-id="166cd-525">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="166cd-525">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="166cd-526">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-526">safariBlocked</span></span>|<span data-ttu-id="166cd-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-527">Boolean</span></span>|<span data-ttu-id="166cd-528">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="166cd-528">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="166cd-529">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="166cd-529">safariCookieSettings</span></span>|[<span data-ttu-id="166cd-530">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="166cd-530">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="166cd-531">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="166cd-531">Cookie settings for Safari.</span></span> <span data-ttu-id="166cd-532">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="166cd-532">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="166cd-533">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="166cd-533">safariManagedDomains</span></span>|<span data-ttu-id="166cd-534">String collection</span><span class="sxs-lookup"><span data-stu-id="166cd-534">String collection</span></span>|<span data-ttu-id="166cd-535">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="166cd-535">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="166cd-536">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="166cd-536">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="166cd-537">String collection</span><span class="sxs-lookup"><span data-stu-id="166cd-537">String collection</span></span>|<span data-ttu-id="166cd-538">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="166cd-538">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="166cd-539">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-539">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="166cd-540">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="166cd-540">safariRequireFraudWarning</span></span>|<span data-ttu-id="166cd-541">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-541">Boolean</span></span>|<span data-ttu-id="166cd-542">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="166cd-542">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="166cd-543">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-543">screenCaptureBlocked</span></span>|<span data-ttu-id="166cd-544">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-544">Boolean</span></span>|<span data-ttu-id="166cd-545">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="166cd-545">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="166cd-546">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-546">siriBlocked</span></span>|<span data-ttu-id="166cd-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-547">Boolean</span></span>|<span data-ttu-id="166cd-548">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="166cd-548">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="166cd-549">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="166cd-549">siriBlockedWhenLocked</span></span>|<span data-ttu-id="166cd-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-550">Boolean</span></span>|<span data-ttu-id="166cd-551">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="166cd-551">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="166cd-552">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="166cd-552">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="166cd-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-553">Boolean</span></span>|<span data-ttu-id="166cd-554">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-554">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="166cd-555">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="166cd-555">siriRequireProfanityFilter</span></span>|<span data-ttu-id="166cd-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-556">Boolean</span></span>|<span data-ttu-id="166cd-557">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-557">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="166cd-558">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="166cd-558">spotlightBlockInternetResults</span></span>|<span data-ttu-id="166cd-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-559">Boolean</span></span>|<span data-ttu-id="166cd-560">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-560">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="166cd-561">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="166cd-561">voiceDialingBlocked</span></span>|<span data-ttu-id="166cd-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-562">Boolean</span></span>|<span data-ttu-id="166cd-563">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="166cd-563">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="166cd-564">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="166cd-564">wallpaperBlockModification</span></span>|<span data-ttu-id="166cd-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-565">Boolean</span></span>|<span data-ttu-id="166cd-566">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="166cd-566">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="166cd-567">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="166cd-567">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="166cd-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="166cd-568">Boolean</span></span>|<span data-ttu-id="166cd-569">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="166cd-569">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="166cd-570">Resposta</span><span class="sxs-lookup"><span data-stu-id="166cd-570">Response</span></span>
<span data-ttu-id="166cd-571">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="166cd-571">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="166cd-572">Exemplo</span><span class="sxs-lookup"><span data-stu-id="166cd-572">Example</span></span>

### <a name="request"></a><span data-ttu-id="166cd-573">Solicitação</span><span class="sxs-lookup"><span data-stu-id="166cd-573">Request</span></span>
<span data-ttu-id="166cd-574">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="166cd-574">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 7841

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```

### <a name="response"></a><span data-ttu-id="166cd-575">Resposta</span><span class="sxs-lookup"><span data-stu-id="166cd-575">Response</span></span>
<span data-ttu-id="166cd-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="166cd-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8013

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```









