---
title: Criar iosGeneralDeviceConfiguration
description: Cria um novo objeto iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb12b8650123860ce2586f5027f44d4ccecdc797
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979130"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="8f497-103">Criar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8f497-103">Create iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="8f497-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f497-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f497-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f497-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f497-106">Cria um novo objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8f497-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f497-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f497-107">Prerequisites</span></span>
<span data-ttu-id="8f497-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f497-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f497-110">Permission type</span></span>|<span data-ttu-id="8f497-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f497-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f497-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f497-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f497-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f497-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f497-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f497-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f497-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f497-115">Not supported.</span></span>|
|<span data-ttu-id="8f497-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f497-116">Application</span></span>|<span data-ttu-id="8f497-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f497-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f497-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f497-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8f497-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f497-119">Request headers</span></span>
|<span data-ttu-id="8f497-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f497-120">Header</span></span>|<span data-ttu-id="8f497-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8f497-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f497-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f497-122">Authorization</span></span>|<span data-ttu-id="8f497-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f497-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f497-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8f497-124">Accept</span></span>|<span data-ttu-id="8f497-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8f497-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f497-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f497-126">Request body</span></span>
<span data-ttu-id="8f497-127">No corpo da solicitação, forneça uma representação JSON do objeto iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8f497-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="8f497-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8f497-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="8f497-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f497-129">Property</span></span>|<span data-ttu-id="8f497-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f497-130">Type</span></span>|<span data-ttu-id="8f497-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f497-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f497-132">id</span><span class="sxs-lookup"><span data-stu-id="8f497-132">id</span></span>|<span data-ttu-id="8f497-133">String</span><span class="sxs-lookup"><span data-stu-id="8f497-133">String</span></span>|<span data-ttu-id="8f497-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8f497-134">Key of the entity.</span></span> <span data-ttu-id="8f497-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f497-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f497-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f497-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8f497-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f497-137">DateTimeOffset</span></span>|<span data-ttu-id="8f497-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8f497-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8f497-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f497-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f497-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f497-140">createdDateTime</span></span>|<span data-ttu-id="8f497-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f497-141">DateTimeOffset</span></span>|<span data-ttu-id="8f497-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8f497-142">DateTime the object was created.</span></span> <span data-ttu-id="8f497-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f497-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f497-144">description</span><span class="sxs-lookup"><span data-stu-id="8f497-144">description</span></span>|<span data-ttu-id="8f497-145">String</span><span class="sxs-lookup"><span data-stu-id="8f497-145">String</span></span>|<span data-ttu-id="8f497-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8f497-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8f497-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f497-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f497-148">displayName</span><span class="sxs-lookup"><span data-stu-id="8f497-148">displayName</span></span>|<span data-ttu-id="8f497-149">String</span><span class="sxs-lookup"><span data-stu-id="8f497-149">String</span></span>|<span data-ttu-id="8f497-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8f497-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8f497-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f497-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f497-152">versão</span><span class="sxs-lookup"><span data-stu-id="8f497-152">version</span></span>|<span data-ttu-id="8f497-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8f497-153">Int32</span></span>|<span data-ttu-id="8f497-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8f497-154">Version of the device configuration.</span></span> <span data-ttu-id="8f497-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f497-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f497-156">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="8f497-156">accountBlockModification</span></span>|<span data-ttu-id="8f497-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-157">Boolean</span></span>|<span data-ttu-id="8f497-158">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-158">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="8f497-159">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="8f497-159">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="8f497-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-160">Boolean</span></span>|<span data-ttu-id="8f497-161">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-161">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="8f497-162">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-162">airDropBlocked</span></span>|<span data-ttu-id="8f497-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-163">Boolean</span></span>|<span data-ttu-id="8f497-164">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-164">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="8f497-165">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="8f497-165">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="8f497-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-166">Boolean</span></span>|<span data-ttu-id="8f497-167">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-167">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="8f497-168">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="8f497-168">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="8f497-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-169">Boolean</span></span>|<span data-ttu-id="8f497-170">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="8f497-170">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="8f497-171">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="8f497-171">appleWatchBlockPairing</span></span>|<span data-ttu-id="8f497-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-172">Boolean</span></span>|<span data-ttu-id="8f497-173">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-173">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="8f497-174">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="8f497-174">appleWatchForceWristDetection</span></span>|<span data-ttu-id="8f497-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-175">Boolean</span></span>|<span data-ttu-id="8f497-176">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-176">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="8f497-177">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-177">appleNewsBlocked</span></span>|<span data-ttu-id="8f497-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-178">Boolean</span></span>|<span data-ttu-id="8f497-179">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-179">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="8f497-180">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="8f497-180">appsSingleAppModeList</span></span>|<span data-ttu-id="8f497-181">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="8f497-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8f497-182">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="8f497-182">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="8f497-183">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-183">Supervised only.</span></span> <span data-ttu-id="8f497-184">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="8f497-184">iOS 7.0 and later.</span></span> <span data-ttu-id="8f497-185">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="8f497-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8f497-186">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="8f497-186">appsVisibilityList</span></span>|<span data-ttu-id="8f497-187">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="8f497-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8f497-188">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-188">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="8f497-189">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="8f497-189">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="8f497-190">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="8f497-190">appsVisibilityListType</span></span>|[<span data-ttu-id="8f497-191">appListType</span><span class="sxs-lookup"><span data-stu-id="8f497-191">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="8f497-192">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="8f497-192">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="8f497-193">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="8f497-193">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="8f497-194">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="8f497-194">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="8f497-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-195">Boolean</span></span>|<span data-ttu-id="8f497-196">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-196">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="8f497-197">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-197">appStoreBlocked</span></span>|<span data-ttu-id="8f497-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-198">Boolean</span></span>|<span data-ttu-id="8f497-199">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="8f497-199">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="8f497-200">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="8f497-200">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="8f497-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-201">Boolean</span></span>|<span data-ttu-id="8f497-202">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f497-202">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="8f497-203">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="8f497-203">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="8f497-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-204">Boolean</span></span>|<span data-ttu-id="8f497-205">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="8f497-205">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="8f497-206">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-206">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="8f497-207">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="8f497-207">appStoreRequirePassword</span></span>|<span data-ttu-id="8f497-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-208">Boolean</span></span>|<span data-ttu-id="8f497-209">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8f497-209">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="8f497-210">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="8f497-210">bluetoothBlockModification</span></span>|<span data-ttu-id="8f497-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-211">Boolean</span></span>|<span data-ttu-id="8f497-212">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-212">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="8f497-213">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-213">cameraBlocked</span></span>|<span data-ttu-id="8f497-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-214">Boolean</span></span>|<span data-ttu-id="8f497-215">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8f497-215">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="8f497-216">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="8f497-216">cellularBlockDataRoaming</span></span>|<span data-ttu-id="8f497-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-217">Boolean</span></span>|<span data-ttu-id="8f497-218">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8f497-218">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="8f497-219">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="8f497-219">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="8f497-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-220">Boolean</span></span>|<span data-ttu-id="8f497-221">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="8f497-221">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="8f497-222">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="8f497-222">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="8f497-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-223">Boolean</span></span>|<span data-ttu-id="8f497-224">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-224">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="8f497-225">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="8f497-225">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="8f497-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-226">Boolean</span></span>|<span data-ttu-id="8f497-227">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8f497-227">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="8f497-228">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="8f497-228">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="8f497-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-229">Boolean</span></span>|<span data-ttu-id="8f497-230">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8f497-230">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="8f497-231">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="8f497-231">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="8f497-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-232">Boolean</span></span>|<span data-ttu-id="8f497-233">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="8f497-233">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="8f497-234">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="8f497-234">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="8f497-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-235">Boolean</span></span>|<span data-ttu-id="8f497-236">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-236">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="8f497-237">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="8f497-237">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="8f497-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-238">Boolean</span></span>|<span data-ttu-id="8f497-239">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-239">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="8f497-240">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="8f497-240">compliantAppsList</span></span>|<span data-ttu-id="8f497-241">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="8f497-241">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8f497-242">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="8f497-242">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="8f497-243">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="8f497-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="8f497-244">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="8f497-244">compliantAppListType</span></span>|[<span data-ttu-id="8f497-245">appListType</span><span class="sxs-lookup"><span data-stu-id="8f497-245">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="8f497-246">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="8f497-246">List that is in the AppComplianceList.</span></span> <span data-ttu-id="8f497-247">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="8f497-247">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="8f497-248">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="8f497-248">configurationProfileBlockChanges</span></span>|<span data-ttu-id="8f497-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-249">Boolean</span></span>|<span data-ttu-id="8f497-250">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-250">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="8f497-251">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-251">definitionLookupBlocked</span></span>|<span data-ttu-id="8f497-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-252">Boolean</span></span>|<span data-ttu-id="8f497-253">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-253">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="8f497-254">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="8f497-254">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="8f497-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-255">Boolean</span></span>|<span data-ttu-id="8f497-256">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-256">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="8f497-257">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="8f497-257">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="8f497-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-258">Boolean</span></span>|<span data-ttu-id="8f497-259">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-259">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="8f497-260">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="8f497-260">deviceBlockNameModification</span></span>|<span data-ttu-id="8f497-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-261">Boolean</span></span>|<span data-ttu-id="8f497-262">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-262">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="8f497-263">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="8f497-263">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="8f497-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-264">Boolean</span></span>|<span data-ttu-id="8f497-265">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8f497-265">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="8f497-266">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="8f497-266">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="8f497-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-267">Boolean</span></span>|<span data-ttu-id="8f497-268">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-268">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="8f497-269">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="8f497-269">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="8f497-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-270">Boolean</span></span>|<span data-ttu-id="8f497-271">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="8f497-271">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="8f497-272">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="8f497-272">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="8f497-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-273">Boolean</span></span>|<span data-ttu-id="8f497-274">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="8f497-274">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="8f497-275">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="8f497-275">emailInDomainSuffixes</span></span>|<span data-ttu-id="8f497-276">String collection</span><span class="sxs-lookup"><span data-stu-id="8f497-276">String collection</span></span>|<span data-ttu-id="8f497-277">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="8f497-277">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="8f497-278">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="8f497-278">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="8f497-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-279">Boolean</span></span>|<span data-ttu-id="8f497-280">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="8f497-280">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="8f497-281">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="8f497-281">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="8f497-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-282">Boolean</span></span>|<span data-ttu-id="8f497-283">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="8f497-283">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="8f497-284">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-284">faceTimeBlocked</span></span>|<span data-ttu-id="8f497-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-285">Boolean</span></span>|<span data-ttu-id="8f497-286">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="8f497-286">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="8f497-287">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-287">findMyFriendsBlocked</span></span>|<span data-ttu-id="8f497-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-288">Boolean</span></span>|<span data-ttu-id="8f497-289">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-289">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="8f497-290">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="8f497-290">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="8f497-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-291">Boolean</span></span>|<span data-ttu-id="8f497-292">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="8f497-292">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="8f497-293">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="8f497-293">gamingBlockMultiplayer</span></span>|<span data-ttu-id="8f497-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-294">Boolean</span></span>|<span data-ttu-id="8f497-295">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="8f497-295">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="8f497-296">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-296">gameCenterBlocked</span></span>|<span data-ttu-id="8f497-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-297">Boolean</span></span>|<span data-ttu-id="8f497-298">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-298">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="8f497-299">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-299">hostPairingBlocked</span></span>|<span data-ttu-id="8f497-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-300">Boolean</span></span>|<span data-ttu-id="8f497-301">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-301">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="8f497-302">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-302">iBooksStoreBlocked</span></span>|<span data-ttu-id="8f497-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-303">Boolean</span></span>|<span data-ttu-id="8f497-304">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-304">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="8f497-305">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="8f497-305">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="8f497-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-306">Boolean</span></span>|<span data-ttu-id="8f497-307">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="8f497-307">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="8f497-308">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="8f497-308">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="8f497-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-309">Boolean</span></span>|<span data-ttu-id="8f497-310">Indica se o usuário será ou não impedido de continuar o trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="8f497-310">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="8f497-311">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="8f497-311">iCloudBlockBackup</span></span>|<span data-ttu-id="8f497-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-312">Boolean</span></span>|<span data-ttu-id="8f497-313">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8f497-313">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="8f497-314">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="8f497-314">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="8f497-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-315">Boolean</span></span>|<span data-ttu-id="8f497-316">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8f497-316">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="8f497-317">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="8f497-317">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="8f497-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-318">Boolean</span></span>|<span data-ttu-id="8f497-319">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8f497-319">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="8f497-320">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="8f497-320">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="8f497-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-321">Boolean</span></span>|<span data-ttu-id="8f497-322">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8f497-322">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="8f497-323">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="8f497-323">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="8f497-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-324">Boolean</span></span>|<span data-ttu-id="8f497-325">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8f497-325">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="8f497-326">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="8f497-326">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="8f497-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-327">Boolean</span></span>|<span data-ttu-id="8f497-328">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8f497-328">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="8f497-329">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="8f497-329">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="8f497-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-330">Boolean</span></span>|<span data-ttu-id="8f497-331">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="8f497-331">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="8f497-332">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="8f497-332">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="8f497-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-333">Boolean</span></span>|<span data-ttu-id="8f497-334">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="8f497-334">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="8f497-335">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="8f497-335">iTunesBlockMusicService</span></span>|<span data-ttu-id="8f497-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-336">Boolean</span></span>|<span data-ttu-id="8f497-337">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-337">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="8f497-338">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="8f497-338">iTunesBlockRadio</span></span>|<span data-ttu-id="8f497-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-339">Boolean</span></span>|<span data-ttu-id="8f497-340">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-340">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="8f497-341">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="8f497-341">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="8f497-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-342">Boolean</span></span>|<span data-ttu-id="8f497-343">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-343">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="8f497-344">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="8f497-344">keyboardBlockDictation</span></span>|<span data-ttu-id="8f497-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-345">Boolean</span></span>|<span data-ttu-id="8f497-346">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-346">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="8f497-347">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="8f497-347">keyboardBlockPredictive</span></span>|<span data-ttu-id="8f497-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-348">Boolean</span></span>|<span data-ttu-id="8f497-349">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-349">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="8f497-350">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="8f497-350">keyboardBlockShortcuts</span></span>|<span data-ttu-id="8f497-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-351">Boolean</span></span>|<span data-ttu-id="8f497-352">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-352">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="8f497-353">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="8f497-353">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="8f497-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-354">Boolean</span></span>|<span data-ttu-id="8f497-355">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-355">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="8f497-356">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="8f497-356">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="8f497-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-357">Boolean</span></span>|<span data-ttu-id="8f497-358">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-358">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-359">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="8f497-359">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="8f497-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-360">Boolean</span></span>|<span data-ttu-id="8f497-361">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-361">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-362">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="8f497-362">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="8f497-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-363">Boolean</span></span>|<span data-ttu-id="8f497-364">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-364">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-365">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="8f497-365">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="8f497-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-366">Boolean</span></span>|<span data-ttu-id="8f497-367">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-367">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-368">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="8f497-368">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="8f497-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-369">Boolean</span></span>|<span data-ttu-id="8f497-370">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-370">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-371">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="8f497-371">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="8f497-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-372">Boolean</span></span>|<span data-ttu-id="8f497-373">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-373">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-374">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="8f497-374">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="8f497-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-375">Boolean</span></span>|<span data-ttu-id="8f497-376">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-376">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-377">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="8f497-377">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="8f497-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-378">Boolean</span></span>|<span data-ttu-id="8f497-379">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-379">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-380">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="8f497-380">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="8f497-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-381">Boolean</span></span>|<span data-ttu-id="8f497-382">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-382">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-383">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="8f497-383">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="8f497-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-384">Boolean</span></span>|<span data-ttu-id="8f497-385">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-385">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-386">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="8f497-386">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="8f497-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-387">Boolean</span></span>|<span data-ttu-id="8f497-388">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-388">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-389">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8f497-389">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="8f497-390">String</span><span class="sxs-lookup"><span data-stu-id="8f497-390">String</span></span>|<span data-ttu-id="8f497-391">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-391">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="8f497-392">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="8f497-392">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="8f497-393">Propriedadekioskmodebuiltinappid</span><span class="sxs-lookup"><span data-stu-id="8f497-393">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="8f497-394">String</span><span class="sxs-lookup"><span data-stu-id="8f497-394">String</span></span>|<span data-ttu-id="8f497-395">ID para aplicativos internos a serem usados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-395">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="8f497-396">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidos.</span><span class="sxs-lookup"><span data-stu-id="8f497-396">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="8f497-397">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="8f497-397">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="8f497-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-398">Boolean</span></span>|<span data-ttu-id="8f497-399">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-399">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-400">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="8f497-400">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="8f497-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-401">Boolean</span></span>|<span data-ttu-id="8f497-402">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-402">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-403">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="8f497-403">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="8f497-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-404">Boolean</span></span>|<span data-ttu-id="8f497-405">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-405">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-406">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="8f497-406">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="8f497-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-407">Boolean</span></span>|<span data-ttu-id="8f497-408">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-408">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-409">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="8f497-409">kioskModeRequireZoom</span></span>|<span data-ttu-id="8f497-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-410">Boolean</span></span>|<span data-ttu-id="8f497-411">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-411">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="8f497-412">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="8f497-412">kioskModeManagedAppId</span></span>|<span data-ttu-id="8f497-413">String</span><span class="sxs-lookup"><span data-stu-id="8f497-413">String</span></span>|<span data-ttu-id="8f497-414">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="8f497-414">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="8f497-415">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="8f497-415">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="8f497-416">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="8f497-416">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="8f497-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-417">Boolean</span></span>|<span data-ttu-id="8f497-418">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="8f497-418">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="8f497-419">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="8f497-419">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="8f497-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-420">Boolean</span></span>|<span data-ttu-id="8f497-421">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="8f497-421">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="8f497-422">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="8f497-422">lockScreenBlockPassbook</span></span>|<span data-ttu-id="8f497-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-423">Boolean</span></span>|<span data-ttu-id="8f497-424">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="8f497-424">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="8f497-425">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="8f497-425">lockScreenBlockTodayView</span></span>|<span data-ttu-id="8f497-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-426">Boolean</span></span>|<span data-ttu-id="8f497-427">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="8f497-427">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="8f497-428">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="8f497-428">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="8f497-429">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="8f497-429">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="8f497-430">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="8f497-430">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="8f497-431">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="8f497-431">mediaContentRatingCanada</span></span>|[<span data-ttu-id="8f497-432">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="8f497-432">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="8f497-433">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="8f497-433">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="8f497-434">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="8f497-434">mediaContentRatingFrance</span></span>|[<span data-ttu-id="8f497-435">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="8f497-435">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="8f497-436">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="8f497-436">Media content rating settings for France</span></span>|
|<span data-ttu-id="8f497-437">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="8f497-437">mediaContentRatingGermany</span></span>|[<span data-ttu-id="8f497-438">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="8f497-438">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="8f497-439">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="8f497-439">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="8f497-440">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="8f497-440">mediaContentRatingIreland</span></span>|[<span data-ttu-id="8f497-441">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="8f497-441">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="8f497-442">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="8f497-442">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="8f497-443">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="8f497-443">mediaContentRatingJapan</span></span>|[<span data-ttu-id="8f497-444">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="8f497-444">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="8f497-445">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="8f497-445">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="8f497-446">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="8f497-446">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="8f497-447">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="8f497-447">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="8f497-448">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="8f497-448">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="8f497-449">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="8f497-449">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="8f497-450">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="8f497-450">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="8f497-451">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="8f497-451">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="8f497-452">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="8f497-452">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="8f497-453">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="8f497-453">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="8f497-454">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="8f497-454">Media content rating settings for United States</span></span>|
|<span data-ttu-id="8f497-455">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="8f497-455">networkUsageRules</span></span>|<span data-ttu-id="8f497-456">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="8f497-456">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="8f497-457">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="8f497-457">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="8f497-458">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="8f497-458">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="8f497-459">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="8f497-459">mediaContentRatingApps</span></span>|[<span data-ttu-id="8f497-460">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="8f497-460">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="8f497-461">Configurações de classificação de conteúdo de mídia para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8f497-461">Media content rating settings for Apps.</span></span> <span data-ttu-id="8f497-462">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="8f497-462">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="8f497-463">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-463">messagesBlocked</span></span>|<span data-ttu-id="8f497-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-464">Boolean</span></span>|<span data-ttu-id="8f497-465">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-465">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="8f497-466">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="8f497-466">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="8f497-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-467">Boolean</span></span>|<span data-ttu-id="8f497-468">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-468">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="8f497-469">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="8f497-469">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="8f497-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-470">Boolean</span></span>|<span data-ttu-id="8f497-471">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8f497-471">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="8f497-472">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="8f497-472">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="8f497-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-473">Boolean</span></span>|<span data-ttu-id="8f497-474">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-474">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="8f497-475">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="8f497-475">passcodeBlockModification</span></span>|<span data-ttu-id="8f497-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-476">Boolean</span></span>|<span data-ttu-id="8f497-477">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-477">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="8f497-478">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="8f497-478">passcodeBlockSimple</span></span>|<span data-ttu-id="8f497-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-479">Boolean</span></span>|<span data-ttu-id="8f497-480">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="8f497-480">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="8f497-481">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8f497-481">passcodeExpirationDays</span></span>|<span data-ttu-id="8f497-482">Int32</span><span class="sxs-lookup"><span data-stu-id="8f497-482">Int32</span></span>|<span data-ttu-id="8f497-483">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="8f497-483">Number of days before the passcode expires.</span></span> <span data-ttu-id="8f497-484">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="8f497-484">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="8f497-485">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8f497-485">passcodeMinimumLength</span></span>|<span data-ttu-id="8f497-486">Int32</span><span class="sxs-lookup"><span data-stu-id="8f497-486">Int32</span></span>|<span data-ttu-id="8f497-487">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="8f497-487">Minimum length of passcode.</span></span> <span data-ttu-id="8f497-488">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="8f497-488">Valid values 4 to 14</span></span>|
|<span data-ttu-id="8f497-489">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="8f497-489">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="8f497-490">Int32</span><span class="sxs-lookup"><span data-stu-id="8f497-490">Int32</span></span>|<span data-ttu-id="8f497-491">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="8f497-491">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="8f497-492">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8f497-492">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8f497-493">Int32</span><span class="sxs-lookup"><span data-stu-id="8f497-493">Int32</span></span>|<span data-ttu-id="8f497-494">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="8f497-494">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8f497-495">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8f497-495">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="8f497-496">Int32</span><span class="sxs-lookup"><span data-stu-id="8f497-496">Int32</span></span>|<span data-ttu-id="8f497-497">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="8f497-497">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="8f497-498">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="8f497-498">Valid values 0 to 4</span></span>|
|<span data-ttu-id="8f497-499">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="8f497-499">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="8f497-500">Int32</span><span class="sxs-lookup"><span data-stu-id="8f497-500">Int32</span></span>|<span data-ttu-id="8f497-501">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="8f497-501">Number of previous passcodes to block.</span></span> <span data-ttu-id="8f497-502">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="8f497-502">Valid values 1 to 24</span></span>|
|<span data-ttu-id="8f497-503">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="8f497-503">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="8f497-504">Int32</span><span class="sxs-lookup"><span data-stu-id="8f497-504">Int32</span></span>|<span data-ttu-id="8f497-505">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8f497-505">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="8f497-506">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="8f497-506">Valid values 4 to 11</span></span>|
|<span data-ttu-id="8f497-507">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="8f497-507">passcodeRequiredType</span></span>|[<span data-ttu-id="8f497-508">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8f497-508">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8f497-509">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="8f497-509">Type of passcode that is required.</span></span> <span data-ttu-id="8f497-510">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="8f497-510">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8f497-511">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="8f497-511">passcodeRequired</span></span>|<span data-ttu-id="8f497-512">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-512">Boolean</span></span>|<span data-ttu-id="8f497-513">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="8f497-513">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="8f497-514">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-514">podcastsBlocked</span></span>|<span data-ttu-id="8f497-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-515">Boolean</span></span>|<span data-ttu-id="8f497-516">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-516">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="8f497-517">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="8f497-517">safariBlockAutofill</span></span>|<span data-ttu-id="8f497-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-518">Boolean</span></span>|<span data-ttu-id="8f497-519">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="8f497-519">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="8f497-520">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="8f497-520">safariBlockJavaScript</span></span>|<span data-ttu-id="8f497-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-521">Boolean</span></span>|<span data-ttu-id="8f497-522">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="8f497-522">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="8f497-523">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="8f497-523">safariBlockPopups</span></span>|<span data-ttu-id="8f497-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-524">Boolean</span></span>|<span data-ttu-id="8f497-525">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="8f497-525">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="8f497-526">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-526">safariBlocked</span></span>|<span data-ttu-id="8f497-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-527">Boolean</span></span>|<span data-ttu-id="8f497-528">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="8f497-528">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="8f497-529">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="8f497-529">safariCookieSettings</span></span>|[<span data-ttu-id="8f497-530">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="8f497-530">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="8f497-531">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="8f497-531">Cookie settings for Safari.</span></span> <span data-ttu-id="8f497-532">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="8f497-532">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="8f497-533">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="8f497-533">safariManagedDomains</span></span>|<span data-ttu-id="8f497-534">String collection</span><span class="sxs-lookup"><span data-stu-id="8f497-534">String collection</span></span>|<span data-ttu-id="8f497-535">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="8f497-535">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="8f497-536">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="8f497-536">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="8f497-537">String collection</span><span class="sxs-lookup"><span data-stu-id="8f497-537">String collection</span></span>|<span data-ttu-id="8f497-538">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="8f497-538">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="8f497-539">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-539">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="8f497-540">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="8f497-540">safariRequireFraudWarning</span></span>|<span data-ttu-id="8f497-541">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-541">Boolean</span></span>|<span data-ttu-id="8f497-542">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="8f497-542">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="8f497-543">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-543">screenCaptureBlocked</span></span>|<span data-ttu-id="8f497-544">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-544">Boolean</span></span>|<span data-ttu-id="8f497-545">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="8f497-545">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="8f497-546">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-546">siriBlocked</span></span>|<span data-ttu-id="8f497-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-547">Boolean</span></span>|<span data-ttu-id="8f497-548">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="8f497-548">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="8f497-549">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="8f497-549">siriBlockedWhenLocked</span></span>|<span data-ttu-id="8f497-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-550">Boolean</span></span>|<span data-ttu-id="8f497-551">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8f497-551">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="8f497-552">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="8f497-552">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="8f497-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-553">Boolean</span></span>|<span data-ttu-id="8f497-554">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-554">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="8f497-555">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="8f497-555">siriRequireProfanityFilter</span></span>|<span data-ttu-id="8f497-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-556">Boolean</span></span>|<span data-ttu-id="8f497-557">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-557">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="8f497-558">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="8f497-558">spotlightBlockInternetResults</span></span>|<span data-ttu-id="8f497-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-559">Boolean</span></span>|<span data-ttu-id="8f497-560">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-560">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="8f497-561">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="8f497-561">voiceDialingBlocked</span></span>|<span data-ttu-id="8f497-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-562">Boolean</span></span>|<span data-ttu-id="8f497-563">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="8f497-563">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="8f497-564">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="8f497-564">wallpaperBlockModification</span></span>|<span data-ttu-id="8f497-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-565">Boolean</span></span>|<span data-ttu-id="8f497-566">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="8f497-566">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="8f497-567">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="8f497-567">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="8f497-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f497-568">Boolean</span></span>|<span data-ttu-id="8f497-569">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="8f497-569">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="8f497-570">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f497-570">Response</span></span>
<span data-ttu-id="8f497-571">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f497-571">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f497-572">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f497-572">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f497-573">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f497-573">Request</span></span>
<span data-ttu-id="8f497-574">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f497-574">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8f497-575">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f497-575">Response</span></span>
<span data-ttu-id="8f497-p127">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f497-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









