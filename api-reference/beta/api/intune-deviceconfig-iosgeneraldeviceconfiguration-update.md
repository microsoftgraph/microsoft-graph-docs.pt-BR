---
title: Atualizar iosGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto iosGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 590fa8264500fbbf10668a397fafd02247d1eb6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936890"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="b0407-103">Atualizar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0407-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="b0407-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b0407-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0407-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b0407-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0407-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b0407-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0407-107">Atualizar as propriedades de um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0407-107">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0407-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0407-108">Prerequisites</span></span>
<span data-ttu-id="b0407-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0407-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0407-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0407-111">Permission type</span></span>|<span data-ttu-id="b0407-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0407-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0407-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0407-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0407-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0407-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0407-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0407-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0407-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0407-116">Not supported.</span></span>|
|<span data-ttu-id="b0407-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0407-117">Application</span></span>|<span data-ttu-id="b0407-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0407-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0407-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0407-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b0407-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0407-120">Request headers</span></span>
|<span data-ttu-id="b0407-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0407-121">Header</span></span>|<span data-ttu-id="b0407-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b0407-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0407-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0407-123">Authorization</span></span>|<span data-ttu-id="b0407-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0407-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0407-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0407-125">Accept</span></span>|<span data-ttu-id="b0407-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0407-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0407-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0407-127">Request body</span></span>
<span data-ttu-id="b0407-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0407-128">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="b0407-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0407-129">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="b0407-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0407-130">Property</span></span>|<span data-ttu-id="b0407-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0407-131">Type</span></span>|<span data-ttu-id="b0407-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0407-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0407-133">id</span><span class="sxs-lookup"><span data-stu-id="b0407-133">id</span></span>|<span data-ttu-id="b0407-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0407-134">String</span></span>|<span data-ttu-id="b0407-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b0407-135">Key of the entity.</span></span> <span data-ttu-id="b0407-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0407-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0407-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0407-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b0407-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0407-138">DateTimeOffset</span></span>|<span data-ttu-id="b0407-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b0407-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b0407-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0407-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0407-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b0407-141">roleScopeTagIds</span></span>|<span data-ttu-id="b0407-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b0407-142">String collection</span></span>|<span data-ttu-id="b0407-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="b0407-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b0407-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0407-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0407-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b0407-145">supportsScopeTags</span></span>|<span data-ttu-id="b0407-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-146">Boolean</span></span>|<span data-ttu-id="b0407-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b0407-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b0407-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b0407-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b0407-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="b0407-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b0407-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0407-150">This property is read-only.</span></span> <span data-ttu-id="b0407-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0407-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0407-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0407-152">createdDateTime</span></span>|<span data-ttu-id="b0407-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0407-153">DateTimeOffset</span></span>|<span data-ttu-id="b0407-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b0407-154">DateTime the object was created.</span></span> <span data-ttu-id="b0407-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0407-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0407-156">description</span><span class="sxs-lookup"><span data-stu-id="b0407-156">description</span></span>|<span data-ttu-id="b0407-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0407-157">String</span></span>|<span data-ttu-id="b0407-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0407-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b0407-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0407-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0407-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b0407-160">displayName</span></span>|<span data-ttu-id="b0407-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0407-161">String</span></span>|<span data-ttu-id="b0407-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0407-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b0407-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0407-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0407-164">version</span><span class="sxs-lookup"><span data-stu-id="b0407-164">version</span></span>|<span data-ttu-id="b0407-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b0407-165">Int32</span></span>|<span data-ttu-id="b0407-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0407-166">Version of the device configuration.</span></span> <span data-ttu-id="b0407-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0407-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0407-168">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="b0407-168">accountBlockModification</span></span>|<span data-ttu-id="b0407-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-169">Boolean</span></span>|<span data-ttu-id="b0407-170">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-170">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-171">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="b0407-171">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="b0407-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-172">Boolean</span></span>|<span data-ttu-id="b0407-173">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-173">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="b0407-174">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-174">airDropBlocked</span></span>|<span data-ttu-id="b0407-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-175">Boolean</span></span>|<span data-ttu-id="b0407-176">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-176">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-177">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="b0407-177">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="b0407-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-178">Boolean</span></span>|<span data-ttu-id="b0407-179">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-179">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0407-180">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="b0407-180">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="b0407-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-181">Boolean</span></span>|<span data-ttu-id="b0407-182">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="b0407-182">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="b0407-183">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="b0407-183">appleWatchBlockPairing</span></span>|<span data-ttu-id="b0407-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-184">Boolean</span></span>|<span data-ttu-id="b0407-185">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-185">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0407-186">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="b0407-186">appleWatchForceWristDetection</span></span>|<span data-ttu-id="b0407-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-187">Boolean</span></span>|<span data-ttu-id="b0407-188">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-188">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="b0407-189">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-189">appleNewsBlocked</span></span>|<span data-ttu-id="b0407-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-190">Boolean</span></span>|<span data-ttu-id="b0407-191">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-191">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0407-192">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="b0407-192">appsSingleAppModeList</span></span>|<span data-ttu-id="b0407-193">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b0407-193">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b0407-194">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="b0407-194">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="b0407-195">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-195">Supervised only.</span></span> <span data-ttu-id="b0407-196">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="b0407-196">iOS 7.0 and later.</span></span> <span data-ttu-id="b0407-197">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b0407-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b0407-198">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="b0407-198">appsVisibilityList</span></span>|<span data-ttu-id="b0407-199">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b0407-199">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b0407-200">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-200">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="b0407-201">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="b0407-201">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b0407-202">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="b0407-202">appsVisibilityListType</span></span>|[<span data-ttu-id="b0407-203">appListType</span><span class="sxs-lookup"><span data-stu-id="b0407-203">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="b0407-204">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="b0407-204">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="b0407-205">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="b0407-205">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b0407-206">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="b0407-206">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="b0407-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-207">Boolean</span></span>|<span data-ttu-id="b0407-208">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-208">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0407-209">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-209">appStoreBlocked</span></span>|<span data-ttu-id="b0407-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-210">Boolean</span></span>|<span data-ttu-id="b0407-211">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="b0407-211">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="b0407-212">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="b0407-212">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="b0407-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-213">Boolean</span></span>|<span data-ttu-id="b0407-214">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0407-214">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="b0407-215">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b0407-215">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="b0407-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-216">Boolean</span></span>|<span data-ttu-id="b0407-217">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="b0407-217">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="b0407-218">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-218">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0407-219">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="b0407-219">appStoreRequirePassword</span></span>|<span data-ttu-id="b0407-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-220">Boolean</span></span>|<span data-ttu-id="b0407-221">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="b0407-221">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="b0407-222">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="b0407-222">bluetoothBlockModification</span></span>|<span data-ttu-id="b0407-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-223">Boolean</span></span>|<span data-ttu-id="b0407-224">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-224">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="b0407-225">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-225">cameraBlocked</span></span>|<span data-ttu-id="b0407-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-226">Boolean</span></span>|<span data-ttu-id="b0407-227">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0407-227">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="b0407-228">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="b0407-228">cellularBlockDataRoaming</span></span>|<span data-ttu-id="b0407-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-229">Boolean</span></span>|<span data-ttu-id="b0407-230">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b0407-230">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="b0407-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="b0407-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="b0407-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-232">Boolean</span></span>|<span data-ttu-id="b0407-233">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="b0407-233">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="b0407-234">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="b0407-234">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="b0407-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-235">Boolean</span></span>|<span data-ttu-id="b0407-236">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-236">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-237">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="b0407-237">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="b0407-238">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-238">Boolean</span></span>|<span data-ttu-id="b0407-239">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b0407-239">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="b0407-240">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="b0407-240">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="b0407-241">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-241">Boolean</span></span>|<span data-ttu-id="b0407-242">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b0407-242">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="b0407-243">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="b0407-243">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="b0407-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-244">Boolean</span></span>|<span data-ttu-id="b0407-245">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="b0407-245">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="b0407-246">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b0407-246">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="b0407-247">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-247">Boolean</span></span>|<span data-ttu-id="b0407-248">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-248">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b0407-249">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b0407-249">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="b0407-250">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-250">Boolean</span></span>|<span data-ttu-id="b0407-251">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-251">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-252">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="b0407-252">compliantAppsList</span></span>|<span data-ttu-id="b0407-253">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b0407-253">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b0407-254">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="b0407-254">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="b0407-255">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="b0407-255">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b0407-256">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="b0407-256">compliantAppListType</span></span>|[<span data-ttu-id="b0407-257">appListType</span><span class="sxs-lookup"><span data-stu-id="b0407-257">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="b0407-258">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="b0407-258">List that is in the AppComplianceList.</span></span> <span data-ttu-id="b0407-259">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="b0407-259">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b0407-260">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="b0407-260">configurationProfileBlockChanges</span></span>|<span data-ttu-id="b0407-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-261">Boolean</span></span>|<span data-ttu-id="b0407-262">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-262">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-263">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-263">definitionLookupBlocked</span></span>|<span data-ttu-id="b0407-264">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-264">Boolean</span></span>|<span data-ttu-id="b0407-265">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-265">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="b0407-266">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="b0407-266">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="b0407-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-267">Boolean</span></span>|<span data-ttu-id="b0407-268">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-268">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-269">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="b0407-269">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="b0407-270">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-270">Boolean</span></span>|<span data-ttu-id="b0407-271">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-271">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-272">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="b0407-272">deviceBlockNameModification</span></span>|<span data-ttu-id="b0407-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-273">Boolean</span></span>|<span data-ttu-id="b0407-274">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-274">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0407-275">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="b0407-275">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="b0407-276">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-276">Boolean</span></span>|<span data-ttu-id="b0407-277">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b0407-277">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b0407-278">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="b0407-278">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="b0407-279">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-279">Boolean</span></span>|<span data-ttu-id="b0407-280">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-280">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="b0407-281">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="b0407-281">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="b0407-282">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-282">Boolean</span></span>|<span data-ttu-id="b0407-283">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="b0407-283">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="b0407-284">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="b0407-284">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="b0407-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-285">Boolean</span></span>|<span data-ttu-id="b0407-286">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="b0407-286">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="b0407-287">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="b0407-287">emailInDomainSuffixes</span></span>|<span data-ttu-id="b0407-288">String collection</span><span class="sxs-lookup"><span data-stu-id="b0407-288">String collection</span></span>|<span data-ttu-id="b0407-289">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="b0407-289">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="b0407-290">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="b0407-290">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="b0407-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-291">Boolean</span></span>|<span data-ttu-id="b0407-292">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="b0407-292">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="b0407-293">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="b0407-293">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="b0407-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-294">Boolean</span></span>|<span data-ttu-id="b0407-295">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="b0407-295">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="b0407-296">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-296">faceTimeBlocked</span></span>|<span data-ttu-id="b0407-297">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-297">Boolean</span></span>|<span data-ttu-id="b0407-298">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="b0407-298">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="b0407-299">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-299">findMyFriendsBlocked</span></span>|<span data-ttu-id="b0407-300">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-300">Boolean</span></span>|<span data-ttu-id="b0407-301">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-301">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-302">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="b0407-302">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="b0407-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-303">Boolean</span></span>|<span data-ttu-id="b0407-304">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="b0407-304">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="b0407-305">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="b0407-305">gamingBlockMultiplayer</span></span>|<span data-ttu-id="b0407-306">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-306">Boolean</span></span>|<span data-ttu-id="b0407-307">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="b0407-307">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="b0407-308">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-308">gameCenterBlocked</span></span>|<span data-ttu-id="b0407-309">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-309">Boolean</span></span>|<span data-ttu-id="b0407-310">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-310">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-311">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-311">hostPairingBlocked</span></span>|<span data-ttu-id="b0407-312">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-312">Boolean</span></span>|<span data-ttu-id="b0407-313">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-313">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-314">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-314">iBooksStoreBlocked</span></span>|<span data-ttu-id="b0407-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-315">Boolean</span></span>|<span data-ttu-id="b0407-316">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-316">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-317">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="b0407-317">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="b0407-318">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-318">Boolean</span></span>|<span data-ttu-id="b0407-319">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="b0407-319">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="b0407-320">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="b0407-320">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="b0407-321">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-321">Boolean</span></span>|<span data-ttu-id="b0407-322">Indica se o usuário será ou não impedido de continuar um trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="b0407-322">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="b0407-323">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="b0407-323">iCloudBlockBackup</span></span>|<span data-ttu-id="b0407-324">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-324">Boolean</span></span>|<span data-ttu-id="b0407-325">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b0407-325">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="b0407-326">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="b0407-326">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="b0407-327">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-327">Boolean</span></span>|<span data-ttu-id="b0407-328">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b0407-328">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="b0407-329">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="b0407-329">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="b0407-330">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-330">Boolean</span></span>|<span data-ttu-id="b0407-331">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b0407-331">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="b0407-332">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="b0407-332">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="b0407-333">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-333">Boolean</span></span>|<span data-ttu-id="b0407-334">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b0407-334">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="b0407-335">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="b0407-335">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="b0407-336">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-336">Boolean</span></span>|<span data-ttu-id="b0407-337">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b0407-337">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="b0407-338">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="b0407-338">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="b0407-339">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-339">Boolean</span></span>|<span data-ttu-id="b0407-340">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b0407-340">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="b0407-341">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="b0407-341">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="b0407-342">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-342">Boolean</span></span>|<span data-ttu-id="b0407-343">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="b0407-343">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="b0407-344">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="b0407-344">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="b0407-345">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-345">Boolean</span></span>|<span data-ttu-id="b0407-346">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="b0407-346">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="b0407-347">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="b0407-347">iTunesBlockMusicService</span></span>|<span data-ttu-id="b0407-348">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-348">Boolean</span></span>|<span data-ttu-id="b0407-349">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-349">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="b0407-350">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="b0407-350">iTunesBlockRadio</span></span>|<span data-ttu-id="b0407-351">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-351">Boolean</span></span>|<span data-ttu-id="b0407-352">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-352">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b0407-353">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="b0407-353">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="b0407-354">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-354">Boolean</span></span>|<span data-ttu-id="b0407-355">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-355">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b0407-356">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="b0407-356">keyboardBlockDictation</span></span>|<span data-ttu-id="b0407-357">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-357">Boolean</span></span>|<span data-ttu-id="b0407-358">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-358">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-359">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="b0407-359">keyboardBlockPredictive</span></span>|<span data-ttu-id="b0407-360">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-360">Boolean</span></span>|<span data-ttu-id="b0407-361">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-361">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b0407-362">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="b0407-362">keyboardBlockShortcuts</span></span>|<span data-ttu-id="b0407-363">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-363">Boolean</span></span>|<span data-ttu-id="b0407-364">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-364">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0407-365">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="b0407-365">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="b0407-366">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-366">Boolean</span></span>|<span data-ttu-id="b0407-367">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-367">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b0407-368">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="b0407-368">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="b0407-369">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-369">Boolean</span></span>|<span data-ttu-id="b0407-370">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-370">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-371">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="b0407-371">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="b0407-372">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-372">Boolean</span></span>|<span data-ttu-id="b0407-373">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-373">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-374">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="b0407-374">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="b0407-375">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-375">Boolean</span></span>|<span data-ttu-id="b0407-376">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-376">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-377">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="b0407-377">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="b0407-378">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-378">Boolean</span></span>|<span data-ttu-id="b0407-379">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-379">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-380">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="b0407-380">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="b0407-381">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-381">Boolean</span></span>|<span data-ttu-id="b0407-382">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-382">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-383">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="b0407-383">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="b0407-384">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-384">Boolean</span></span>|<span data-ttu-id="b0407-385">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-385">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-386">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="b0407-386">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="b0407-387">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-387">Boolean</span></span>|<span data-ttu-id="b0407-388">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-388">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-389">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="b0407-389">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="b0407-390">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-390">Boolean</span></span>|<span data-ttu-id="b0407-391">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-391">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-392">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="b0407-392">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="b0407-393">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-393">Boolean</span></span>|<span data-ttu-id="b0407-394">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-394">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-395">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="b0407-395">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="b0407-396">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-396">Boolean</span></span>|<span data-ttu-id="b0407-397">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-397">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-398">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="b0407-398">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="b0407-399">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-399">Boolean</span></span>|<span data-ttu-id="b0407-400">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-400">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="b0407-401">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="b0407-401">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="b0407-402">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-402">Boolean</span></span>|<span data-ttu-id="b0407-403">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-403">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-404">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b0407-404">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="b0407-405">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0407-405">String</span></span>|<span data-ttu-id="b0407-406">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-406">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="b0407-407">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="b0407-407">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="b0407-408">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="b0407-408">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="b0407-409">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0407-409">String</span></span>|<span data-ttu-id="b0407-410">ID para aplicativos internos a ser usado para o modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-410">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="b0407-411">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidas.</span><span class="sxs-lookup"><span data-stu-id="b0407-411">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="b0407-412">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="b0407-412">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="b0407-413">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-413">Boolean</span></span>|<span data-ttu-id="b0407-414">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-414">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-415">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="b0407-415">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="b0407-416">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-416">Boolean</span></span>|<span data-ttu-id="b0407-417">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-417">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-418">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="b0407-418">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="b0407-419">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-419">Boolean</span></span>|<span data-ttu-id="b0407-420">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-420">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-421">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="b0407-421">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="b0407-422">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-422">Boolean</span></span>|<span data-ttu-id="b0407-423">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-423">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-424">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="b0407-424">kioskModeRequireZoom</span></span>|<span data-ttu-id="b0407-425">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-425">Boolean</span></span>|<span data-ttu-id="b0407-426">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-426">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="b0407-427">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="b0407-427">kioskModeManagedAppId</span></span>|<span data-ttu-id="b0407-428">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0407-428">String</span></span>|<span data-ttu-id="b0407-429">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="b0407-429">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="b0407-430">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="b0407-430">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="b0407-431">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="b0407-431">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="b0407-432">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-432">Boolean</span></span>|<span data-ttu-id="b0407-433">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="b0407-433">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="b0407-434">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="b0407-434">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="b0407-435">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-435">Boolean</span></span>|<span data-ttu-id="b0407-436">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="b0407-436">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="b0407-437">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="b0407-437">lockScreenBlockPassbook</span></span>|<span data-ttu-id="b0407-438">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-438">Boolean</span></span>|<span data-ttu-id="b0407-439">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="b0407-439">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="b0407-440">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="b0407-440">lockScreenBlockTodayView</span></span>|<span data-ttu-id="b0407-441">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-441">Boolean</span></span>|<span data-ttu-id="b0407-442">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="b0407-442">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="b0407-443">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b0407-443">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="b0407-444">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b0407-444">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="b0407-445">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="b0407-445">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="b0407-446">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b0407-446">mediaContentRatingCanada</span></span>|[<span data-ttu-id="b0407-447">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b0407-447">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="b0407-448">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="b0407-448">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="b0407-449">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b0407-449">mediaContentRatingFrance</span></span>|[<span data-ttu-id="b0407-450">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b0407-450">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="b0407-451">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="b0407-451">Media content rating settings for France</span></span>|
|<span data-ttu-id="b0407-452">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b0407-452">mediaContentRatingGermany</span></span>|[<span data-ttu-id="b0407-453">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b0407-453">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="b0407-454">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="b0407-454">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="b0407-455">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b0407-455">mediaContentRatingIreland</span></span>|[<span data-ttu-id="b0407-456">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b0407-456">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="b0407-457">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="b0407-457">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="b0407-458">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="b0407-458">mediaContentRatingJapan</span></span>|[<span data-ttu-id="b0407-459">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="b0407-459">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="b0407-460">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="b0407-460">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="b0407-461">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b0407-461">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="b0407-462">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b0407-462">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="b0407-463">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="b0407-463">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="b0407-464">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b0407-464">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="b0407-465">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b0407-465">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="b0407-466">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="b0407-466">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="b0407-467">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="b0407-467">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="b0407-468">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="b0407-468">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="b0407-469">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="b0407-469">Media content rating settings for United States</span></span>|
|<span data-ttu-id="b0407-470">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="b0407-470">networkUsageRules</span></span>|<span data-ttu-id="b0407-471">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="b0407-471">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="b0407-472">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="b0407-472">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="b0407-473">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="b0407-473">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="b0407-474">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="b0407-474">mediaContentRatingApps</span></span>|[<span data-ttu-id="b0407-475">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="b0407-475">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="b0407-476">As configurações de classificação para aplicativos de conteúdo de mídia.</span><span class="sxs-lookup"><span data-stu-id="b0407-476">Media content rating settings for Apps.</span></span> <span data-ttu-id="b0407-477">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="b0407-477">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="b0407-478">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-478">messagesBlocked</span></span>|<span data-ttu-id="b0407-479">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-479">Boolean</span></span>|<span data-ttu-id="b0407-480">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-480">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="b0407-481">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="b0407-481">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="b0407-482">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-482">Boolean</span></span>|<span data-ttu-id="b0407-483">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-483">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b0407-484">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="b0407-484">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="b0407-485">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-485">Boolean</span></span>|<span data-ttu-id="b0407-486">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b0407-486">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="b0407-487">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="b0407-487">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="b0407-488">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-488">Boolean</span></span>|<span data-ttu-id="b0407-489">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-489">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="b0407-490">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="b0407-490">passcodeBlockModification</span></span>|<span data-ttu-id="b0407-491">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-491">Boolean</span></span>|<span data-ttu-id="b0407-492">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-492">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b0407-493">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b0407-493">passcodeBlockSimple</span></span>|<span data-ttu-id="b0407-494">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-494">Boolean</span></span>|<span data-ttu-id="b0407-495">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="b0407-495">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="b0407-496">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b0407-496">passcodeExpirationDays</span></span>|<span data-ttu-id="b0407-497">Int32</span><span class="sxs-lookup"><span data-stu-id="b0407-497">Int32</span></span>|<span data-ttu-id="b0407-498">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="b0407-498">Number of days before the passcode expires.</span></span> <span data-ttu-id="b0407-499">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="b0407-499">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b0407-500">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b0407-500">passcodeMinimumLength</span></span>|<span data-ttu-id="b0407-501">Int32</span><span class="sxs-lookup"><span data-stu-id="b0407-501">Int32</span></span>|<span data-ttu-id="b0407-502">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="b0407-502">Minimum length of passcode.</span></span> <span data-ttu-id="b0407-503">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="b0407-503">Valid values 4 to 14</span></span>|
|<span data-ttu-id="b0407-504">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b0407-504">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b0407-505">Int32</span><span class="sxs-lookup"><span data-stu-id="b0407-505">Int32</span></span>|<span data-ttu-id="b0407-506">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="b0407-506">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="b0407-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b0407-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b0407-508">Int32</span><span class="sxs-lookup"><span data-stu-id="b0407-508">Int32</span></span>|<span data-ttu-id="b0407-509">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="b0407-509">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b0407-510">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b0407-510">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="b0407-511">Int32</span><span class="sxs-lookup"><span data-stu-id="b0407-511">Int32</span></span>|<span data-ttu-id="b0407-512">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="b0407-512">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="b0407-513">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="b0407-513">Valid values 0 to 4</span></span>|
|<span data-ttu-id="b0407-514">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="b0407-514">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="b0407-515">Int32</span><span class="sxs-lookup"><span data-stu-id="b0407-515">Int32</span></span>|<span data-ttu-id="b0407-516">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="b0407-516">Number of previous passcodes to block.</span></span> <span data-ttu-id="b0407-517">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="b0407-517">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b0407-518">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="b0407-518">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="b0407-519">Int32</span><span class="sxs-lookup"><span data-stu-id="b0407-519">Int32</span></span>|<span data-ttu-id="b0407-520">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0407-520">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="b0407-521">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="b0407-521">Valid values 4 to 11</span></span>|
|<span data-ttu-id="b0407-522">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="b0407-522">passcodeRequiredType</span></span>|[<span data-ttu-id="b0407-523">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b0407-523">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b0407-524">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="b0407-524">Type of passcode that is required.</span></span> <span data-ttu-id="b0407-525">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b0407-525">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b0407-526">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="b0407-526">passcodeRequired</span></span>|<span data-ttu-id="b0407-527">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-527">Boolean</span></span>|<span data-ttu-id="b0407-528">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="b0407-528">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="b0407-529">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-529">podcastsBlocked</span></span>|<span data-ttu-id="b0407-530">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-530">Boolean</span></span>|<span data-ttu-id="b0407-531">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-531">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="b0407-532">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b0407-532">safariBlockAutofill</span></span>|<span data-ttu-id="b0407-533">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-533">Boolean</span></span>|<span data-ttu-id="b0407-534">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="b0407-534">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="b0407-535">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b0407-535">safariBlockJavaScript</span></span>|<span data-ttu-id="b0407-536">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-536">Boolean</span></span>|<span data-ttu-id="b0407-537">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="b0407-537">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="b0407-538">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b0407-538">safariBlockPopups</span></span>|<span data-ttu-id="b0407-539">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-539">Boolean</span></span>|<span data-ttu-id="b0407-540">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="b0407-540">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="b0407-541">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-541">safariBlocked</span></span>|<span data-ttu-id="b0407-542">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-542">Boolean</span></span>|<span data-ttu-id="b0407-543">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="b0407-543">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="b0407-544">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b0407-544">safariCookieSettings</span></span>|[<span data-ttu-id="b0407-545">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b0407-545">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="b0407-546">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="b0407-546">Cookie settings for Safari.</span></span> <span data-ttu-id="b0407-547">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="b0407-547">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="b0407-548">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="b0407-548">safariManagedDomains</span></span>|<span data-ttu-id="b0407-549">String collection</span><span class="sxs-lookup"><span data-stu-id="b0407-549">String collection</span></span>|<span data-ttu-id="b0407-550">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="b0407-550">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="b0407-551">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="b0407-551">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="b0407-552">String collection</span><span class="sxs-lookup"><span data-stu-id="b0407-552">String collection</span></span>|<span data-ttu-id="b0407-553">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="b0407-553">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="b0407-554">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-554">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b0407-555">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="b0407-555">safariRequireFraudWarning</span></span>|<span data-ttu-id="b0407-556">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-556">Boolean</span></span>|<span data-ttu-id="b0407-557">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="b0407-557">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="b0407-558">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-558">screenCaptureBlocked</span></span>|<span data-ttu-id="b0407-559">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-559">Boolean</span></span>|<span data-ttu-id="b0407-560">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="b0407-560">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="b0407-561">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-561">siriBlocked</span></span>|<span data-ttu-id="b0407-562">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-562">Boolean</span></span>|<span data-ttu-id="b0407-563">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="b0407-563">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="b0407-564">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="b0407-564">siriBlockedWhenLocked</span></span>|<span data-ttu-id="b0407-565">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-565">Boolean</span></span>|<span data-ttu-id="b0407-566">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b0407-566">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="b0407-567">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="b0407-567">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="b0407-568">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-568">Boolean</span></span>|<span data-ttu-id="b0407-569">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-569">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="b0407-570">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="b0407-570">siriRequireProfanityFilter</span></span>|<span data-ttu-id="b0407-571">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-571">Boolean</span></span>|<span data-ttu-id="b0407-572">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-572">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="b0407-573">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="b0407-573">spotlightBlockInternetResults</span></span>|<span data-ttu-id="b0407-574">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-574">Boolean</span></span>|<span data-ttu-id="b0407-575">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-575">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="b0407-576">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-576">voiceDialingBlocked</span></span>|<span data-ttu-id="b0407-577">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-577">Boolean</span></span>|<span data-ttu-id="b0407-578">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b0407-578">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="b0407-579">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="b0407-579">wallpaperBlockModification</span></span>|<span data-ttu-id="b0407-580">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-580">Boolean</span></span>|<span data-ttu-id="b0407-581">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-581">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="b0407-582">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="b0407-582">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="b0407-583">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-583">Boolean</span></span>|<span data-ttu-id="b0407-584">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="b0407-584">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b0407-585">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="b0407-585">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="b0407-586">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-586">Boolean</span></span>|<span data-ttu-id="b0407-587">Indica se um estudante inscrito em um curso não gerenciado por meio da sala de aula solicitará permissão do professor ao tentar deixar o curso (iOS 11.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-587">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="b0407-588">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="b0407-588">keychainBlockCloudSync</span></span>|<span data-ttu-id="b0407-589">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-589">Boolean</span></span>|<span data-ttu-id="b0407-590">Indica se ou não a sincronização do conjunto de chaves iCloud está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b0407-590">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="b0407-591">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="b0407-591">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="b0407-592">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-592">Boolean</span></span>|<span data-ttu-id="b0407-593">Indica se ou não atualizações PKI via satélite são bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="b0407-593">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="b0407-594">Definindo essa restrição para false, não desabilite verificações CRL e OCSP (iOS 7.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-594">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="b0407-595">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="b0407-595">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="b0407-596">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-596">Boolean</span></span>|<span data-ttu-id="b0407-597">Indica se o anúncio acompanhamento é limitado. (iOS 7.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="b0407-597">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="b0407-598">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="b0407-598">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="b0407-599">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-599">Boolean</span></span>|<span data-ttu-id="b0407-600">Indica se ou não a empresa livro backup seja bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b0407-600">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="b0407-601">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="b0407-601">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="b0407-602">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-602">Boolean</span></span>|<span data-ttu-id="b0407-603">Indica se ou não Enterprise catálogo notas e destaques sync está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b0407-603">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="b0407-604">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="b0407-604">airPrintBlocked</span></span>|<span data-ttu-id="b0407-605">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-605">Boolean</span></span>|<span data-ttu-id="b0407-606">Indica se é ou não AirPrint bloqueados (iOS 11.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="b0407-606">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b0407-607">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="b0407-607">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="b0407-608">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-608">Boolean</span></span>|<span data-ttu-id="b0407-609">Indica se ou não o armazenamento do conjunto de chaves do usuário e senha para Airprint é bloqueado (iOS 11.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="b0407-609">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b0407-610">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="b0407-610">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="b0407-611">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-611">Boolean</span></span>|<span data-ttu-id="b0407-612">Indica se os certificados confiáveis são necessários para a comunicação de impressão de TLS (iOS 11.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="b0407-612">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b0407-613">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="b0407-613">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="b0407-614">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-614">Boolean</span></span>|<span data-ttu-id="b0407-615">Indica se ou não iBeacon descoberta de impressoras AirPrint está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b0407-615">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="b0407-616">Isso impede que os avisos de AirPrint Bluetooth artificiais contra phishing para tráfego de rede (iOS 11.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="b0407-616">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b0407-617">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="b0407-617">blockSystemAppRemoval</span></span>|<span data-ttu-id="b0407-618">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-618">Boolean</span></span>|<span data-ttu-id="b0407-619">Indica se ou não a remoção de aplicativos do sistema do dispositivo seja bloqueada em um dispositivo supervisionado (iOS 11.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="b0407-619">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b0407-620">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="b0407-620">vpnBlockCreation</span></span>|<span data-ttu-id="b0407-621">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0407-621">Boolean</span></span>|<span data-ttu-id="b0407-622">Indica se é ou não a criação de configurações de VPN bloqueados (iOS 11.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="b0407-622">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|



## <a name="response"></a><span data-ttu-id="b0407-623">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0407-623">Response</span></span>
<span data-ttu-id="b0407-624">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0407-624">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0407-625">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0407-625">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0407-626">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0407-626">Request</span></span>
<span data-ttu-id="b0407-627">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0407-627">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 8428

{
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

### <a name="response"></a><span data-ttu-id="b0407-628">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0407-628">Response</span></span>
<span data-ttu-id="b0407-p132">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0407-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





