---
title: Criar iosGeneralDeviceConfiguration
description: Cria um novo objeto iosGeneralDeviceConfiguration.
author: tfitzmac
ms.openlocfilehash: 0d53f5f5289c21223c0b8e73f0c0eba81bb74731
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332939"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="98810-103">Criar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="98810-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="98810-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="98810-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98810-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="98810-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98810-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="98810-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98810-107">Cria um novo objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="98810-107">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="98810-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98810-108">Prerequisites</span></span>
<span data-ttu-id="98810-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98810-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98810-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98810-111">Permission type</span></span>|<span data-ttu-id="98810-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98810-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98810-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98810-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98810-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98810-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98810-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98810-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98810-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98810-116">Not supported.</span></span>|
|<span data-ttu-id="98810-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98810-117">Application</span></span>|<span data-ttu-id="98810-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98810-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98810-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98810-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="98810-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98810-120">Request headers</span></span>
|<span data-ttu-id="98810-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98810-121">Header</span></span>|<span data-ttu-id="98810-122">Valor</span><span class="sxs-lookup"><span data-stu-id="98810-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98810-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="98810-123">Authorization</span></span>|<span data-ttu-id="98810-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98810-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98810-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98810-125">Accept</span></span>|<span data-ttu-id="98810-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98810-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98810-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98810-127">Request body</span></span>
<span data-ttu-id="98810-128">No corpo da solicitação, forneça uma representação JSON do objeto iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="98810-128">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="98810-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="98810-129">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="98810-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98810-130">Property</span></span>|<span data-ttu-id="98810-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="98810-131">Type</span></span>|<span data-ttu-id="98810-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="98810-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98810-133">id</span><span class="sxs-lookup"><span data-stu-id="98810-133">id</span></span>|<span data-ttu-id="98810-134">String</span><span class="sxs-lookup"><span data-stu-id="98810-134">String</span></span>|<span data-ttu-id="98810-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="98810-135">Key of the entity.</span></span> <span data-ttu-id="98810-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98810-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98810-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98810-137">lastModifiedDateTime</span></span>|<span data-ttu-id="98810-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98810-138">DateTimeOffset</span></span>|<span data-ttu-id="98810-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="98810-139">DateTime the object was last modified.</span></span> <span data-ttu-id="98810-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98810-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98810-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="98810-141">roleScopeTagIds</span></span>|<span data-ttu-id="98810-142">String collection</span><span class="sxs-lookup"><span data-stu-id="98810-142">String collection</span></span>|<span data-ttu-id="98810-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="98810-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="98810-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98810-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98810-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="98810-145">supportsScopeTags</span></span>|<span data-ttu-id="98810-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-146">Boolean</span></span>|<span data-ttu-id="98810-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="98810-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="98810-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="98810-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="98810-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="98810-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="98810-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="98810-150">This property is read-only.</span></span> <span data-ttu-id="98810-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98810-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98810-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98810-152">createdDateTime</span></span>|<span data-ttu-id="98810-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98810-153">DateTimeOffset</span></span>|<span data-ttu-id="98810-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="98810-154">DateTime the object was created.</span></span> <span data-ttu-id="98810-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98810-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98810-156">description</span><span class="sxs-lookup"><span data-stu-id="98810-156">description</span></span>|<span data-ttu-id="98810-157">String</span><span class="sxs-lookup"><span data-stu-id="98810-157">String</span></span>|<span data-ttu-id="98810-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98810-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="98810-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98810-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98810-160">displayName</span><span class="sxs-lookup"><span data-stu-id="98810-160">displayName</span></span>|<span data-ttu-id="98810-161">String</span><span class="sxs-lookup"><span data-stu-id="98810-161">String</span></span>|<span data-ttu-id="98810-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98810-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="98810-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98810-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98810-164">version</span><span class="sxs-lookup"><span data-stu-id="98810-164">version</span></span>|<span data-ttu-id="98810-165">Int32</span><span class="sxs-lookup"><span data-stu-id="98810-165">Int32</span></span>|<span data-ttu-id="98810-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98810-166">Version of the device configuration.</span></span> <span data-ttu-id="98810-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98810-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98810-168">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="98810-168">accountBlockModification</span></span>|<span data-ttu-id="98810-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-169">Boolean</span></span>|<span data-ttu-id="98810-170">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-170">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-171">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="98810-171">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="98810-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-172">Boolean</span></span>|<span data-ttu-id="98810-173">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-173">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="98810-174">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-174">airDropBlocked</span></span>|<span data-ttu-id="98810-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-175">Boolean</span></span>|<span data-ttu-id="98810-176">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-176">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-177">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="98810-177">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="98810-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-178">Boolean</span></span>|<span data-ttu-id="98810-179">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-179">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="98810-180">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="98810-180">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="98810-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-181">Boolean</span></span>|<span data-ttu-id="98810-182">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="98810-182">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="98810-183">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="98810-183">appleWatchBlockPairing</span></span>|<span data-ttu-id="98810-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-184">Boolean</span></span>|<span data-ttu-id="98810-185">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-185">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="98810-186">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="98810-186">appleWatchForceWristDetection</span></span>|<span data-ttu-id="98810-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-187">Boolean</span></span>|<span data-ttu-id="98810-188">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-188">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="98810-189">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-189">appleNewsBlocked</span></span>|<span data-ttu-id="98810-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-190">Boolean</span></span>|<span data-ttu-id="98810-191">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-191">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="98810-192">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="98810-192">appsSingleAppModeList</span></span>|<span data-ttu-id="98810-193">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="98810-193">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="98810-194">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="98810-194">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="98810-195">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-195">Supervised only.</span></span> <span data-ttu-id="98810-196">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="98810-196">iOS 7.0 and later.</span></span> <span data-ttu-id="98810-197">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="98810-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="98810-198">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="98810-198">appsVisibilityList</span></span>|<span data-ttu-id="98810-199">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="98810-199">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="98810-200">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-200">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="98810-201">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="98810-201">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="98810-202">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="98810-202">appsVisibilityListType</span></span>|[<span data-ttu-id="98810-203">appListType</span><span class="sxs-lookup"><span data-stu-id="98810-203">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="98810-204">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="98810-204">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="98810-205">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="98810-205">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="98810-206">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="98810-206">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="98810-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-207">Boolean</span></span>|<span data-ttu-id="98810-208">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-208">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="98810-209">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-209">appStoreBlocked</span></span>|<span data-ttu-id="98810-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-210">Boolean</span></span>|<span data-ttu-id="98810-211">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="98810-211">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="98810-212">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="98810-212">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="98810-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-213">Boolean</span></span>|<span data-ttu-id="98810-214">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98810-214">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="98810-215">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="98810-215">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="98810-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-216">Boolean</span></span>|<span data-ttu-id="98810-217">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="98810-217">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="98810-218">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-218">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="98810-219">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="98810-219">appStoreRequirePassword</span></span>|<span data-ttu-id="98810-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-220">Boolean</span></span>|<span data-ttu-id="98810-221">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="98810-221">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="98810-222">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="98810-222">bluetoothBlockModification</span></span>|<span data-ttu-id="98810-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-223">Boolean</span></span>|<span data-ttu-id="98810-224">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-224">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="98810-225">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-225">cameraBlocked</span></span>|<span data-ttu-id="98810-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-226">Boolean</span></span>|<span data-ttu-id="98810-227">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98810-227">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="98810-228">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="98810-228">cellularBlockDataRoaming</span></span>|<span data-ttu-id="98810-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-229">Boolean</span></span>|<span data-ttu-id="98810-230">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="98810-230">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="98810-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="98810-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="98810-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-232">Boolean</span></span>|<span data-ttu-id="98810-233">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="98810-233">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="98810-234">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="98810-234">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="98810-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-235">Boolean</span></span>|<span data-ttu-id="98810-236">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-236">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-237">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="98810-237">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="98810-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-238">Boolean</span></span>|<span data-ttu-id="98810-239">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="98810-239">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="98810-240">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="98810-240">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="98810-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-241">Boolean</span></span>|<span data-ttu-id="98810-242">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="98810-242">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="98810-243">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="98810-243">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="98810-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-244">Boolean</span></span>|<span data-ttu-id="98810-245">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="98810-245">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="98810-246">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="98810-246">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="98810-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-247">Boolean</span></span>|<span data-ttu-id="98810-248">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-248">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="98810-249">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="98810-249">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="98810-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-250">Boolean</span></span>|<span data-ttu-id="98810-251">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-251">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-252">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="98810-252">compliantAppsList</span></span>|<span data-ttu-id="98810-253">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="98810-253">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="98810-254">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="98810-254">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="98810-255">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="98810-255">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="98810-256">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="98810-256">compliantAppListType</span></span>|[<span data-ttu-id="98810-257">appListType</span><span class="sxs-lookup"><span data-stu-id="98810-257">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="98810-258">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="98810-258">List that is in the AppComplianceList.</span></span> <span data-ttu-id="98810-259">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="98810-259">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="98810-260">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="98810-260">configurationProfileBlockChanges</span></span>|<span data-ttu-id="98810-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-261">Boolean</span></span>|<span data-ttu-id="98810-262">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-262">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-263">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-263">definitionLookupBlocked</span></span>|<span data-ttu-id="98810-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-264">Boolean</span></span>|<span data-ttu-id="98810-265">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-265">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="98810-266">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="98810-266">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="98810-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-267">Boolean</span></span>|<span data-ttu-id="98810-268">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-268">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-269">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="98810-269">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="98810-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-270">Boolean</span></span>|<span data-ttu-id="98810-271">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-271">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-272">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="98810-272">deviceBlockNameModification</span></span>|<span data-ttu-id="98810-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-273">Boolean</span></span>|<span data-ttu-id="98810-274">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-274">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="98810-275">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="98810-275">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="98810-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-276">Boolean</span></span>|<span data-ttu-id="98810-277">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="98810-277">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="98810-278">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="98810-278">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="98810-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-279">Boolean</span></span>|<span data-ttu-id="98810-280">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-280">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="98810-281">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="98810-281">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="98810-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-282">Boolean</span></span>|<span data-ttu-id="98810-283">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="98810-283">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="98810-284">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="98810-284">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="98810-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-285">Boolean</span></span>|<span data-ttu-id="98810-286">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="98810-286">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="98810-287">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="98810-287">emailInDomainSuffixes</span></span>|<span data-ttu-id="98810-288">String collection</span><span class="sxs-lookup"><span data-stu-id="98810-288">String collection</span></span>|<span data-ttu-id="98810-289">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="98810-289">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="98810-290">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="98810-290">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="98810-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-291">Boolean</span></span>|<span data-ttu-id="98810-292">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="98810-292">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="98810-293">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="98810-293">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="98810-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-294">Boolean</span></span>|<span data-ttu-id="98810-295">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="98810-295">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="98810-296">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-296">faceTimeBlocked</span></span>|<span data-ttu-id="98810-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-297">Boolean</span></span>|<span data-ttu-id="98810-298">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="98810-298">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="98810-299">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-299">findMyFriendsBlocked</span></span>|<span data-ttu-id="98810-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-300">Boolean</span></span>|<span data-ttu-id="98810-301">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-301">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-302">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="98810-302">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="98810-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-303">Boolean</span></span>|<span data-ttu-id="98810-304">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="98810-304">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="98810-305">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="98810-305">gamingBlockMultiplayer</span></span>|<span data-ttu-id="98810-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-306">Boolean</span></span>|<span data-ttu-id="98810-307">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="98810-307">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="98810-308">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-308">gameCenterBlocked</span></span>|<span data-ttu-id="98810-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-309">Boolean</span></span>|<span data-ttu-id="98810-310">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-310">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-311">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-311">hostPairingBlocked</span></span>|<span data-ttu-id="98810-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-312">Boolean</span></span>|<span data-ttu-id="98810-313">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-313">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-314">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-314">iBooksStoreBlocked</span></span>|<span data-ttu-id="98810-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-315">Boolean</span></span>|<span data-ttu-id="98810-316">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-316">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-317">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="98810-317">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="98810-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-318">Boolean</span></span>|<span data-ttu-id="98810-319">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="98810-319">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="98810-320">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="98810-320">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="98810-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-321">Boolean</span></span>|<span data-ttu-id="98810-322">Indica se o usuário será ou não impedido de continuar um trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="98810-322">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="98810-323">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="98810-323">iCloudBlockBackup</span></span>|<span data-ttu-id="98810-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-324">Boolean</span></span>|<span data-ttu-id="98810-325">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="98810-325">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="98810-326">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="98810-326">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="98810-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-327">Boolean</span></span>|<span data-ttu-id="98810-328">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98810-328">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="98810-329">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="98810-329">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="98810-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-330">Boolean</span></span>|<span data-ttu-id="98810-331">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98810-331">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="98810-332">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="98810-332">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="98810-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-333">Boolean</span></span>|<span data-ttu-id="98810-334">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98810-334">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="98810-335">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="98810-335">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="98810-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-336">Boolean</span></span>|<span data-ttu-id="98810-337">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98810-337">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="98810-338">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="98810-338">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="98810-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-339">Boolean</span></span>|<span data-ttu-id="98810-340">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98810-340">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="98810-341">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="98810-341">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="98810-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-342">Boolean</span></span>|<span data-ttu-id="98810-343">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="98810-343">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="98810-344">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="98810-344">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="98810-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-345">Boolean</span></span>|<span data-ttu-id="98810-346">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="98810-346">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="98810-347">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="98810-347">iTunesBlockMusicService</span></span>|<span data-ttu-id="98810-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-348">Boolean</span></span>|<span data-ttu-id="98810-349">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-349">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="98810-350">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="98810-350">iTunesBlockRadio</span></span>|<span data-ttu-id="98810-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-351">Boolean</span></span>|<span data-ttu-id="98810-352">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-352">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="98810-353">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="98810-353">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="98810-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-354">Boolean</span></span>|<span data-ttu-id="98810-355">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-355">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="98810-356">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="98810-356">keyboardBlockDictation</span></span>|<span data-ttu-id="98810-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-357">Boolean</span></span>|<span data-ttu-id="98810-358">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-358">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-359">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="98810-359">keyboardBlockPredictive</span></span>|<span data-ttu-id="98810-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-360">Boolean</span></span>|<span data-ttu-id="98810-361">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-361">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="98810-362">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="98810-362">keyboardBlockShortcuts</span></span>|<span data-ttu-id="98810-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-363">Boolean</span></span>|<span data-ttu-id="98810-364">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-364">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="98810-365">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="98810-365">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="98810-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-366">Boolean</span></span>|<span data-ttu-id="98810-367">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-367">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="98810-368">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="98810-368">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="98810-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-369">Boolean</span></span>|<span data-ttu-id="98810-370">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-370">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-371">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="98810-371">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="98810-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-372">Boolean</span></span>|<span data-ttu-id="98810-373">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-373">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-374">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="98810-374">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="98810-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-375">Boolean</span></span>|<span data-ttu-id="98810-376">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-376">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-377">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="98810-377">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="98810-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-378">Boolean</span></span>|<span data-ttu-id="98810-379">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-379">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-380">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="98810-380">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="98810-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-381">Boolean</span></span>|<span data-ttu-id="98810-382">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-382">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-383">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="98810-383">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="98810-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-384">Boolean</span></span>|<span data-ttu-id="98810-385">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-385">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-386">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="98810-386">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="98810-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-387">Boolean</span></span>|<span data-ttu-id="98810-388">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-388">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-389">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="98810-389">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="98810-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-390">Boolean</span></span>|<span data-ttu-id="98810-391">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-391">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-392">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="98810-392">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="98810-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-393">Boolean</span></span>|<span data-ttu-id="98810-394">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-394">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-395">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="98810-395">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="98810-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-396">Boolean</span></span>|<span data-ttu-id="98810-397">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-397">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-398">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="98810-398">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="98810-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-399">Boolean</span></span>|<span data-ttu-id="98810-400">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-400">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="98810-401">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="98810-401">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="98810-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-402">Boolean</span></span>|<span data-ttu-id="98810-403">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-403">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-404">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="98810-404">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="98810-405">String</span><span class="sxs-lookup"><span data-stu-id="98810-405">String</span></span>|<span data-ttu-id="98810-406">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-406">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="98810-407">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="98810-407">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="98810-408">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="98810-408">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="98810-409">String</span><span class="sxs-lookup"><span data-stu-id="98810-409">String</span></span>|<span data-ttu-id="98810-410">ID para aplicativos internos a ser usado para o modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-410">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="98810-411">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidas.</span><span class="sxs-lookup"><span data-stu-id="98810-411">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="98810-412">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="98810-412">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="98810-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-413">Boolean</span></span>|<span data-ttu-id="98810-414">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-414">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-415">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="98810-415">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="98810-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-416">Boolean</span></span>|<span data-ttu-id="98810-417">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-417">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-418">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="98810-418">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="98810-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-419">Boolean</span></span>|<span data-ttu-id="98810-420">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-420">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-421">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="98810-421">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="98810-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-422">Boolean</span></span>|<span data-ttu-id="98810-423">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-423">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-424">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="98810-424">kioskModeRequireZoom</span></span>|<span data-ttu-id="98810-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-425">Boolean</span></span>|<span data-ttu-id="98810-426">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-426">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="98810-427">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="98810-427">kioskModeManagedAppId</span></span>|<span data-ttu-id="98810-428">String</span><span class="sxs-lookup"><span data-stu-id="98810-428">String</span></span>|<span data-ttu-id="98810-429">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="98810-429">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="98810-430">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="98810-430">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="98810-431">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="98810-431">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="98810-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-432">Boolean</span></span>|<span data-ttu-id="98810-433">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="98810-433">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="98810-434">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="98810-434">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="98810-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-435">Boolean</span></span>|<span data-ttu-id="98810-436">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="98810-436">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="98810-437">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="98810-437">lockScreenBlockPassbook</span></span>|<span data-ttu-id="98810-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-438">Boolean</span></span>|<span data-ttu-id="98810-439">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="98810-439">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="98810-440">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="98810-440">lockScreenBlockTodayView</span></span>|<span data-ttu-id="98810-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-441">Boolean</span></span>|<span data-ttu-id="98810-442">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="98810-442">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="98810-443">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="98810-443">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="98810-444">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="98810-444">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="98810-445">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="98810-445">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="98810-446">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="98810-446">mediaContentRatingCanada</span></span>|[<span data-ttu-id="98810-447">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="98810-447">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="98810-448">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="98810-448">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="98810-449">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="98810-449">mediaContentRatingFrance</span></span>|[<span data-ttu-id="98810-450">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="98810-450">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="98810-451">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="98810-451">Media content rating settings for France</span></span>|
|<span data-ttu-id="98810-452">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="98810-452">mediaContentRatingGermany</span></span>|[<span data-ttu-id="98810-453">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="98810-453">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="98810-454">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="98810-454">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="98810-455">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="98810-455">mediaContentRatingIreland</span></span>|[<span data-ttu-id="98810-456">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="98810-456">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="98810-457">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="98810-457">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="98810-458">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="98810-458">mediaContentRatingJapan</span></span>|[<span data-ttu-id="98810-459">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="98810-459">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="98810-460">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="98810-460">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="98810-461">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="98810-461">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="98810-462">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="98810-462">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="98810-463">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="98810-463">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="98810-464">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="98810-464">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="98810-465">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="98810-465">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="98810-466">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="98810-466">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="98810-467">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="98810-467">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="98810-468">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="98810-468">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="98810-469">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="98810-469">Media content rating settings for United States</span></span>|
|<span data-ttu-id="98810-470">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="98810-470">networkUsageRules</span></span>|<span data-ttu-id="98810-471">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="98810-471">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="98810-472">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="98810-472">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="98810-473">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="98810-473">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="98810-474">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="98810-474">mediaContentRatingApps</span></span>|[<span data-ttu-id="98810-475">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="98810-475">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="98810-476">As configurações de classificação para aplicativos de conteúdo de mídia.</span><span class="sxs-lookup"><span data-stu-id="98810-476">Media content rating settings for Apps.</span></span> <span data-ttu-id="98810-477">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="98810-477">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="98810-478">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-478">messagesBlocked</span></span>|<span data-ttu-id="98810-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-479">Boolean</span></span>|<span data-ttu-id="98810-480">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-480">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="98810-481">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="98810-481">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="98810-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-482">Boolean</span></span>|<span data-ttu-id="98810-483">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-483">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="98810-484">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="98810-484">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="98810-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-485">Boolean</span></span>|<span data-ttu-id="98810-486">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="98810-486">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="98810-487">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="98810-487">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="98810-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-488">Boolean</span></span>|<span data-ttu-id="98810-489">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-489">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="98810-490">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="98810-490">passcodeBlockModification</span></span>|<span data-ttu-id="98810-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-491">Boolean</span></span>|<span data-ttu-id="98810-492">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-492">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="98810-493">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="98810-493">passcodeBlockSimple</span></span>|<span data-ttu-id="98810-494">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-494">Boolean</span></span>|<span data-ttu-id="98810-495">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="98810-495">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="98810-496">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="98810-496">passcodeExpirationDays</span></span>|<span data-ttu-id="98810-497">Int32</span><span class="sxs-lookup"><span data-stu-id="98810-497">Int32</span></span>|<span data-ttu-id="98810-498">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="98810-498">Number of days before the passcode expires.</span></span> <span data-ttu-id="98810-499">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="98810-499">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="98810-500">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="98810-500">passcodeMinimumLength</span></span>|<span data-ttu-id="98810-501">Int32</span><span class="sxs-lookup"><span data-stu-id="98810-501">Int32</span></span>|<span data-ttu-id="98810-502">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="98810-502">Minimum length of passcode.</span></span> <span data-ttu-id="98810-503">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="98810-503">Valid values 4 to 14</span></span>|
|<span data-ttu-id="98810-504">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="98810-504">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="98810-505">Int32</span><span class="sxs-lookup"><span data-stu-id="98810-505">Int32</span></span>|<span data-ttu-id="98810-506">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="98810-506">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="98810-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="98810-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="98810-508">Int32</span><span class="sxs-lookup"><span data-stu-id="98810-508">Int32</span></span>|<span data-ttu-id="98810-509">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="98810-509">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="98810-510">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="98810-510">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="98810-511">Int32</span><span class="sxs-lookup"><span data-stu-id="98810-511">Int32</span></span>|<span data-ttu-id="98810-512">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="98810-512">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="98810-513">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="98810-513">Valid values 0 to 4</span></span>|
|<span data-ttu-id="98810-514">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="98810-514">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="98810-515">Int32</span><span class="sxs-lookup"><span data-stu-id="98810-515">Int32</span></span>|<span data-ttu-id="98810-516">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="98810-516">Number of previous passcodes to block.</span></span> <span data-ttu-id="98810-517">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="98810-517">Valid values 1 to 24</span></span>|
|<span data-ttu-id="98810-518">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="98810-518">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="98810-519">Int32</span><span class="sxs-lookup"><span data-stu-id="98810-519">Int32</span></span>|<span data-ttu-id="98810-520">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98810-520">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="98810-521">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="98810-521">Valid values 4 to 11</span></span>|
|<span data-ttu-id="98810-522">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="98810-522">passcodeRequiredType</span></span>|[<span data-ttu-id="98810-523">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="98810-523">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="98810-524">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="98810-524">Type of passcode that is required.</span></span> <span data-ttu-id="98810-525">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="98810-525">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="98810-526">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="98810-526">passcodeRequired</span></span>|<span data-ttu-id="98810-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-527">Boolean</span></span>|<span data-ttu-id="98810-528">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="98810-528">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="98810-529">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-529">podcastsBlocked</span></span>|<span data-ttu-id="98810-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-530">Boolean</span></span>|<span data-ttu-id="98810-531">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-531">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="98810-532">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="98810-532">safariBlockAutofill</span></span>|<span data-ttu-id="98810-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-533">Boolean</span></span>|<span data-ttu-id="98810-534">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="98810-534">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="98810-535">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="98810-535">safariBlockJavaScript</span></span>|<span data-ttu-id="98810-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-536">Boolean</span></span>|<span data-ttu-id="98810-537">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="98810-537">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="98810-538">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="98810-538">safariBlockPopups</span></span>|<span data-ttu-id="98810-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-539">Boolean</span></span>|<span data-ttu-id="98810-540">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="98810-540">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="98810-541">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-541">safariBlocked</span></span>|<span data-ttu-id="98810-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-542">Boolean</span></span>|<span data-ttu-id="98810-543">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="98810-543">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="98810-544">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="98810-544">safariCookieSettings</span></span>|[<span data-ttu-id="98810-545">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="98810-545">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="98810-546">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="98810-546">Cookie settings for Safari.</span></span> <span data-ttu-id="98810-547">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="98810-547">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="98810-548">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="98810-548">safariManagedDomains</span></span>|<span data-ttu-id="98810-549">String collection</span><span class="sxs-lookup"><span data-stu-id="98810-549">String collection</span></span>|<span data-ttu-id="98810-550">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="98810-550">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="98810-551">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="98810-551">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="98810-552">String collection</span><span class="sxs-lookup"><span data-stu-id="98810-552">String collection</span></span>|<span data-ttu-id="98810-553">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="98810-553">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="98810-554">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-554">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="98810-555">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="98810-555">safariRequireFraudWarning</span></span>|<span data-ttu-id="98810-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-556">Boolean</span></span>|<span data-ttu-id="98810-557">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="98810-557">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="98810-558">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-558">screenCaptureBlocked</span></span>|<span data-ttu-id="98810-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-559">Boolean</span></span>|<span data-ttu-id="98810-560">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="98810-560">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="98810-561">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-561">siriBlocked</span></span>|<span data-ttu-id="98810-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-562">Boolean</span></span>|<span data-ttu-id="98810-563">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="98810-563">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="98810-564">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="98810-564">siriBlockedWhenLocked</span></span>|<span data-ttu-id="98810-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-565">Boolean</span></span>|<span data-ttu-id="98810-566">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="98810-566">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="98810-567">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="98810-567">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="98810-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-568">Boolean</span></span>|<span data-ttu-id="98810-569">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-569">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="98810-570">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="98810-570">siriRequireProfanityFilter</span></span>|<span data-ttu-id="98810-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-571">Boolean</span></span>|<span data-ttu-id="98810-572">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-572">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="98810-573">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="98810-573">spotlightBlockInternetResults</span></span>|<span data-ttu-id="98810-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-574">Boolean</span></span>|<span data-ttu-id="98810-575">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-575">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="98810-576">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-576">voiceDialingBlocked</span></span>|<span data-ttu-id="98810-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-577">Boolean</span></span>|<span data-ttu-id="98810-578">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98810-578">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="98810-579">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="98810-579">wallpaperBlockModification</span></span>|<span data-ttu-id="98810-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-580">Boolean</span></span>|<span data-ttu-id="98810-581">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-581">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="98810-582">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="98810-582">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="98810-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-583">Boolean</span></span>|<span data-ttu-id="98810-584">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="98810-584">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="98810-585">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="98810-585">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="98810-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-586">Boolean</span></span>|<span data-ttu-id="98810-587">Indica se um estudante inscrito em um curso não gerenciado por meio da sala de aula solicitará permissão do professor ao tentar deixar o curso (iOS 11.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-587">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="98810-588">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="98810-588">keychainBlockCloudSync</span></span>|<span data-ttu-id="98810-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-589">Boolean</span></span>|<span data-ttu-id="98810-590">Indica se ou não a sincronização do conjunto de chaves iCloud está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98810-590">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="98810-591">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="98810-591">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="98810-592">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-592">Boolean</span></span>|<span data-ttu-id="98810-593">Indica se ou não atualizações PKI via satélite são bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="98810-593">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="98810-594">Definindo essa restrição para false, não desabilite verificações CRL e OCSP (iOS 7.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-594">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="98810-595">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="98810-595">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="98810-596">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-596">Boolean</span></span>|<span data-ttu-id="98810-597">Indica se o anúncio acompanhamento é limitado. (iOS 7.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="98810-597">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="98810-598">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="98810-598">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="98810-599">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-599">Boolean</span></span>|<span data-ttu-id="98810-600">Indica se ou não a empresa livro backup seja bloqueado.</span><span class="sxs-lookup"><span data-stu-id="98810-600">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="98810-601">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="98810-601">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="98810-602">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-602">Boolean</span></span>|<span data-ttu-id="98810-603">Indica se ou não Enterprise catálogo notas e destaques sync está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="98810-603">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="98810-604">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="98810-604">airPrintBlocked</span></span>|<span data-ttu-id="98810-605">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-605">Boolean</span></span>|<span data-ttu-id="98810-606">Indica se é ou não AirPrint bloqueados (iOS 11.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="98810-606">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="98810-607">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="98810-607">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="98810-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-608">Boolean</span></span>|<span data-ttu-id="98810-609">Indica se ou não o armazenamento do conjunto de chaves do usuário e senha para Airprint é bloqueado (iOS 11.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="98810-609">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="98810-610">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="98810-610">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="98810-611">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-611">Boolean</span></span>|<span data-ttu-id="98810-612">Indica se os certificados confiáveis são necessários para a comunicação de impressão de TLS (iOS 11.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="98810-612">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="98810-613">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="98810-613">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="98810-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-614">Boolean</span></span>|<span data-ttu-id="98810-615">Indica se ou não iBeacon descoberta de impressoras AirPrint está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98810-615">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="98810-616">Isso impede que os avisos de AirPrint Bluetooth artificiais contra phishing para tráfego de rede (iOS 11.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="98810-616">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="98810-617">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="98810-617">blockSystemAppRemoval</span></span>|<span data-ttu-id="98810-618">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-618">Boolean</span></span>|<span data-ttu-id="98810-619">Indica se ou não a remoção de aplicativos do sistema do dispositivo seja bloqueada em um dispositivo supervisionado (iOS 11.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="98810-619">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="98810-620">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="98810-620">vpnBlockCreation</span></span>|<span data-ttu-id="98810-621">Boolean</span><span class="sxs-lookup"><span data-stu-id="98810-621">Boolean</span></span>|<span data-ttu-id="98810-622">Indica se é ou não a criação de configurações de VPN bloqueados (iOS 11.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="98810-622">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|



## <a name="response"></a><span data-ttu-id="98810-623">Resposta</span><span class="sxs-lookup"><span data-stu-id="98810-623">Response</span></span>
<span data-ttu-id="98810-624">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98810-624">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98810-625">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98810-625">Example</span></span>
### <a name="request"></a><span data-ttu-id="98810-626">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98810-626">Request</span></span>
<span data-ttu-id="98810-627">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98810-627">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 8496

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "kioskModeBlockVolumeButtons": true,
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
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true
}
```

### <a name="response"></a><span data-ttu-id="98810-628">Resposta</span><span class="sxs-lookup"><span data-stu-id="98810-628">Response</span></span>
<span data-ttu-id="98810-p132">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98810-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 8604

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "kioskModeBlockVolumeButtons": true,
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
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true
}
```





