---
title: Atualizar iosGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto iosGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d005f9d64ab69be09772e75e72f1cc9739c39c3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973485"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="ad1ee-103">Atualizar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ad1ee-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="ad1ee-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad1ee-105">Atualizar as propriedades de um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-105">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad1ee-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ad1ee-106">Prerequisites</span></span>
<span data-ttu-id="ad1ee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad1ee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad1ee-109">Permission type</span></span>|<span data-ttu-id="ad1ee-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad1ee-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ad1ee-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad1ee-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ad1ee-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad1ee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-114">Not supported.</span></span>|
|<span data-ttu-id="ad1ee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad1ee-115">Application</span></span>|<span data-ttu-id="ad1ee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad1ee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad1ee-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ad1ee-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad1ee-118">Request headers</span></span>
|<span data-ttu-id="ad1ee-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ad1ee-119">Header</span></span>|<span data-ttu-id="ad1ee-120">Valor</span><span class="sxs-lookup"><span data-stu-id="ad1ee-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad1ee-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad1ee-121">Authorization</span></span>|<span data-ttu-id="ad1ee-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad1ee-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ad1ee-123">Accept</span></span>|<span data-ttu-id="ad1ee-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ad1ee-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad1ee-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad1ee-125">Request body</span></span>
<span data-ttu-id="ad1ee-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-126">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="ad1ee-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-127">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="ad1ee-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad1ee-128">Property</span></span>|<span data-ttu-id="ad1ee-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad1ee-129">Type</span></span>|<span data-ttu-id="ad1ee-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad1ee-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad1ee-131">id</span><span class="sxs-lookup"><span data-stu-id="ad1ee-131">id</span></span>|<span data-ttu-id="ad1ee-132">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-132">String</span></span>|<span data-ttu-id="ad1ee-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-133">Key of the entity.</span></span> <span data-ttu-id="ad1ee-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad1ee-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad1ee-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ad1ee-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad1ee-136">DateTimeOffset</span></span>|<span data-ttu-id="ad1ee-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-137">DateTime the object was last modified.</span></span> <span data-ttu-id="ad1ee-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad1ee-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad1ee-139">createdDateTime</span></span>|<span data-ttu-id="ad1ee-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad1ee-140">DateTimeOffset</span></span>|<span data-ttu-id="ad1ee-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-141">DateTime the object was created.</span></span> <span data-ttu-id="ad1ee-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad1ee-143">descrição</span><span class="sxs-lookup"><span data-stu-id="ad1ee-143">description</span></span>|<span data-ttu-id="ad1ee-144">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-144">String</span></span>|<span data-ttu-id="ad1ee-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ad1ee-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad1ee-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ad1ee-147">displayName</span></span>|<span data-ttu-id="ad1ee-148">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-148">String</span></span>|<span data-ttu-id="ad1ee-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ad1ee-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad1ee-151">versão</span><span class="sxs-lookup"><span data-stu-id="ad1ee-151">version</span></span>|<span data-ttu-id="ad1ee-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ad1ee-152">Int32</span></span>|<span data-ttu-id="ad1ee-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-153">Version of the device configuration.</span></span> <span data-ttu-id="ad1ee-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ad1ee-155">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="ad1ee-155">accountBlockModification</span></span>|<span data-ttu-id="ad1ee-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-156">Boolean</span></span>|<span data-ttu-id="ad1ee-157">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-157">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-158">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="ad1ee-158">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="ad1ee-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-159">Boolean</span></span>|<span data-ttu-id="ad1ee-160">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-160">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-161">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-161">airDropBlocked</span></span>|<span data-ttu-id="ad1ee-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-162">Boolean</span></span>|<span data-ttu-id="ad1ee-163">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-163">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-164">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="ad1ee-164">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="ad1ee-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-165">Boolean</span></span>|<span data-ttu-id="ad1ee-166">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-166">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ad1ee-167">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="ad1ee-167">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="ad1ee-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-168">Boolean</span></span>|<span data-ttu-id="ad1ee-169">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-169">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="ad1ee-170">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="ad1ee-170">appleWatchBlockPairing</span></span>|<span data-ttu-id="ad1ee-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-171">Boolean</span></span>|<span data-ttu-id="ad1ee-172">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-172">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ad1ee-173">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="ad1ee-173">appleWatchForceWristDetection</span></span>|<span data-ttu-id="ad1ee-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-174">Boolean</span></span>|<span data-ttu-id="ad1ee-175">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-175">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="ad1ee-176">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-176">appleNewsBlocked</span></span>|<span data-ttu-id="ad1ee-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-177">Boolean</span></span>|<span data-ttu-id="ad1ee-178">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-178">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ad1ee-179">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="ad1ee-179">appsSingleAppModeList</span></span>|<span data-ttu-id="ad1ee-180">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ad1ee-181">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-181">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="ad1ee-182">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-182">Supervised only.</span></span> <span data-ttu-id="ad1ee-183">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-183">iOS 7.0 and later.</span></span> <span data-ttu-id="ad1ee-184">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ad1ee-185">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="ad1ee-185">appsVisibilityList</span></span>|<span data-ttu-id="ad1ee-186">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ad1ee-187">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-187">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="ad1ee-188">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-188">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ad1ee-189">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="ad1ee-189">appsVisibilityListType</span></span>|[<span data-ttu-id="ad1ee-190">appListType</span><span class="sxs-lookup"><span data-stu-id="ad1ee-190">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="ad1ee-191">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-191">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="ad1ee-192">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-192">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ad1ee-193">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="ad1ee-193">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="ad1ee-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-194">Boolean</span></span>|<span data-ttu-id="ad1ee-195">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-195">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ad1ee-196">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-196">appStoreBlocked</span></span>|<span data-ttu-id="ad1ee-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-197">Boolean</span></span>|<span data-ttu-id="ad1ee-198">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-198">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="ad1ee-199">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="ad1ee-199">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="ad1ee-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-200">Boolean</span></span>|<span data-ttu-id="ad1ee-201">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-201">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="ad1ee-202">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ad1ee-202">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="ad1ee-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-203">Boolean</span></span>|<span data-ttu-id="ad1ee-204">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-204">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="ad1ee-205">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-205">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ad1ee-206">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="ad1ee-206">appStoreRequirePassword</span></span>|<span data-ttu-id="ad1ee-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-207">Boolean</span></span>|<span data-ttu-id="ad1ee-208">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-208">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="ad1ee-209">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="ad1ee-209">bluetoothBlockModification</span></span>|<span data-ttu-id="ad1ee-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-210">Boolean</span></span>|<span data-ttu-id="ad1ee-211">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-211">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="ad1ee-212">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-212">cameraBlocked</span></span>|<span data-ttu-id="ad1ee-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-213">Boolean</span></span>|<span data-ttu-id="ad1ee-214">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-214">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="ad1ee-215">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="ad1ee-215">cellularBlockDataRoaming</span></span>|<span data-ttu-id="ad1ee-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-216">Boolean</span></span>|<span data-ttu-id="ad1ee-217">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-217">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="ad1ee-218">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="ad1ee-218">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="ad1ee-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-219">Boolean</span></span>|<span data-ttu-id="ad1ee-220">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-220">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="ad1ee-221">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="ad1ee-221">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="ad1ee-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-222">Boolean</span></span>|<span data-ttu-id="ad1ee-223">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-223">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-224">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="ad1ee-224">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="ad1ee-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-225">Boolean</span></span>|<span data-ttu-id="ad1ee-226">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-226">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="ad1ee-227">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="ad1ee-227">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="ad1ee-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-228">Boolean</span></span>|<span data-ttu-id="ad1ee-229">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-229">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="ad1ee-230">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="ad1ee-230">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="ad1ee-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-231">Boolean</span></span>|<span data-ttu-id="ad1ee-232">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-232">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="ad1ee-233">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ad1ee-233">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="ad1ee-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-234">Boolean</span></span>|<span data-ttu-id="ad1ee-235">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-235">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ad1ee-236">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ad1ee-236">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="ad1ee-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-237">Boolean</span></span>|<span data-ttu-id="ad1ee-238">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-238">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-239">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="ad1ee-239">compliantAppsList</span></span>|<span data-ttu-id="ad1ee-240">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-240">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ad1ee-241">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-241">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="ad1ee-242">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ad1ee-243">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="ad1ee-243">compliantAppListType</span></span>|[<span data-ttu-id="ad1ee-244">appListType</span><span class="sxs-lookup"><span data-stu-id="ad1ee-244">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="ad1ee-245">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-245">List that is in the AppComplianceList.</span></span> <span data-ttu-id="ad1ee-246">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-246">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ad1ee-247">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="ad1ee-247">configurationProfileBlockChanges</span></span>|<span data-ttu-id="ad1ee-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-248">Boolean</span></span>|<span data-ttu-id="ad1ee-249">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-249">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-250">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-250">definitionLookupBlocked</span></span>|<span data-ttu-id="ad1ee-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-251">Boolean</span></span>|<span data-ttu-id="ad1ee-252">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-252">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="ad1ee-253">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="ad1ee-253">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="ad1ee-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-254">Boolean</span></span>|<span data-ttu-id="ad1ee-255">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-255">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-256">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="ad1ee-256">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="ad1ee-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-257">Boolean</span></span>|<span data-ttu-id="ad1ee-258">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-258">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-259">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="ad1ee-259">deviceBlockNameModification</span></span>|<span data-ttu-id="ad1ee-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-260">Boolean</span></span>|<span data-ttu-id="ad1ee-261">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-261">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ad1ee-262">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="ad1ee-262">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="ad1ee-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-263">Boolean</span></span>|<span data-ttu-id="ad1ee-264">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-264">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="ad1ee-265">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="ad1ee-265">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="ad1ee-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-266">Boolean</span></span>|<span data-ttu-id="ad1ee-267">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-267">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="ad1ee-268">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="ad1ee-268">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="ad1ee-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-269">Boolean</span></span>|<span data-ttu-id="ad1ee-270">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-270">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="ad1ee-271">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="ad1ee-271">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="ad1ee-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-272">Boolean</span></span>|<span data-ttu-id="ad1ee-273">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-273">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="ad1ee-274">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="ad1ee-274">emailInDomainSuffixes</span></span>|<span data-ttu-id="ad1ee-275">String collection</span><span class="sxs-lookup"><span data-stu-id="ad1ee-275">String collection</span></span>|<span data-ttu-id="ad1ee-276">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-276">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="ad1ee-277">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="ad1ee-277">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="ad1ee-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-278">Boolean</span></span>|<span data-ttu-id="ad1ee-279">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-279">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="ad1ee-280">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="ad1ee-280">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="ad1ee-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-281">Boolean</span></span>|<span data-ttu-id="ad1ee-282">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-282">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="ad1ee-283">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-283">faceTimeBlocked</span></span>|<span data-ttu-id="ad1ee-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-284">Boolean</span></span>|<span data-ttu-id="ad1ee-285">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-285">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="ad1ee-286">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-286">findMyFriendsBlocked</span></span>|<span data-ttu-id="ad1ee-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-287">Boolean</span></span>|<span data-ttu-id="ad1ee-288">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-288">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-289">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="ad1ee-289">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="ad1ee-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-290">Boolean</span></span>|<span data-ttu-id="ad1ee-291">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-291">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="ad1ee-292">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="ad1ee-292">gamingBlockMultiplayer</span></span>|<span data-ttu-id="ad1ee-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-293">Boolean</span></span>|<span data-ttu-id="ad1ee-294">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-294">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="ad1ee-295">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-295">gameCenterBlocked</span></span>|<span data-ttu-id="ad1ee-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-296">Boolean</span></span>|<span data-ttu-id="ad1ee-297">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-297">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-298">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-298">hostPairingBlocked</span></span>|<span data-ttu-id="ad1ee-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-299">Boolean</span></span>|<span data-ttu-id="ad1ee-300">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-300">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-301">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-301">iBooksStoreBlocked</span></span>|<span data-ttu-id="ad1ee-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-302">Boolean</span></span>|<span data-ttu-id="ad1ee-303">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-303">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-304">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="ad1ee-304">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="ad1ee-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-305">Boolean</span></span>|<span data-ttu-id="ad1ee-306">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-306">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="ad1ee-307">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="ad1ee-307">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="ad1ee-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-308">Boolean</span></span>|<span data-ttu-id="ad1ee-309">Indica se o usuário será ou não impedido de continuar um trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-309">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="ad1ee-310">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="ad1ee-310">iCloudBlockBackup</span></span>|<span data-ttu-id="ad1ee-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-311">Boolean</span></span>|<span data-ttu-id="ad1ee-312">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-312">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="ad1ee-313">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="ad1ee-313">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="ad1ee-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-314">Boolean</span></span>|<span data-ttu-id="ad1ee-315">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-315">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="ad1ee-316">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="ad1ee-316">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="ad1ee-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-317">Boolean</span></span>|<span data-ttu-id="ad1ee-318">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-318">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="ad1ee-319">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="ad1ee-319">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="ad1ee-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-320">Boolean</span></span>|<span data-ttu-id="ad1ee-321">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-321">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="ad1ee-322">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="ad1ee-322">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="ad1ee-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-323">Boolean</span></span>|<span data-ttu-id="ad1ee-324">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-324">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="ad1ee-325">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="ad1ee-325">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="ad1ee-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-326">Boolean</span></span>|<span data-ttu-id="ad1ee-327">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-327">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="ad1ee-328">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="ad1ee-328">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="ad1ee-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-329">Boolean</span></span>|<span data-ttu-id="ad1ee-330">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-330">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="ad1ee-331">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="ad1ee-331">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="ad1ee-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-332">Boolean</span></span>|<span data-ttu-id="ad1ee-333">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-333">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="ad1ee-334">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="ad1ee-334">iTunesBlockMusicService</span></span>|<span data-ttu-id="ad1ee-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-335">Boolean</span></span>|<span data-ttu-id="ad1ee-336">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-336">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="ad1ee-337">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="ad1ee-337">iTunesBlockRadio</span></span>|<span data-ttu-id="ad1ee-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-338">Boolean</span></span>|<span data-ttu-id="ad1ee-339">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-339">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ad1ee-340">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="ad1ee-340">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="ad1ee-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-341">Boolean</span></span>|<span data-ttu-id="ad1ee-342">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-342">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ad1ee-343">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="ad1ee-343">keyboardBlockDictation</span></span>|<span data-ttu-id="ad1ee-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-344">Boolean</span></span>|<span data-ttu-id="ad1ee-345">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-345">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-346">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="ad1ee-346">keyboardBlockPredictive</span></span>|<span data-ttu-id="ad1ee-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-347">Boolean</span></span>|<span data-ttu-id="ad1ee-348">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-348">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ad1ee-349">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="ad1ee-349">keyboardBlockShortcuts</span></span>|<span data-ttu-id="ad1ee-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-350">Boolean</span></span>|<span data-ttu-id="ad1ee-351">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-351">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ad1ee-352">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="ad1ee-352">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="ad1ee-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-353">Boolean</span></span>|<span data-ttu-id="ad1ee-354">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-354">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ad1ee-355">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="ad1ee-355">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="ad1ee-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-356">Boolean</span></span>|<span data-ttu-id="ad1ee-357">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-357">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-358">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="ad1ee-358">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="ad1ee-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-359">Boolean</span></span>|<span data-ttu-id="ad1ee-360">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-360">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-361">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="ad1ee-361">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="ad1ee-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-362">Boolean</span></span>|<span data-ttu-id="ad1ee-363">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-363">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-364">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="ad1ee-364">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="ad1ee-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-365">Boolean</span></span>|<span data-ttu-id="ad1ee-366">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-366">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-367">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="ad1ee-367">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="ad1ee-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-368">Boolean</span></span>|<span data-ttu-id="ad1ee-369">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-369">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-370">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="ad1ee-370">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="ad1ee-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-371">Boolean</span></span>|<span data-ttu-id="ad1ee-372">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-372">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-373">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="ad1ee-373">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="ad1ee-374">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-374">Boolean</span></span>|<span data-ttu-id="ad1ee-375">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-375">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-376">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="ad1ee-376">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="ad1ee-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-377">Boolean</span></span>|<span data-ttu-id="ad1ee-378">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-378">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-379">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="ad1ee-379">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="ad1ee-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-380">Boolean</span></span>|<span data-ttu-id="ad1ee-381">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-381">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-382">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="ad1ee-382">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="ad1ee-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-383">Boolean</span></span>|<span data-ttu-id="ad1ee-384">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-384">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-385">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="ad1ee-385">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="ad1ee-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-386">Boolean</span></span>|<span data-ttu-id="ad1ee-387">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-387">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-388">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ad1ee-388">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="ad1ee-389">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-389">String</span></span>|<span data-ttu-id="ad1ee-390">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-390">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="ad1ee-391">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-391">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="ad1ee-392">Propriedadekioskmodebuiltinappid</span><span class="sxs-lookup"><span data-stu-id="ad1ee-392">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="ad1ee-393">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-393">String</span></span>|<span data-ttu-id="ad1ee-394">ID para aplicativos internos a serem usados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-394">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="ad1ee-395">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidos.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-395">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="ad1ee-396">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="ad1ee-396">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="ad1ee-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-397">Boolean</span></span>|<span data-ttu-id="ad1ee-398">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-398">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-399">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="ad1ee-399">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="ad1ee-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-400">Boolean</span></span>|<span data-ttu-id="ad1ee-401">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-401">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-402">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="ad1ee-402">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="ad1ee-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-403">Boolean</span></span>|<span data-ttu-id="ad1ee-404">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-404">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-405">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="ad1ee-405">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="ad1ee-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-406">Boolean</span></span>|<span data-ttu-id="ad1ee-407">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-407">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-408">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="ad1ee-408">kioskModeRequireZoom</span></span>|<span data-ttu-id="ad1ee-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-409">Boolean</span></span>|<span data-ttu-id="ad1ee-410">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-410">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="ad1ee-411">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="ad1ee-411">kioskModeManagedAppId</span></span>|<span data-ttu-id="ad1ee-412">String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-412">String</span></span>|<span data-ttu-id="ad1ee-413">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-413">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="ad1ee-414">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-414">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="ad1ee-415">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="ad1ee-415">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="ad1ee-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-416">Boolean</span></span>|<span data-ttu-id="ad1ee-417">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-417">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="ad1ee-418">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="ad1ee-418">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="ad1ee-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-419">Boolean</span></span>|<span data-ttu-id="ad1ee-420">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-420">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="ad1ee-421">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="ad1ee-421">lockScreenBlockPassbook</span></span>|<span data-ttu-id="ad1ee-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-422">Boolean</span></span>|<span data-ttu-id="ad1ee-423">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="ad1ee-423">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="ad1ee-424">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="ad1ee-424">lockScreenBlockTodayView</span></span>|<span data-ttu-id="ad1ee-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-425">Boolean</span></span>|<span data-ttu-id="ad1ee-426">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-426">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="ad1ee-427">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ad1ee-427">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="ad1ee-428">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ad1ee-428">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="ad1ee-429">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="ad1ee-429">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="ad1ee-430">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ad1ee-430">mediaContentRatingCanada</span></span>|[<span data-ttu-id="ad1ee-431">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ad1ee-431">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="ad1ee-432">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="ad1ee-432">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="ad1ee-433">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ad1ee-433">mediaContentRatingFrance</span></span>|[<span data-ttu-id="ad1ee-434">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ad1ee-434">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="ad1ee-435">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="ad1ee-435">Media content rating settings for France</span></span>|
|<span data-ttu-id="ad1ee-436">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ad1ee-436">mediaContentRatingGermany</span></span>|[<span data-ttu-id="ad1ee-437">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ad1ee-437">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="ad1ee-438">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="ad1ee-438">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="ad1ee-439">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ad1ee-439">mediaContentRatingIreland</span></span>|[<span data-ttu-id="ad1ee-440">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ad1ee-440">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="ad1ee-441">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="ad1ee-441">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="ad1ee-442">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ad1ee-442">mediaContentRatingJapan</span></span>|[<span data-ttu-id="ad1ee-443">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ad1ee-443">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="ad1ee-444">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="ad1ee-444">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="ad1ee-445">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ad1ee-445">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="ad1ee-446">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ad1ee-446">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="ad1ee-447">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="ad1ee-447">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="ad1ee-448">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ad1ee-448">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="ad1ee-449">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ad1ee-449">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="ad1ee-450">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="ad1ee-450">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="ad1ee-451">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ad1ee-451">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="ad1ee-452">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ad1ee-452">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="ad1ee-453">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="ad1ee-453">Media content rating settings for United States</span></span>|
|<span data-ttu-id="ad1ee-454">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="ad1ee-454">networkUsageRules</span></span>|<span data-ttu-id="ad1ee-455">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="ad1ee-455">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="ad1ee-456">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-456">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="ad1ee-457">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-457">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ad1ee-458">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="ad1ee-458">mediaContentRatingApps</span></span>|[<span data-ttu-id="ad1ee-459">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="ad1ee-459">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="ad1ee-460">Configurações de classificação de conteúdo de mídia para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-460">Media content rating settings for Apps.</span></span> <span data-ttu-id="ad1ee-461">Os valores possíveis são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-461">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="ad1ee-462">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-462">messagesBlocked</span></span>|<span data-ttu-id="ad1ee-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-463">Boolean</span></span>|<span data-ttu-id="ad1ee-464">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-464">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="ad1ee-465">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="ad1ee-465">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="ad1ee-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-466">Boolean</span></span>|<span data-ttu-id="ad1ee-467">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-467">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ad1ee-468">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="ad1ee-468">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="ad1ee-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-469">Boolean</span></span>|<span data-ttu-id="ad1ee-470">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-470">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="ad1ee-471">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="ad1ee-471">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="ad1ee-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-472">Boolean</span></span>|<span data-ttu-id="ad1ee-473">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-473">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="ad1ee-474">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="ad1ee-474">passcodeBlockModification</span></span>|<span data-ttu-id="ad1ee-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-475">Boolean</span></span>|<span data-ttu-id="ad1ee-476">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-476">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ad1ee-477">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ad1ee-477">passcodeBlockSimple</span></span>|<span data-ttu-id="ad1ee-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-478">Boolean</span></span>|<span data-ttu-id="ad1ee-479">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-479">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="ad1ee-480">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ad1ee-480">passcodeExpirationDays</span></span>|<span data-ttu-id="ad1ee-481">Int32</span><span class="sxs-lookup"><span data-stu-id="ad1ee-481">Int32</span></span>|<span data-ttu-id="ad1ee-482">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-482">Number of days before the passcode expires.</span></span> <span data-ttu-id="ad1ee-483">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="ad1ee-483">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="ad1ee-484">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ad1ee-484">passcodeMinimumLength</span></span>|<span data-ttu-id="ad1ee-485">Int32</span><span class="sxs-lookup"><span data-stu-id="ad1ee-485">Int32</span></span>|<span data-ttu-id="ad1ee-486">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-486">Minimum length of passcode.</span></span> <span data-ttu-id="ad1ee-487">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="ad1ee-487">Valid values 4 to 14</span></span>|
|<span data-ttu-id="ad1ee-488">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ad1ee-488">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ad1ee-489">Int32</span><span class="sxs-lookup"><span data-stu-id="ad1ee-489">Int32</span></span>|<span data-ttu-id="ad1ee-490">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-490">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="ad1ee-491">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ad1ee-491">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ad1ee-492">Int32</span><span class="sxs-lookup"><span data-stu-id="ad1ee-492">Int32</span></span>|<span data-ttu-id="ad1ee-493">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-493">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ad1ee-494">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ad1ee-494">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="ad1ee-495">Int32</span><span class="sxs-lookup"><span data-stu-id="ad1ee-495">Int32</span></span>|<span data-ttu-id="ad1ee-496">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-496">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="ad1ee-497">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="ad1ee-497">Valid values 0 to 4</span></span>|
|<span data-ttu-id="ad1ee-498">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="ad1ee-498">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="ad1ee-499">Int32</span><span class="sxs-lookup"><span data-stu-id="ad1ee-499">Int32</span></span>|<span data-ttu-id="ad1ee-500">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-500">Number of previous passcodes to block.</span></span> <span data-ttu-id="ad1ee-501">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="ad1ee-501">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ad1ee-502">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="ad1ee-502">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="ad1ee-503">Int32</span><span class="sxs-lookup"><span data-stu-id="ad1ee-503">Int32</span></span>|<span data-ttu-id="ad1ee-504">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-504">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="ad1ee-505">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="ad1ee-505">Valid values 4 to 11</span></span>|
|<span data-ttu-id="ad1ee-506">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="ad1ee-506">passcodeRequiredType</span></span>|[<span data-ttu-id="ad1ee-507">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ad1ee-507">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ad1ee-508">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-508">Type of passcode that is required.</span></span> <span data-ttu-id="ad1ee-509">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-509">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ad1ee-510">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="ad1ee-510">passcodeRequired</span></span>|<span data-ttu-id="ad1ee-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-511">Boolean</span></span>|<span data-ttu-id="ad1ee-512">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-512">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="ad1ee-513">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-513">podcastsBlocked</span></span>|<span data-ttu-id="ad1ee-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-514">Boolean</span></span>|<span data-ttu-id="ad1ee-515">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-515">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="ad1ee-516">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ad1ee-516">safariBlockAutofill</span></span>|<span data-ttu-id="ad1ee-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-517">Boolean</span></span>|<span data-ttu-id="ad1ee-518">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-518">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="ad1ee-519">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="ad1ee-519">safariBlockJavaScript</span></span>|<span data-ttu-id="ad1ee-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-520">Boolean</span></span>|<span data-ttu-id="ad1ee-521">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-521">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="ad1ee-522">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="ad1ee-522">safariBlockPopups</span></span>|<span data-ttu-id="ad1ee-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-523">Boolean</span></span>|<span data-ttu-id="ad1ee-524">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-524">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="ad1ee-525">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-525">safariBlocked</span></span>|<span data-ttu-id="ad1ee-526">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-526">Boolean</span></span>|<span data-ttu-id="ad1ee-527">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-527">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="ad1ee-528">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ad1ee-528">safariCookieSettings</span></span>|[<span data-ttu-id="ad1ee-529">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ad1ee-529">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="ad1ee-530">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-530">Cookie settings for Safari.</span></span> <span data-ttu-id="ad1ee-531">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-531">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="ad1ee-532">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="ad1ee-532">safariManagedDomains</span></span>|<span data-ttu-id="ad1ee-533">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ad1ee-533">String collection</span></span>|<span data-ttu-id="ad1ee-534">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-534">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="ad1ee-535">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="ad1ee-535">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="ad1ee-536">String collection</span><span class="sxs-lookup"><span data-stu-id="ad1ee-536">String collection</span></span>|<span data-ttu-id="ad1ee-537">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-537">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="ad1ee-538">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-538">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ad1ee-539">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="ad1ee-539">safariRequireFraudWarning</span></span>|<span data-ttu-id="ad1ee-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-540">Boolean</span></span>|<span data-ttu-id="ad1ee-541">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-541">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="ad1ee-542">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-542">screenCaptureBlocked</span></span>|<span data-ttu-id="ad1ee-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-543">Boolean</span></span>|<span data-ttu-id="ad1ee-544">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-544">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="ad1ee-545">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-545">siriBlocked</span></span>|<span data-ttu-id="ad1ee-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-546">Boolean</span></span>|<span data-ttu-id="ad1ee-547">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-547">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="ad1ee-548">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-548">siriBlockedWhenLocked</span></span>|<span data-ttu-id="ad1ee-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-549">Boolean</span></span>|<span data-ttu-id="ad1ee-550">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-550">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="ad1ee-551">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="ad1ee-551">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="ad1ee-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-552">Boolean</span></span>|<span data-ttu-id="ad1ee-553">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-553">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="ad1ee-554">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="ad1ee-554">siriRequireProfanityFilter</span></span>|<span data-ttu-id="ad1ee-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-555">Boolean</span></span>|<span data-ttu-id="ad1ee-556">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-556">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="ad1ee-557">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="ad1ee-557">spotlightBlockInternetResults</span></span>|<span data-ttu-id="ad1ee-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-558">Boolean</span></span>|<span data-ttu-id="ad1ee-559">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-559">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="ad1ee-560">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="ad1ee-560">voiceDialingBlocked</span></span>|<span data-ttu-id="ad1ee-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-561">Boolean</span></span>|<span data-ttu-id="ad1ee-562">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-562">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="ad1ee-563">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="ad1ee-563">wallpaperBlockModification</span></span>|<span data-ttu-id="ad1ee-564">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-564">Boolean</span></span>|<span data-ttu-id="ad1ee-565">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ad1ee-565">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="ad1ee-566">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="ad1ee-566">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="ad1ee-567">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad1ee-567">Boolean</span></span>|<span data-ttu-id="ad1ee-568">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-568">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="ad1ee-569">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad1ee-569">Response</span></span>
<span data-ttu-id="ad1ee-570">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-570">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad1ee-571">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad1ee-571">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad1ee-572">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad1ee-572">Request</span></span>
<span data-ttu-id="ad1ee-573">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-573">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ad1ee-574">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad1ee-574">Response</span></span>
<span data-ttu-id="ad1ee-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad1ee-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



