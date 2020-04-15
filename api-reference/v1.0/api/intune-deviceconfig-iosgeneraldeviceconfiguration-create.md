---
title: Criar iosGeneralDeviceConfiguration
description: Cria um novo objeto iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1165f90440af167c86888a3189f2f0567f1a48f0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463904"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="d34ba-103">Criar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d34ba-103">Create iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="d34ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d34ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d34ba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d34ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d34ba-106">Cria um novo objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d34ba-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d34ba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d34ba-107">Prerequisites</span></span>
<span data-ttu-id="d34ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d34ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d34ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d34ba-110">Permission type</span></span>|<span data-ttu-id="d34ba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d34ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d34ba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d34ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d34ba-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d34ba-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d34ba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d34ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d34ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d34ba-115">Not supported.</span></span>|
|<span data-ttu-id="d34ba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d34ba-116">Application</span></span>|<span data-ttu-id="d34ba-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d34ba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d34ba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d34ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d34ba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d34ba-119">Request headers</span></span>
|<span data-ttu-id="d34ba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d34ba-120">Header</span></span>|<span data-ttu-id="d34ba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d34ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d34ba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d34ba-122">Authorization</span></span>|<span data-ttu-id="d34ba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d34ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d34ba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d34ba-124">Accept</span></span>|<span data-ttu-id="d34ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d34ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d34ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d34ba-126">Request body</span></span>
<span data-ttu-id="d34ba-127">No corpo da solicitação, forneça uma representação JSON do objeto iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d34ba-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="d34ba-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d34ba-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="d34ba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d34ba-129">Property</span></span>|<span data-ttu-id="d34ba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d34ba-130">Type</span></span>|<span data-ttu-id="d34ba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d34ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d34ba-132">id</span><span class="sxs-lookup"><span data-stu-id="d34ba-132">id</span></span>|<span data-ttu-id="d34ba-133">String</span><span class="sxs-lookup"><span data-stu-id="d34ba-133">String</span></span>|<span data-ttu-id="d34ba-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d34ba-134">Key of the entity.</span></span> <span data-ttu-id="d34ba-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d34ba-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d34ba-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d34ba-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d34ba-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d34ba-137">DateTimeOffset</span></span>|<span data-ttu-id="d34ba-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d34ba-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d34ba-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d34ba-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d34ba-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d34ba-140">createdDateTime</span></span>|<span data-ttu-id="d34ba-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d34ba-141">DateTimeOffset</span></span>|<span data-ttu-id="d34ba-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-142">DateTime the object was created.</span></span> <span data-ttu-id="d34ba-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d34ba-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d34ba-144">description</span><span class="sxs-lookup"><span data-stu-id="d34ba-144">description</span></span>|<span data-ttu-id="d34ba-145">String</span><span class="sxs-lookup"><span data-stu-id="d34ba-145">String</span></span>|<span data-ttu-id="d34ba-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d34ba-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d34ba-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d34ba-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d34ba-148">displayName</span><span class="sxs-lookup"><span data-stu-id="d34ba-148">displayName</span></span>|<span data-ttu-id="d34ba-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d34ba-149">String</span></span>|<span data-ttu-id="d34ba-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d34ba-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d34ba-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d34ba-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d34ba-152">versão</span><span class="sxs-lookup"><span data-stu-id="d34ba-152">version</span></span>|<span data-ttu-id="d34ba-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d34ba-153">Int32</span></span>|<span data-ttu-id="d34ba-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d34ba-154">Version of the device configuration.</span></span> <span data-ttu-id="d34ba-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d34ba-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d34ba-156">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="d34ba-156">accountBlockModification</span></span>|<span data-ttu-id="d34ba-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-157">Boolean</span></span>|<span data-ttu-id="d34ba-158">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-158">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-159">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="d34ba-159">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="d34ba-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-160">Boolean</span></span>|<span data-ttu-id="d34ba-161">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-161">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="d34ba-162">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-162">airDropBlocked</span></span>|<span data-ttu-id="d34ba-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-163">Boolean</span></span>|<span data-ttu-id="d34ba-164">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-164">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-165">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="d34ba-165">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="d34ba-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-166">Boolean</span></span>|<span data-ttu-id="d34ba-167">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-167">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d34ba-168">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="d34ba-168">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="d34ba-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-169">Boolean</span></span>|<span data-ttu-id="d34ba-170">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="d34ba-170">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="d34ba-171">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="d34ba-171">appleWatchBlockPairing</span></span>|<span data-ttu-id="d34ba-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-172">Boolean</span></span>|<span data-ttu-id="d34ba-173">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-173">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d34ba-174">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="d34ba-174">appleWatchForceWristDetection</span></span>|<span data-ttu-id="d34ba-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-175">Boolean</span></span>|<span data-ttu-id="d34ba-176">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-176">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="d34ba-177">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-177">appleNewsBlocked</span></span>|<span data-ttu-id="d34ba-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-178">Boolean</span></span>|<span data-ttu-id="d34ba-179">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-179">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d34ba-180">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="d34ba-180">appsSingleAppModeList</span></span>|<span data-ttu-id="d34ba-181">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d34ba-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d34ba-182">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="d34ba-182">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="d34ba-183">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-183">Supervised only.</span></span> <span data-ttu-id="d34ba-184">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d34ba-184">iOS 7.0 and later.</span></span> <span data-ttu-id="d34ba-185">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d34ba-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d34ba-186">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="d34ba-186">appsVisibilityList</span></span>|<span data-ttu-id="d34ba-187">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d34ba-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d34ba-188">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-188">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="d34ba-189">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d34ba-189">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d34ba-190">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="d34ba-190">appsVisibilityListType</span></span>|[<span data-ttu-id="d34ba-191">appListType</span><span class="sxs-lookup"><span data-stu-id="d34ba-191">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d34ba-192">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="d34ba-192">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="d34ba-193">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d34ba-193">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d34ba-194">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="d34ba-194">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="d34ba-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-195">Boolean</span></span>|<span data-ttu-id="d34ba-196">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-196">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d34ba-197">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-197">appStoreBlocked</span></span>|<span data-ttu-id="d34ba-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-198">Boolean</span></span>|<span data-ttu-id="d34ba-199">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="d34ba-199">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="d34ba-200">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="d34ba-200">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="d34ba-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-201">Boolean</span></span>|<span data-ttu-id="d34ba-202">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d34ba-202">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="d34ba-203">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d34ba-203">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="d34ba-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-204">Boolean</span></span>|<span data-ttu-id="d34ba-205">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="d34ba-205">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="d34ba-206">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-206">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d34ba-207">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="d34ba-207">appStoreRequirePassword</span></span>|<span data-ttu-id="d34ba-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-208">Boolean</span></span>|<span data-ttu-id="d34ba-209">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d34ba-209">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="d34ba-210">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="d34ba-210">bluetoothBlockModification</span></span>|<span data-ttu-id="d34ba-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-211">Boolean</span></span>|<span data-ttu-id="d34ba-212">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-212">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="d34ba-213">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-213">cameraBlocked</span></span>|<span data-ttu-id="d34ba-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-214">Boolean</span></span>|<span data-ttu-id="d34ba-215">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d34ba-215">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="d34ba-216">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="d34ba-216">cellularBlockDataRoaming</span></span>|<span data-ttu-id="d34ba-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-217">Boolean</span></span>|<span data-ttu-id="d34ba-218">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-218">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="d34ba-219">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="d34ba-219">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="d34ba-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-220">Boolean</span></span>|<span data-ttu-id="d34ba-221">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="d34ba-221">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="d34ba-222">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="d34ba-222">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="d34ba-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-223">Boolean</span></span>|<span data-ttu-id="d34ba-224">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-224">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-225">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="d34ba-225">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="d34ba-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="d34ba-226">Boolean</span></span>|<span data-ttu-id="d34ba-227">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-227">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="d34ba-228">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="d34ba-228">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="d34ba-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-229">Boolean</span></span>|<span data-ttu-id="d34ba-230">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-230">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="d34ba-231">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="d34ba-231">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="d34ba-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-232">Boolean</span></span>|<span data-ttu-id="d34ba-233">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d34ba-233">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="d34ba-234">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d34ba-234">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="d34ba-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-235">Boolean</span></span>|<span data-ttu-id="d34ba-236">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-236">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d34ba-237">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d34ba-237">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="d34ba-238">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-238">Boolean</span></span>|<span data-ttu-id="d34ba-239">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-239">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-240">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="d34ba-240">compliantAppsList</span></span>|<span data-ttu-id="d34ba-241">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d34ba-241">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d34ba-242">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="d34ba-242">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="d34ba-243">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d34ba-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d34ba-244">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="d34ba-244">compliantAppListType</span></span>|[<span data-ttu-id="d34ba-245">appListType</span><span class="sxs-lookup"><span data-stu-id="d34ba-245">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d34ba-246">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="d34ba-246">List that is in the AppComplianceList.</span></span> <span data-ttu-id="d34ba-247">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d34ba-247">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d34ba-248">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="d34ba-248">configurationProfileBlockChanges</span></span>|<span data-ttu-id="d34ba-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-249">Boolean</span></span>|<span data-ttu-id="d34ba-250">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-250">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-251">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-251">definitionLookupBlocked</span></span>|<span data-ttu-id="d34ba-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-252">Boolean</span></span>|<span data-ttu-id="d34ba-253">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-253">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="d34ba-254">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="d34ba-254">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="d34ba-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-255">Boolean</span></span>|<span data-ttu-id="d34ba-256">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-256">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-257">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="d34ba-257">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="d34ba-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-258">Boolean</span></span>|<span data-ttu-id="d34ba-259">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-259">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-260">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="d34ba-260">deviceBlockNameModification</span></span>|<span data-ttu-id="d34ba-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-261">Boolean</span></span>|<span data-ttu-id="d34ba-262">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-262">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d34ba-263">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="d34ba-263">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="d34ba-264">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-264">Boolean</span></span>|<span data-ttu-id="d34ba-265">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-265">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="d34ba-266">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="d34ba-266">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="d34ba-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-267">Boolean</span></span>|<span data-ttu-id="d34ba-268">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-268">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="d34ba-269">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="d34ba-269">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="d34ba-270">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-270">Boolean</span></span>|<span data-ttu-id="d34ba-271">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="d34ba-271">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="d34ba-272">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="d34ba-272">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="d34ba-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-273">Boolean</span></span>|<span data-ttu-id="d34ba-274">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="d34ba-274">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="d34ba-275">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="d34ba-275">emailInDomainSuffixes</span></span>|<span data-ttu-id="d34ba-276">String collection</span><span class="sxs-lookup"><span data-stu-id="d34ba-276">String collection</span></span>|<span data-ttu-id="d34ba-277">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="d34ba-277">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="d34ba-278">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="d34ba-278">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="d34ba-279">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-279">Boolean</span></span>|<span data-ttu-id="d34ba-280">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="d34ba-280">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="d34ba-281">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="d34ba-281">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="d34ba-282">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-282">Boolean</span></span>|<span data-ttu-id="d34ba-283">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="d34ba-283">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="d34ba-284">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-284">faceTimeBlocked</span></span>|<span data-ttu-id="d34ba-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-285">Boolean</span></span>|<span data-ttu-id="d34ba-286">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="d34ba-286">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="d34ba-287">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-287">findMyFriendsBlocked</span></span>|<span data-ttu-id="d34ba-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-288">Boolean</span></span>|<span data-ttu-id="d34ba-289">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-289">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-290">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="d34ba-290">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="d34ba-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-291">Boolean</span></span>|<span data-ttu-id="d34ba-292">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="d34ba-292">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="d34ba-293">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="d34ba-293">gamingBlockMultiplayer</span></span>|<span data-ttu-id="d34ba-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-294">Boolean</span></span>|<span data-ttu-id="d34ba-295">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="d34ba-295">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="d34ba-296">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-296">gameCenterBlocked</span></span>|<span data-ttu-id="d34ba-297">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-297">Boolean</span></span>|<span data-ttu-id="d34ba-298">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-298">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-299">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-299">hostPairingBlocked</span></span>|<span data-ttu-id="d34ba-300">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-300">Boolean</span></span>|<span data-ttu-id="d34ba-301">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-301">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-302">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-302">iBooksStoreBlocked</span></span>|<span data-ttu-id="d34ba-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-303">Boolean</span></span>|<span data-ttu-id="d34ba-304">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-304">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-305">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="d34ba-305">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="d34ba-306">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-306">Boolean</span></span>|<span data-ttu-id="d34ba-307">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="d34ba-307">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="d34ba-308">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="d34ba-308">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="d34ba-309">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-309">Boolean</span></span>|<span data-ttu-id="d34ba-310">Indica se o usuário será ou não impedido de continuar o trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="d34ba-310">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="d34ba-311">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="d34ba-311">iCloudBlockBackup</span></span>|<span data-ttu-id="d34ba-312">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-312">Boolean</span></span>|<span data-ttu-id="d34ba-313">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-313">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="d34ba-314">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="d34ba-314">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="d34ba-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-315">Boolean</span></span>|<span data-ttu-id="d34ba-316">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d34ba-316">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="d34ba-317">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="d34ba-317">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="d34ba-318">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-318">Boolean</span></span>|<span data-ttu-id="d34ba-319">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d34ba-319">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="d34ba-320">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="d34ba-320">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="d34ba-321">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-321">Boolean</span></span>|<span data-ttu-id="d34ba-322">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d34ba-322">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="d34ba-323">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="d34ba-323">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="d34ba-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="d34ba-324">Boolean</span></span>|<span data-ttu-id="d34ba-325">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d34ba-325">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="d34ba-326">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="d34ba-326">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="d34ba-327">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-327">Boolean</span></span>|<span data-ttu-id="d34ba-328">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d34ba-328">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="d34ba-329">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="d34ba-329">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="d34ba-330">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-330">Boolean</span></span>|<span data-ttu-id="d34ba-331">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="d34ba-331">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="d34ba-332">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="d34ba-332">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="d34ba-333">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-333">Boolean</span></span>|<span data-ttu-id="d34ba-334">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="d34ba-334">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="d34ba-335">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="d34ba-335">iTunesBlockMusicService</span></span>|<span data-ttu-id="d34ba-336">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-336">Boolean</span></span>|<span data-ttu-id="d34ba-337">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-337">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="d34ba-338">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="d34ba-338">iTunesBlockRadio</span></span>|<span data-ttu-id="d34ba-339">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-339">Boolean</span></span>|<span data-ttu-id="d34ba-340">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-340">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d34ba-341">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="d34ba-341">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="d34ba-342">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-342">Boolean</span></span>|<span data-ttu-id="d34ba-343">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-343">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d34ba-344">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="d34ba-344">keyboardBlockDictation</span></span>|<span data-ttu-id="d34ba-345">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-345">Boolean</span></span>|<span data-ttu-id="d34ba-346">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-346">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-347">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="d34ba-347">keyboardBlockPredictive</span></span>|<span data-ttu-id="d34ba-348">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-348">Boolean</span></span>|<span data-ttu-id="d34ba-349">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-349">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d34ba-350">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="d34ba-350">keyboardBlockShortcuts</span></span>|<span data-ttu-id="d34ba-351">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-351">Boolean</span></span>|<span data-ttu-id="d34ba-352">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-352">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d34ba-353">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="d34ba-353">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="d34ba-354">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-354">Boolean</span></span>|<span data-ttu-id="d34ba-355">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-355">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d34ba-356">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="d34ba-356">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="d34ba-357">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-357">Boolean</span></span>|<span data-ttu-id="d34ba-358">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-358">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-359">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="d34ba-359">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="d34ba-360">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-360">Boolean</span></span>|<span data-ttu-id="d34ba-361">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-361">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-362">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="d34ba-362">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="d34ba-363">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-363">Boolean</span></span>|<span data-ttu-id="d34ba-364">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-364">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-365">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="d34ba-365">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="d34ba-366">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-366">Boolean</span></span>|<span data-ttu-id="d34ba-367">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-367">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-368">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="d34ba-368">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="d34ba-369">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-369">Boolean</span></span>|<span data-ttu-id="d34ba-370">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-370">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-371">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="d34ba-371">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="d34ba-372">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-372">Boolean</span></span>|<span data-ttu-id="d34ba-373">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-373">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-374">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="d34ba-374">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="d34ba-375">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-375">Boolean</span></span>|<span data-ttu-id="d34ba-376">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-376">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-377">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="d34ba-377">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="d34ba-378">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-378">Boolean</span></span>|<span data-ttu-id="d34ba-379">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-379">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-380">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="d34ba-380">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="d34ba-381">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-381">Boolean</span></span>|<span data-ttu-id="d34ba-382">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-382">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-383">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="d34ba-383">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="d34ba-384">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-384">Boolean</span></span>|<span data-ttu-id="d34ba-385">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-385">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-386">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="d34ba-386">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="d34ba-387">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-387">Boolean</span></span>|<span data-ttu-id="d34ba-388">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-388">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-389">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d34ba-389">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="d34ba-390">String</span><span class="sxs-lookup"><span data-stu-id="d34ba-390">String</span></span>|<span data-ttu-id="d34ba-391">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-391">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="d34ba-392">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="d34ba-392">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="d34ba-393">Propriedadekioskmodebuiltinappid</span><span class="sxs-lookup"><span data-stu-id="d34ba-393">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="d34ba-394">String</span><span class="sxs-lookup"><span data-stu-id="d34ba-394">String</span></span>|<span data-ttu-id="d34ba-395">ID para aplicativos internos a serem usados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-395">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="d34ba-396">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidos.</span><span class="sxs-lookup"><span data-stu-id="d34ba-396">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="d34ba-397">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="d34ba-397">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="d34ba-398">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-398">Boolean</span></span>|<span data-ttu-id="d34ba-399">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-399">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-400">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="d34ba-400">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="d34ba-401">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-401">Boolean</span></span>|<span data-ttu-id="d34ba-402">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-402">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-403">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="d34ba-403">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="d34ba-404">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-404">Boolean</span></span>|<span data-ttu-id="d34ba-405">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-405">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-406">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="d34ba-406">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="d34ba-407">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-407">Boolean</span></span>|<span data-ttu-id="d34ba-408">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-408">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-409">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="d34ba-409">kioskModeRequireZoom</span></span>|<span data-ttu-id="d34ba-410">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-410">Boolean</span></span>|<span data-ttu-id="d34ba-411">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-411">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="d34ba-412">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="d34ba-412">kioskModeManagedAppId</span></span>|<span data-ttu-id="d34ba-413">String</span><span class="sxs-lookup"><span data-stu-id="d34ba-413">String</span></span>|<span data-ttu-id="d34ba-414">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="d34ba-414">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="d34ba-415">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="d34ba-415">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="d34ba-416">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="d34ba-416">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="d34ba-417">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-417">Boolean</span></span>|<span data-ttu-id="d34ba-418">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="d34ba-418">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="d34ba-419">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="d34ba-419">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="d34ba-420">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-420">Boolean</span></span>|<span data-ttu-id="d34ba-421">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="d34ba-421">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="d34ba-422">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="d34ba-422">lockScreenBlockPassbook</span></span>|<span data-ttu-id="d34ba-423">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-423">Boolean</span></span>|<span data-ttu-id="d34ba-424">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="d34ba-424">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="d34ba-425">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="d34ba-425">lockScreenBlockTodayView</span></span>|<span data-ttu-id="d34ba-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="d34ba-426">Boolean</span></span>|<span data-ttu-id="d34ba-427">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="d34ba-427">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="d34ba-428">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d34ba-428">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="d34ba-429">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d34ba-429">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="d34ba-430">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="d34ba-430">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="d34ba-431">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="d34ba-431">mediaContentRatingCanada</span></span>|[<span data-ttu-id="d34ba-432">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="d34ba-432">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="d34ba-433">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="d34ba-433">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="d34ba-434">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d34ba-434">mediaContentRatingFrance</span></span>|[<span data-ttu-id="d34ba-435">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d34ba-435">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="d34ba-436">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="d34ba-436">Media content rating settings for France</span></span>|
|<span data-ttu-id="d34ba-437">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d34ba-437">mediaContentRatingGermany</span></span>|[<span data-ttu-id="d34ba-438">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d34ba-438">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="d34ba-439">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="d34ba-439">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="d34ba-440">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="d34ba-440">mediaContentRatingIreland</span></span>|[<span data-ttu-id="d34ba-441">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="d34ba-441">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="d34ba-442">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="d34ba-442">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="d34ba-443">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d34ba-443">mediaContentRatingJapan</span></span>|[<span data-ttu-id="d34ba-444">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d34ba-444">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="d34ba-445">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="d34ba-445">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="d34ba-446">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d34ba-446">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="d34ba-447">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d34ba-447">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="d34ba-448">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="d34ba-448">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="d34ba-449">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="d34ba-449">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="d34ba-450">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="d34ba-450">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="d34ba-451">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="d34ba-451">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="d34ba-452">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d34ba-452">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="d34ba-453">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d34ba-453">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="d34ba-454">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="d34ba-454">Media content rating settings for United States</span></span>|
|<span data-ttu-id="d34ba-455">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="d34ba-455">networkUsageRules</span></span>|<span data-ttu-id="d34ba-456">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="d34ba-456">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="d34ba-457">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="d34ba-457">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="d34ba-458">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d34ba-458">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="d34ba-459">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="d34ba-459">mediaContentRatingApps</span></span>|[<span data-ttu-id="d34ba-460">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="d34ba-460">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="d34ba-461">Configurações de classificação de conteúdo de mídia para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d34ba-461">Media content rating settings for Apps.</span></span> <span data-ttu-id="d34ba-462">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="d34ba-462">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="d34ba-463">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-463">messagesBlocked</span></span>|<span data-ttu-id="d34ba-464">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-464">Boolean</span></span>|<span data-ttu-id="d34ba-465">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-465">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="d34ba-466">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="d34ba-466">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="d34ba-467">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-467">Boolean</span></span>|<span data-ttu-id="d34ba-468">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-468">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d34ba-469">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d34ba-469">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="d34ba-470">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-470">Boolean</span></span>|<span data-ttu-id="d34ba-471">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-471">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="d34ba-472">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="d34ba-472">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="d34ba-473">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-473">Boolean</span></span>|<span data-ttu-id="d34ba-474">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-474">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="d34ba-475">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="d34ba-475">passcodeBlockModification</span></span>|<span data-ttu-id="d34ba-476">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-476">Boolean</span></span>|<span data-ttu-id="d34ba-477">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-477">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d34ba-478">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d34ba-478">passcodeBlockSimple</span></span>|<span data-ttu-id="d34ba-479">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-479">Boolean</span></span>|<span data-ttu-id="d34ba-480">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d34ba-480">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="d34ba-481">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d34ba-481">passcodeExpirationDays</span></span>|<span data-ttu-id="d34ba-482">Int32</span><span class="sxs-lookup"><span data-stu-id="d34ba-482">Int32</span></span>|<span data-ttu-id="d34ba-483">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="d34ba-483">Number of days before the passcode expires.</span></span> <span data-ttu-id="d34ba-484">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="d34ba-484">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="d34ba-485">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d34ba-485">passcodeMinimumLength</span></span>|<span data-ttu-id="d34ba-486">Int32</span><span class="sxs-lookup"><span data-stu-id="d34ba-486">Int32</span></span>|<span data-ttu-id="d34ba-487">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="d34ba-487">Minimum length of passcode.</span></span> <span data-ttu-id="d34ba-488">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="d34ba-488">Valid values 4 to 14</span></span>|
|<span data-ttu-id="d34ba-489">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d34ba-489">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d34ba-490">Int32</span><span class="sxs-lookup"><span data-stu-id="d34ba-490">Int32</span></span>|<span data-ttu-id="d34ba-491">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="d34ba-491">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="d34ba-492">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d34ba-492">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d34ba-493">Int32</span><span class="sxs-lookup"><span data-stu-id="d34ba-493">Int32</span></span>|<span data-ttu-id="d34ba-494">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="d34ba-494">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d34ba-495">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d34ba-495">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="d34ba-496">Int32</span><span class="sxs-lookup"><span data-stu-id="d34ba-496">Int32</span></span>|<span data-ttu-id="d34ba-497">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="d34ba-497">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="d34ba-498">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="d34ba-498">Valid values 0 to 4</span></span>|
|<span data-ttu-id="d34ba-499">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="d34ba-499">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="d34ba-500">Int32</span><span class="sxs-lookup"><span data-stu-id="d34ba-500">Int32</span></span>|<span data-ttu-id="d34ba-501">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="d34ba-501">Number of previous passcodes to block.</span></span> <span data-ttu-id="d34ba-502">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="d34ba-502">Valid values 1 to 24</span></span>|
|<span data-ttu-id="d34ba-503">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="d34ba-503">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="d34ba-504">Int32</span><span class="sxs-lookup"><span data-stu-id="d34ba-504">Int32</span></span>|<span data-ttu-id="d34ba-505">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d34ba-505">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="d34ba-506">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="d34ba-506">Valid values 4 to 11</span></span>|
|<span data-ttu-id="d34ba-507">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="d34ba-507">passcodeRequiredType</span></span>|[<span data-ttu-id="d34ba-508">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d34ba-508">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d34ba-509">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="d34ba-509">Type of passcode that is required.</span></span> <span data-ttu-id="d34ba-510">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d34ba-510">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d34ba-511">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="d34ba-511">passcodeRequired</span></span>|<span data-ttu-id="d34ba-512">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-512">Boolean</span></span>|<span data-ttu-id="d34ba-513">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="d34ba-513">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="d34ba-514">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-514">podcastsBlocked</span></span>|<span data-ttu-id="d34ba-515">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-515">Boolean</span></span>|<span data-ttu-id="d34ba-516">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-516">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="d34ba-517">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="d34ba-517">safariBlockAutofill</span></span>|<span data-ttu-id="d34ba-518">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-518">Boolean</span></span>|<span data-ttu-id="d34ba-519">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="d34ba-519">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="d34ba-520">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="d34ba-520">safariBlockJavaScript</span></span>|<span data-ttu-id="d34ba-521">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-521">Boolean</span></span>|<span data-ttu-id="d34ba-522">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="d34ba-522">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="d34ba-523">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="d34ba-523">safariBlockPopups</span></span>|<span data-ttu-id="d34ba-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="d34ba-524">Boolean</span></span>|<span data-ttu-id="d34ba-525">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="d34ba-525">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="d34ba-526">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-526">safariBlocked</span></span>|<span data-ttu-id="d34ba-527">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-527">Boolean</span></span>|<span data-ttu-id="d34ba-528">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="d34ba-528">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="d34ba-529">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d34ba-529">safariCookieSettings</span></span>|[<span data-ttu-id="d34ba-530">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d34ba-530">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="d34ba-531">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="d34ba-531">Cookie settings for Safari.</span></span> <span data-ttu-id="d34ba-532">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="d34ba-532">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="d34ba-533">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="d34ba-533">safariManagedDomains</span></span>|<span data-ttu-id="d34ba-534">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d34ba-534">String collection</span></span>|<span data-ttu-id="d34ba-535">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="d34ba-535">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="d34ba-536">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="d34ba-536">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="d34ba-537">String collection</span><span class="sxs-lookup"><span data-stu-id="d34ba-537">String collection</span></span>|<span data-ttu-id="d34ba-538">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="d34ba-538">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="d34ba-539">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-539">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d34ba-540">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="d34ba-540">safariRequireFraudWarning</span></span>|<span data-ttu-id="d34ba-541">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-541">Boolean</span></span>|<span data-ttu-id="d34ba-542">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="d34ba-542">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="d34ba-543">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-543">screenCaptureBlocked</span></span>|<span data-ttu-id="d34ba-544">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-544">Boolean</span></span>|<span data-ttu-id="d34ba-545">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="d34ba-545">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="d34ba-546">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-546">siriBlocked</span></span>|<span data-ttu-id="d34ba-547">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-547">Boolean</span></span>|<span data-ttu-id="d34ba-548">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="d34ba-548">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="d34ba-549">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-549">siriBlockedWhenLocked</span></span>|<span data-ttu-id="d34ba-550">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-550">Boolean</span></span>|<span data-ttu-id="d34ba-551">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-551">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="d34ba-552">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="d34ba-552">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="d34ba-553">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-553">Boolean</span></span>|<span data-ttu-id="d34ba-554">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-554">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="d34ba-555">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="d34ba-555">siriRequireProfanityFilter</span></span>|<span data-ttu-id="d34ba-556">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-556">Boolean</span></span>|<span data-ttu-id="d34ba-557">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-557">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="d34ba-558">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="d34ba-558">spotlightBlockInternetResults</span></span>|<span data-ttu-id="d34ba-559">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-559">Boolean</span></span>|<span data-ttu-id="d34ba-560">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-560">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="d34ba-561">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="d34ba-561">voiceDialingBlocked</span></span>|<span data-ttu-id="d34ba-562">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-562">Boolean</span></span>|<span data-ttu-id="d34ba-563">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d34ba-563">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="d34ba-564">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="d34ba-564">wallpaperBlockModification</span></span>|<span data-ttu-id="d34ba-565">Booliano</span><span class="sxs-lookup"><span data-stu-id="d34ba-565">Boolean</span></span>|<span data-ttu-id="d34ba-566">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d34ba-566">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="d34ba-567">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="d34ba-567">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="d34ba-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="d34ba-568">Boolean</span></span>|<span data-ttu-id="d34ba-569">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d34ba-569">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="d34ba-570">Resposta</span><span class="sxs-lookup"><span data-stu-id="d34ba-570">Response</span></span>
<span data-ttu-id="d34ba-571">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d34ba-571">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d34ba-572">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d34ba-572">Example</span></span>

### <a name="request"></a><span data-ttu-id="d34ba-573">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d34ba-573">Request</span></span>
<span data-ttu-id="d34ba-574">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d34ba-574">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d34ba-575">Resposta</span><span class="sxs-lookup"><span data-stu-id="d34ba-575">Response</span></span>
<span data-ttu-id="d34ba-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d34ba-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






