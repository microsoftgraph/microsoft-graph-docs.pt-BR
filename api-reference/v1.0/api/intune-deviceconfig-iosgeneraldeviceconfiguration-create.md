---
title: Criar iosGeneralDeviceConfiguration
description: Cria um novo objeto iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e8649b945c6f57b1968c067798ac5141b28a089
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757077"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="7baca-103">Criar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="7baca-103">Create iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="7baca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7baca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7baca-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7baca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7baca-106">Cria um novo objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7baca-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7baca-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7baca-107">Prerequisites</span></span>
<span data-ttu-id="7baca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7baca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7baca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7baca-110">Permission type</span></span>|<span data-ttu-id="7baca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7baca-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7baca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7baca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7baca-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7baca-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7baca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7baca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7baca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7baca-115">Not supported.</span></span>|
|<span data-ttu-id="7baca-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7baca-116">Application</span></span>|<span data-ttu-id="7baca-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7baca-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7baca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7baca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7baca-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7baca-119">Request headers</span></span>
|<span data-ttu-id="7baca-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7baca-120">Header</span></span>|<span data-ttu-id="7baca-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7baca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7baca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7baca-122">Authorization</span></span>|<span data-ttu-id="7baca-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7baca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7baca-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7baca-124">Accept</span></span>|<span data-ttu-id="7baca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7baca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7baca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7baca-126">Request body</span></span>
<span data-ttu-id="7baca-127">No corpo da solicitação, forneça uma representação JSON do objeto iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7baca-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="7baca-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7baca-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="7baca-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7baca-129">Property</span></span>|<span data-ttu-id="7baca-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7baca-130">Type</span></span>|<span data-ttu-id="7baca-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7baca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7baca-132">id</span><span class="sxs-lookup"><span data-stu-id="7baca-132">id</span></span>|<span data-ttu-id="7baca-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7baca-133">String</span></span>|<span data-ttu-id="7baca-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7baca-134">Key of the entity.</span></span> <span data-ttu-id="7baca-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7baca-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7baca-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7baca-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7baca-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7baca-137">DateTimeOffset</span></span>|<span data-ttu-id="7baca-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7baca-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7baca-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7baca-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7baca-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7baca-140">createdDateTime</span></span>|<span data-ttu-id="7baca-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7baca-141">DateTimeOffset</span></span>|<span data-ttu-id="7baca-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7baca-142">DateTime the object was created.</span></span> <span data-ttu-id="7baca-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7baca-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7baca-144">descrição</span><span class="sxs-lookup"><span data-stu-id="7baca-144">description</span></span>|<span data-ttu-id="7baca-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7baca-145">String</span></span>|<span data-ttu-id="7baca-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7baca-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7baca-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7baca-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7baca-148">displayName</span><span class="sxs-lookup"><span data-stu-id="7baca-148">displayName</span></span>|<span data-ttu-id="7baca-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7baca-149">String</span></span>|<span data-ttu-id="7baca-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7baca-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7baca-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7baca-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7baca-152">versão</span><span class="sxs-lookup"><span data-stu-id="7baca-152">version</span></span>|<span data-ttu-id="7baca-153">Int32</span><span class="sxs-lookup"><span data-stu-id="7baca-153">Int32</span></span>|<span data-ttu-id="7baca-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7baca-154">Version of the device configuration.</span></span> <span data-ttu-id="7baca-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7baca-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7baca-156">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="7baca-156">accountBlockModification</span></span>|<span data-ttu-id="7baca-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-157">Boolean</span></span>|<span data-ttu-id="7baca-158">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-158">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7baca-159">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="7baca-159">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="7baca-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-160">Boolean</span></span>|<span data-ttu-id="7baca-161">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-161">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="7baca-162">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-162">airDropBlocked</span></span>|<span data-ttu-id="7baca-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-163">Boolean</span></span>|<span data-ttu-id="7baca-164">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-164">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7baca-165">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="7baca-165">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="7baca-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-166">Boolean</span></span>|<span data-ttu-id="7baca-167">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-167">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7baca-168">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="7baca-168">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="7baca-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-169">Boolean</span></span>|<span data-ttu-id="7baca-170">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="7baca-170">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="7baca-171">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="7baca-171">appleWatchBlockPairing</span></span>|<span data-ttu-id="7baca-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-172">Boolean</span></span>|<span data-ttu-id="7baca-173">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-173">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7baca-174">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="7baca-174">appleWatchForceWristDetection</span></span>|<span data-ttu-id="7baca-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-175">Boolean</span></span>|<span data-ttu-id="7baca-176">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-176">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="7baca-177">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-177">appleNewsBlocked</span></span>|<span data-ttu-id="7baca-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-178">Boolean</span></span>|<span data-ttu-id="7baca-179">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-179">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7baca-180">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="7baca-180">appsSingleAppModeList</span></span>|<span data-ttu-id="7baca-181">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7baca-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7baca-182">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="7baca-182">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="7baca-183">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-183">Supervised only.</span></span> <span data-ttu-id="7baca-184">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7baca-184">iOS 7.0 and later.</span></span> <span data-ttu-id="7baca-185">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="7baca-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7baca-186">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="7baca-186">appsVisibilityList</span></span>|<span data-ttu-id="7baca-187">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7baca-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7baca-188">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-188">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="7baca-189">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="7baca-189">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="7baca-190">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="7baca-190">appsVisibilityListType</span></span>|[<span data-ttu-id="7baca-191">appListType</span><span class="sxs-lookup"><span data-stu-id="7baca-191">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="7baca-192">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="7baca-192">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="7baca-193">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="7baca-193">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="7baca-194">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="7baca-194">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="7baca-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-195">Boolean</span></span>|<span data-ttu-id="7baca-196">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-196">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7baca-197">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-197">appStoreBlocked</span></span>|<span data-ttu-id="7baca-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-198">Boolean</span></span>|<span data-ttu-id="7baca-199">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="7baca-199">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="7baca-200">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7baca-200">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="7baca-201">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="7baca-201">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="7baca-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-202">Boolean</span></span>|<span data-ttu-id="7baca-203">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7baca-203">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="7baca-204">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="7baca-204">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="7baca-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-205">Boolean</span></span>|<span data-ttu-id="7baca-206">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="7baca-206">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="7baca-207">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-207">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7baca-208">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="7baca-208">appStoreRequirePassword</span></span>|<span data-ttu-id="7baca-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-209">Boolean</span></span>|<span data-ttu-id="7baca-210">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="7baca-210">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="7baca-211">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="7baca-211">bluetoothBlockModification</span></span>|<span data-ttu-id="7baca-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-212">Boolean</span></span>|<span data-ttu-id="7baca-213">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-213">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="7baca-214">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-214">cameraBlocked</span></span>|<span data-ttu-id="7baca-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-215">Boolean</span></span>|<span data-ttu-id="7baca-216">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7baca-216">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="7baca-217">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7baca-217">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="7baca-218">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="7baca-218">cellularBlockDataRoaming</span></span>|<span data-ttu-id="7baca-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-219">Boolean</span></span>|<span data-ttu-id="7baca-220">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7baca-220">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="7baca-221">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="7baca-221">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="7baca-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-222">Boolean</span></span>|<span data-ttu-id="7baca-223">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="7baca-223">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="7baca-224">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="7baca-224">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="7baca-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-225">Boolean</span></span>|<span data-ttu-id="7baca-226">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-226">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7baca-227">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="7baca-227">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="7baca-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-228">Boolean</span></span>|<span data-ttu-id="7baca-229">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7baca-229">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="7baca-230">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="7baca-230">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="7baca-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-231">Boolean</span></span>|<span data-ttu-id="7baca-232">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7baca-232">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="7baca-233">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="7baca-233">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="7baca-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-234">Boolean</span></span>|<span data-ttu-id="7baca-235">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="7baca-235">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="7baca-236">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="7baca-236">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="7baca-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-237">Boolean</span></span>|<span data-ttu-id="7baca-238">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-238">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="7baca-239">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="7baca-239">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="7baca-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-240">Boolean</span></span>|<span data-ttu-id="7baca-241">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-241">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7baca-242">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="7baca-242">compliantAppsList</span></span>|<span data-ttu-id="7baca-243">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7baca-243">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="7baca-244">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="7baca-244">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="7baca-245">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="7baca-245">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="7baca-246">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="7baca-246">compliantAppListType</span></span>|[<span data-ttu-id="7baca-247">appListType</span><span class="sxs-lookup"><span data-stu-id="7baca-247">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="7baca-248">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="7baca-248">List that is in the AppComplianceList.</span></span> <span data-ttu-id="7baca-249">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="7baca-249">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="7baca-250">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="7baca-250">configurationProfileBlockChanges</span></span>|<span data-ttu-id="7baca-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-251">Boolean</span></span>|<span data-ttu-id="7baca-252">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-252">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7baca-253">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-253">definitionLookupBlocked</span></span>|<span data-ttu-id="7baca-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-254">Boolean</span></span>|<span data-ttu-id="7baca-255">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-255">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="7baca-256">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="7baca-256">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="7baca-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-257">Boolean</span></span>|<span data-ttu-id="7baca-258">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-258">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7baca-259">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="7baca-259">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="7baca-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-260">Boolean</span></span>|<span data-ttu-id="7baca-261">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-261">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7baca-262">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="7baca-262">deviceBlockNameModification</span></span>|<span data-ttu-id="7baca-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-263">Boolean</span></span>|<span data-ttu-id="7baca-264">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-264">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7baca-265">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="7baca-265">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="7baca-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-266">Boolean</span></span>|<span data-ttu-id="7baca-267">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7baca-267">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="7baca-268">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="7baca-268">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="7baca-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-269">Boolean</span></span>|<span data-ttu-id="7baca-270">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-270">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="7baca-271">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="7baca-271">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="7baca-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-272">Boolean</span></span>|<span data-ttu-id="7baca-273">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="7baca-273">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="7baca-274">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="7baca-274">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="7baca-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-275">Boolean</span></span>|<span data-ttu-id="7baca-276">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="7baca-276">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="7baca-277">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="7baca-277">emailInDomainSuffixes</span></span>|<span data-ttu-id="7baca-278">String collection</span><span class="sxs-lookup"><span data-stu-id="7baca-278">String collection</span></span>|<span data-ttu-id="7baca-279">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="7baca-279">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="7baca-280">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="7baca-280">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="7baca-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-281">Boolean</span></span>|<span data-ttu-id="7baca-282">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="7baca-282">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="7baca-283">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="7baca-283">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="7baca-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-284">Boolean</span></span>|<span data-ttu-id="7baca-285">\[Preterido Configurar essa configuração e definir o valor como \] "true" não tem efeito no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7baca-285">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="7baca-286">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-286">faceTimeBlocked</span></span>|<span data-ttu-id="7baca-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-287">Boolean</span></span>|<span data-ttu-id="7baca-288">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="7baca-288">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="7baca-289">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7baca-289">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="7baca-290">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-290">findMyFriendsBlocked</span></span>|<span data-ttu-id="7baca-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-291">Boolean</span></span>|<span data-ttu-id="7baca-292">Indica se deve ou não bloquear as alterações para Encontrar Meus Amigos quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-292">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7baca-293">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="7baca-293">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="7baca-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-294">Boolean</span></span>|<span data-ttu-id="7baca-295">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="7baca-295">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="7baca-296">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7baca-296">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="7baca-297">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="7baca-297">gamingBlockMultiplayer</span></span>|<span data-ttu-id="7baca-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-298">Boolean</span></span>|<span data-ttu-id="7baca-299">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="7baca-299">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="7baca-300">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7baca-300">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="7baca-301">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-301">gameCenterBlocked</span></span>|<span data-ttu-id="7baca-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-302">Boolean</span></span>|<span data-ttu-id="7baca-303">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-303">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7baca-304">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-304">hostPairingBlocked</span></span>|<span data-ttu-id="7baca-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-305">Boolean</span></span>|<span data-ttu-id="7baca-306">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-306">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="7baca-307">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-307">iBooksStoreBlocked</span></span>|<span data-ttu-id="7baca-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-308">Boolean</span></span>|<span data-ttu-id="7baca-309">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-309">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7baca-310">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="7baca-310">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="7baca-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-311">Boolean</span></span>|<span data-ttu-id="7baca-312">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="7baca-312">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="7baca-313">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="7baca-313">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="7baca-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-314">Boolean</span></span>|<span data-ttu-id="7baca-315">Indica se o usuário deve ou não bloquear o trabalho contínuo iniciado no dispositivo iOS para outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="7baca-315">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="7baca-316">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="7baca-316">iCloudBlockBackup</span></span>|<span data-ttu-id="7baca-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-317">Boolean</span></span>|<span data-ttu-id="7baca-318">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7baca-318">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="7baca-319">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7baca-319">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="7baca-320">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="7baca-320">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="7baca-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-321">Boolean</span></span>|<span data-ttu-id="7baca-322">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueado. Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7baca-322">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="7baca-323">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="7baca-323">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="7baca-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-324">Boolean</span></span>|<span data-ttu-id="7baca-325">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7baca-325">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="7baca-326">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="7baca-326">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="7baca-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-327">Boolean</span></span>|<span data-ttu-id="7baca-328">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7baca-328">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="7baca-329">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="7baca-329">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="7baca-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-330">Boolean</span></span>|<span data-ttu-id="7baca-331">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7baca-331">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="7baca-332">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="7baca-332">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="7baca-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-333">Boolean</span></span>|<span data-ttu-id="7baca-334">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7baca-334">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="7baca-335">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="7baca-335">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="7baca-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-336">Boolean</span></span>|<span data-ttu-id="7baca-337">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="7baca-337">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="7baca-338">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="7baca-338">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="7baca-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-339">Boolean</span></span>|<span data-ttu-id="7baca-340">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="7baca-340">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="7baca-341">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7baca-341">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="7baca-342">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="7baca-342">iTunesBlockMusicService</span></span>|<span data-ttu-id="7baca-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-343">Boolean</span></span>|<span data-ttu-id="7baca-344">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-344">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="7baca-345">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="7baca-345">iTunesBlockRadio</span></span>|<span data-ttu-id="7baca-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-346">Boolean</span></span>|<span data-ttu-id="7baca-347">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-347">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="7baca-348">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="7baca-348">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="7baca-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-349">Boolean</span></span>|<span data-ttu-id="7baca-350">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-350">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="7baca-351">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="7baca-351">keyboardBlockDictation</span></span>|<span data-ttu-id="7baca-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-352">Boolean</span></span>|<span data-ttu-id="7baca-353">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-353">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="7baca-354">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="7baca-354">keyboardBlockPredictive</span></span>|<span data-ttu-id="7baca-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-355">Boolean</span></span>|<span data-ttu-id="7baca-356">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-356">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="7baca-357">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="7baca-357">keyboardBlockShortcuts</span></span>|<span data-ttu-id="7baca-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-358">Boolean</span></span>|<span data-ttu-id="7baca-359">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-359">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7baca-360">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="7baca-360">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="7baca-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-361">Boolean</span></span>|<span data-ttu-id="7baca-362">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-362">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="7baca-363">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="7baca-363">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="7baca-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-364">Boolean</span></span>|<span data-ttu-id="7baca-365">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-365">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="7baca-366">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="7baca-366">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="7baca-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-367">Boolean</span></span>|<span data-ttu-id="7baca-368">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-368">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="7baca-369">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="7baca-369">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="7baca-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-370">Boolean</span></span>|<span data-ttu-id="7baca-371">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-371">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="7baca-372">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="7baca-372">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="7baca-373">Em vez disso, use KioskModeBlockAutoLock.</span><span class="sxs-lookup"><span data-stu-id="7baca-373">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="7baca-374">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="7baca-374">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="7baca-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-375">Boolean</span></span>|<span data-ttu-id="7baca-376">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-376">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="7baca-377">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="7baca-377">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="7baca-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-378">Boolean</span></span>|<span data-ttu-id="7baca-379">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-379">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="7baca-380">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="7baca-380">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="7baca-381">Use KioskModeBlockRingerSwitch.</span><span class="sxs-lookup"><span data-stu-id="7baca-381">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="7baca-382">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="7baca-382">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="7baca-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-383">Boolean</span></span>|<span data-ttu-id="7baca-384">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-384">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="7baca-385">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="7baca-385">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="7baca-386">Use KioskModeBlockScreenRotation em vez disso.</span><span class="sxs-lookup"><span data-stu-id="7baca-386">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="7baca-387">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="7baca-387">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="7baca-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-388">Boolean</span></span>|<span data-ttu-id="7baca-389">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-389">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="7baca-390">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="7baca-390">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="7baca-391">Use KioskModeBlockSleepButton em vez disso.</span><span class="sxs-lookup"><span data-stu-id="7baca-391">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="7baca-392">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="7baca-392">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="7baca-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-393">Boolean</span></span>|<span data-ttu-id="7baca-394">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-394">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="7baca-395">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="7baca-395">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="7baca-396">Use KioskModeBlockTouchscreen em vez disso.</span><span class="sxs-lookup"><span data-stu-id="7baca-396">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="7baca-397">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="7baca-397">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="7baca-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-398">Boolean</span></span>|<span data-ttu-id="7baca-399">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-399">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="7baca-400">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="7baca-400">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="7baca-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-401">Boolean</span></span>|<span data-ttu-id="7baca-402">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-402">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="7baca-403">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="7baca-403">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="7baca-404">Use KioskModeBlockVolumeButtons.</span><span class="sxs-lookup"><span data-stu-id="7baca-404">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="7baca-405">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="7baca-405">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="7baca-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-406">Boolean</span></span>|<span data-ttu-id="7baca-407">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-407">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="7baca-408">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7baca-408">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="7baca-409">String</span><span class="sxs-lookup"><span data-stu-id="7baca-409">String</span></span>|<span data-ttu-id="7baca-410">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-410">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="7baca-411">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="7baca-411">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="7baca-412">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="7baca-412">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="7baca-413">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7baca-413">String</span></span>|<span data-ttu-id="7baca-414">ID para aplicativos integrados a usar no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-414">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="7baca-415">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não estão definidos.</span><span class="sxs-lookup"><span data-stu-id="7baca-415">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="7baca-416">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="7baca-416">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="7baca-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-417">Boolean</span></span>|<span data-ttu-id="7baca-418">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-418">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="7baca-419">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="7baca-419">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="7baca-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-420">Boolean</span></span>|<span data-ttu-id="7baca-421">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-421">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="7baca-422">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="7baca-422">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="7baca-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-423">Boolean</span></span>|<span data-ttu-id="7baca-424">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-424">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="7baca-425">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="7baca-425">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="7baca-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-426">Boolean</span></span>|<span data-ttu-id="7baca-427">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-427">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="7baca-428">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="7baca-428">kioskModeRequireZoom</span></span>|<span data-ttu-id="7baca-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-429">Boolean</span></span>|<span data-ttu-id="7baca-430">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-430">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="7baca-431">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="7baca-431">kioskModeManagedAppId</span></span>|<span data-ttu-id="7baca-432">String</span><span class="sxs-lookup"><span data-stu-id="7baca-432">String</span></span>|<span data-ttu-id="7baca-433">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="7baca-433">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="7baca-434">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="7baca-434">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="7baca-435">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="7baca-435">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="7baca-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-436">Boolean</span></span>|<span data-ttu-id="7baca-437">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="7baca-437">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="7baca-438">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="7baca-438">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="7baca-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-439">Boolean</span></span>|<span data-ttu-id="7baca-440">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="7baca-440">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="7baca-441">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="7baca-441">lockScreenBlockPassbook</span></span>|<span data-ttu-id="7baca-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-442">Boolean</span></span>|<span data-ttu-id="7baca-443">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="7baca-443">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="7baca-444">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="7baca-444">lockScreenBlockTodayView</span></span>|<span data-ttu-id="7baca-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-445">Boolean</span></span>|<span data-ttu-id="7baca-446">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="7baca-446">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="7baca-447">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="7baca-447">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="7baca-448">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="7baca-448">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="7baca-449">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="7baca-449">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="7baca-450">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="7baca-450">mediaContentRatingCanada</span></span>|[<span data-ttu-id="7baca-451">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="7baca-451">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="7baca-452">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="7baca-452">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="7baca-453">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="7baca-453">mediaContentRatingFrance</span></span>|[<span data-ttu-id="7baca-454">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="7baca-454">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="7baca-455">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="7baca-455">Media content rating settings for France</span></span>|
|<span data-ttu-id="7baca-456">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="7baca-456">mediaContentRatingGermany</span></span>|[<span data-ttu-id="7baca-457">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="7baca-457">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="7baca-458">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="7baca-458">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="7baca-459">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="7baca-459">mediaContentRatingIreland</span></span>|[<span data-ttu-id="7baca-460">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="7baca-460">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="7baca-461">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="7baca-461">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="7baca-462">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="7baca-462">mediaContentRatingJapan</span></span>|[<span data-ttu-id="7baca-463">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="7baca-463">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="7baca-464">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="7baca-464">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="7baca-465">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="7baca-465">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="7baca-466">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="7baca-466">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="7baca-467">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="7baca-467">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="7baca-468">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="7baca-468">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="7baca-469">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="7baca-469">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="7baca-470">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="7baca-470">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="7baca-471">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="7baca-471">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="7baca-472">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="7baca-472">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="7baca-473">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="7baca-473">Media content rating settings for United States</span></span>|
|<span data-ttu-id="7baca-474">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="7baca-474">networkUsageRules</span></span>|<span data-ttu-id="7baca-475">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="7baca-475">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="7baca-476">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="7baca-476">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="7baca-477">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="7baca-477">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="7baca-478">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="7baca-478">mediaContentRatingApps</span></span>|[<span data-ttu-id="7baca-479">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="7baca-479">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="7baca-480">Configurações de classificação de conteúdo de mídia para Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="7baca-480">Media content rating settings for Apps.</span></span> <span data-ttu-id="7baca-481">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="7baca-481">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="7baca-482">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-482">messagesBlocked</span></span>|<span data-ttu-id="7baca-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-483">Boolean</span></span>|<span data-ttu-id="7baca-484">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-484">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="7baca-485">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="7baca-485">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="7baca-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-486">Boolean</span></span>|<span data-ttu-id="7baca-487">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-487">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="7baca-488">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="7baca-488">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="7baca-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-489">Boolean</span></span>|<span data-ttu-id="7baca-490">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7baca-490">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="7baca-491">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="7baca-491">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="7baca-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-492">Boolean</span></span>|<span data-ttu-id="7baca-493">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-493">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="7baca-494">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="7baca-494">passcodeBlockModification</span></span>|<span data-ttu-id="7baca-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-495">Boolean</span></span>|<span data-ttu-id="7baca-496">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-496">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="7baca-497">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="7baca-497">passcodeBlockSimple</span></span>|<span data-ttu-id="7baca-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-498">Boolean</span></span>|<span data-ttu-id="7baca-499">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="7baca-499">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="7baca-500">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="7baca-500">passcodeExpirationDays</span></span>|<span data-ttu-id="7baca-501">Int32</span><span class="sxs-lookup"><span data-stu-id="7baca-501">Int32</span></span>|<span data-ttu-id="7baca-502">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="7baca-502">Number of days before the passcode expires.</span></span> <span data-ttu-id="7baca-503">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="7baca-503">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="7baca-504">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="7baca-504">passcodeMinimumLength</span></span>|<span data-ttu-id="7baca-505">Int32</span><span class="sxs-lookup"><span data-stu-id="7baca-505">Int32</span></span>|<span data-ttu-id="7baca-506">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="7baca-506">Minimum length of passcode.</span></span> <span data-ttu-id="7baca-507">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="7baca-507">Valid values 4 to 14</span></span>|
|<span data-ttu-id="7baca-508">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="7baca-508">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="7baca-509">Int32</span><span class="sxs-lookup"><span data-stu-id="7baca-509">Int32</span></span>|<span data-ttu-id="7baca-510">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="7baca-510">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="7baca-511">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="7baca-511">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="7baca-512">Int32</span><span class="sxs-lookup"><span data-stu-id="7baca-512">Int32</span></span>|<span data-ttu-id="7baca-513">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="7baca-513">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="7baca-514">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="7baca-514">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="7baca-515">Int32</span><span class="sxs-lookup"><span data-stu-id="7baca-515">Int32</span></span>|<span data-ttu-id="7baca-516">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="7baca-516">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="7baca-517">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="7baca-517">Valid values 0 to 4</span></span>|
|<span data-ttu-id="7baca-518">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="7baca-518">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="7baca-519">Int32</span><span class="sxs-lookup"><span data-stu-id="7baca-519">Int32</span></span>|<span data-ttu-id="7baca-520">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="7baca-520">Number of previous passcodes to block.</span></span> <span data-ttu-id="7baca-521">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="7baca-521">Valid values 1 to 24</span></span>|
|<span data-ttu-id="7baca-522">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="7baca-522">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="7baca-523">Int32</span><span class="sxs-lookup"><span data-stu-id="7baca-523">Int32</span></span>|<span data-ttu-id="7baca-524">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7baca-524">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="7baca-525">Valores válidos de 2 a 11</span><span class="sxs-lookup"><span data-stu-id="7baca-525">Valid values 2 to 11</span></span>|
|<span data-ttu-id="7baca-526">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="7baca-526">passcodeRequiredType</span></span>|[<span data-ttu-id="7baca-527">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="7baca-527">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="7baca-528">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="7baca-528">Type of passcode that is required.</span></span> <span data-ttu-id="7baca-529">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="7baca-529">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="7baca-530">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="7baca-530">passcodeRequired</span></span>|<span data-ttu-id="7baca-531">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-531">Boolean</span></span>|<span data-ttu-id="7baca-532">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="7baca-532">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="7baca-533">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-533">podcastsBlocked</span></span>|<span data-ttu-id="7baca-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-534">Boolean</span></span>|<span data-ttu-id="7baca-535">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-535">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="7baca-536">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="7baca-536">safariBlockAutofill</span></span>|<span data-ttu-id="7baca-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-537">Boolean</span></span>|<span data-ttu-id="7baca-538">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="7baca-538">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="7baca-539">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7baca-539">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="7baca-540">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="7baca-540">safariBlockJavaScript</span></span>|<span data-ttu-id="7baca-541">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-541">Boolean</span></span>|<span data-ttu-id="7baca-542">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="7baca-542">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="7baca-543">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="7baca-543">safariBlockPopups</span></span>|<span data-ttu-id="7baca-544">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-544">Boolean</span></span>|<span data-ttu-id="7baca-545">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="7baca-545">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="7baca-546">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-546">safariBlocked</span></span>|<span data-ttu-id="7baca-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-547">Boolean</span></span>|<span data-ttu-id="7baca-548">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="7baca-548">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="7baca-549">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="7baca-549">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="7baca-550">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="7baca-550">safariCookieSettings</span></span>|[<span data-ttu-id="7baca-551">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="7baca-551">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="7baca-552">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="7baca-552">Cookie settings for Safari.</span></span> <span data-ttu-id="7baca-553">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="7baca-553">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="7baca-554">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="7baca-554">safariManagedDomains</span></span>|<span data-ttu-id="7baca-555">String collection</span><span class="sxs-lookup"><span data-stu-id="7baca-555">String collection</span></span>|<span data-ttu-id="7baca-556">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="7baca-556">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="7baca-557">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="7baca-557">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="7baca-558">String collection</span><span class="sxs-lookup"><span data-stu-id="7baca-558">String collection</span></span>|<span data-ttu-id="7baca-559">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="7baca-559">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="7baca-560">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-560">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="7baca-561">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="7baca-561">safariRequireFraudWarning</span></span>|<span data-ttu-id="7baca-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-562">Boolean</span></span>|<span data-ttu-id="7baca-563">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="7baca-563">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="7baca-564">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-564">screenCaptureBlocked</span></span>|<span data-ttu-id="7baca-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-565">Boolean</span></span>|<span data-ttu-id="7baca-566">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="7baca-566">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="7baca-567">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-567">siriBlocked</span></span>|<span data-ttu-id="7baca-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-568">Boolean</span></span>|<span data-ttu-id="7baca-569">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="7baca-569">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="7baca-570">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="7baca-570">siriBlockedWhenLocked</span></span>|<span data-ttu-id="7baca-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-571">Boolean</span></span>|<span data-ttu-id="7baca-572">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7baca-572">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="7baca-573">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="7baca-573">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="7baca-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-574">Boolean</span></span>|<span data-ttu-id="7baca-575">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-575">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="7baca-576">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="7baca-576">siriRequireProfanityFilter</span></span>|<span data-ttu-id="7baca-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-577">Boolean</span></span>|<span data-ttu-id="7baca-578">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-578">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="7baca-579">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="7baca-579">spotlightBlockInternetResults</span></span>|<span data-ttu-id="7baca-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-580">Boolean</span></span>|<span data-ttu-id="7baca-581">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-581">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="7baca-582">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="7baca-582">voiceDialingBlocked</span></span>|<span data-ttu-id="7baca-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-583">Boolean</span></span>|<span data-ttu-id="7baca-584">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="7baca-584">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="7baca-585">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="7baca-585">wallpaperBlockModification</span></span>|<span data-ttu-id="7baca-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-586">Boolean</span></span>|<span data-ttu-id="7baca-587">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="7baca-587">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="7baca-588">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="7baca-588">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="7baca-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="7baca-589">Boolean</span></span>|<span data-ttu-id="7baca-590">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="7baca-590">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span> <span data-ttu-id="7baca-591">Disponível para dispositivos que executam versões 14.4 e anteriores do iOS e iPadOS.</span><span class="sxs-lookup"><span data-stu-id="7baca-591">Available for devices running iOS and iPadOS versions 14.4 and earlier.</span></span> <span data-ttu-id="7baca-592">Os dispositivos que executam 14,5+ devem usar a configuração "WiFiConnectToAllowedNetworksOnlyForced.</span><span class="sxs-lookup"><span data-stu-id="7baca-592">Devices running 14.5+ should use the setting, “WiFiConnectToAllowedNetworksOnlyForced.</span></span>|



## <a name="response"></a><span data-ttu-id="7baca-593">Resposta</span><span class="sxs-lookup"><span data-stu-id="7baca-593">Response</span></span>
<span data-ttu-id="7baca-594">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7baca-594">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7baca-595">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7baca-595">Example</span></span>

### <a name="request"></a><span data-ttu-id="7baca-596">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7baca-596">Request</span></span>
<span data-ttu-id="7baca-597">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7baca-597">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7baca-598">Resposta</span><span class="sxs-lookup"><span data-stu-id="7baca-598">Response</span></span>
<span data-ttu-id="7baca-p143">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7baca-p143">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




