---
title: Atualizar iosGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto iosGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71a2618af07d459d52c379a27e47f7c251c9d97d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923451"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="ffd95-103">Atualizar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ffd95-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="ffd95-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ffd95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffd95-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ffd95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffd95-106">Atualizar as propriedades de um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffd95-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffd95-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ffd95-107">Prerequisites</span></span>
<span data-ttu-id="ffd95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffd95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffd95-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ffd95-110">Permission type</span></span>|<span data-ttu-id="ffd95-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ffd95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffd95-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ffd95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ffd95-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffd95-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ffd95-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ffd95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffd95-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffd95-115">Not supported.</span></span>|
|<span data-ttu-id="ffd95-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ffd95-116">Application</span></span>|<span data-ttu-id="ffd95-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffd95-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffd95-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ffd95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ffd95-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ffd95-119">Request headers</span></span>
|<span data-ttu-id="ffd95-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ffd95-120">Header</span></span>|<span data-ttu-id="ffd95-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ffd95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffd95-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ffd95-122">Authorization</span></span>|<span data-ttu-id="ffd95-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ffd95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffd95-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ffd95-124">Accept</span></span>|<span data-ttu-id="ffd95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ffd95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffd95-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ffd95-126">Request body</span></span>
<span data-ttu-id="ffd95-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffd95-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="ffd95-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ffd95-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="ffd95-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ffd95-129">Property</span></span>|<span data-ttu-id="ffd95-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffd95-130">Type</span></span>|<span data-ttu-id="ffd95-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffd95-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffd95-132">id</span><span class="sxs-lookup"><span data-stu-id="ffd95-132">id</span></span>|<span data-ttu-id="ffd95-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ffd95-133">String</span></span>|<span data-ttu-id="ffd95-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ffd95-134">Key of the entity.</span></span> <span data-ttu-id="ffd95-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffd95-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd95-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffd95-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ffd95-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffd95-137">DateTimeOffset</span></span>|<span data-ttu-id="ffd95-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ffd95-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ffd95-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffd95-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd95-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ffd95-140">roleScopeTagIds</span></span>|<span data-ttu-id="ffd95-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ffd95-141">String collection</span></span>|<span data-ttu-id="ffd95-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ffd95-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ffd95-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffd95-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd95-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ffd95-144">supportsScopeTags</span></span>|<span data-ttu-id="ffd95-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-145">Boolean</span></span>|<span data-ttu-id="ffd95-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ffd95-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ffd95-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ffd95-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ffd95-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ffd95-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ffd95-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ffd95-149">This property is read-only.</span></span> <span data-ttu-id="ffd95-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffd95-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd95-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffd95-151">createdDateTime</span></span>|<span data-ttu-id="ffd95-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffd95-152">DateTimeOffset</span></span>|<span data-ttu-id="ffd95-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-153">DateTime the object was created.</span></span> <span data-ttu-id="ffd95-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffd95-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd95-155">description</span><span class="sxs-lookup"><span data-stu-id="ffd95-155">description</span></span>|<span data-ttu-id="ffd95-156">String</span><span class="sxs-lookup"><span data-stu-id="ffd95-156">String</span></span>|<span data-ttu-id="ffd95-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ffd95-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ffd95-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffd95-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd95-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ffd95-159">displayName</span></span>|<span data-ttu-id="ffd95-160">String</span><span class="sxs-lookup"><span data-stu-id="ffd95-160">String</span></span>|<span data-ttu-id="ffd95-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ffd95-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ffd95-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffd95-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd95-163">versão</span><span class="sxs-lookup"><span data-stu-id="ffd95-163">version</span></span>|<span data-ttu-id="ffd95-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ffd95-164">Int32</span></span>|<span data-ttu-id="ffd95-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ffd95-165">Version of the device configuration.</span></span> <span data-ttu-id="ffd95-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ffd95-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ffd95-167">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-167">accountBlockModification</span></span>|<span data-ttu-id="ffd95-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-168">Boolean</span></span>|<span data-ttu-id="ffd95-169">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-169">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-170">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="ffd95-170">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="ffd95-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-171">Boolean</span></span>|<span data-ttu-id="ffd95-172">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-172">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="ffd95-173">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-173">airDropBlocked</span></span>|<span data-ttu-id="ffd95-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-174">Boolean</span></span>|<span data-ttu-id="ffd95-175">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-175">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-176">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="ffd95-176">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="ffd95-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-177">Boolean</span></span>|<span data-ttu-id="ffd95-178">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-178">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ffd95-179">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="ffd95-179">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="ffd95-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-180">Boolean</span></span>|<span data-ttu-id="ffd95-181">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="ffd95-181">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="ffd95-182">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="ffd95-182">appleWatchBlockPairing</span></span>|<span data-ttu-id="ffd95-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-183">Boolean</span></span>|<span data-ttu-id="ffd95-184">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-184">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ffd95-185">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="ffd95-185">appleWatchForceWristDetection</span></span>|<span data-ttu-id="ffd95-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-186">Boolean</span></span>|<span data-ttu-id="ffd95-187">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-187">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="ffd95-188">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-188">appleNewsBlocked</span></span>|<span data-ttu-id="ffd95-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-189">Boolean</span></span>|<span data-ttu-id="ffd95-190">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-190">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ffd95-191">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="ffd95-191">appsSingleAppModeList</span></span>|<span data-ttu-id="ffd95-192">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ffd95-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ffd95-193">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="ffd95-193">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="ffd95-194">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-194">Supervised only.</span></span> <span data-ttu-id="ffd95-195">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="ffd95-195">iOS 7.0 and later.</span></span> <span data-ttu-id="ffd95-196">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ffd95-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ffd95-197">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="ffd95-197">appsVisibilityList</span></span>|<span data-ttu-id="ffd95-198">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ffd95-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ffd95-199">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-199">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="ffd95-200">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="ffd95-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ffd95-201">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="ffd95-201">appsVisibilityListType</span></span>|[<span data-ttu-id="ffd95-202">appListType</span><span class="sxs-lookup"><span data-stu-id="ffd95-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="ffd95-203">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="ffd95-203">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="ffd95-204">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="ffd95-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ffd95-205">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="ffd95-205">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="ffd95-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-206">Boolean</span></span>|<span data-ttu-id="ffd95-207">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-207">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ffd95-208">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-208">appStoreBlocked</span></span>|<span data-ttu-id="ffd95-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-209">Boolean</span></span>|<span data-ttu-id="ffd95-210">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="ffd95-210">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="ffd95-211">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="ffd95-211">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="ffd95-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-212">Boolean</span></span>|<span data-ttu-id="ffd95-213">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ffd95-213">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="ffd95-214">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ffd95-214">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="ffd95-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-215">Boolean</span></span>|<span data-ttu-id="ffd95-216">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="ffd95-216">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="ffd95-217">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-217">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ffd95-218">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="ffd95-218">appStoreRequirePassword</span></span>|<span data-ttu-id="ffd95-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-219">Boolean</span></span>|<span data-ttu-id="ffd95-220">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ffd95-220">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="ffd95-221">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="ffd95-221">autoFillForceAuthentication</span></span>|<span data-ttu-id="ffd95-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-222">Boolean</span></span>|<span data-ttu-id="ffd95-223">Indica se a autenticação do usuário deve ou não ser forçada antes de preencher automaticamente as informações de cartão de crédito e o Safari e outros aplicativos em dispositivos supervisionados.</span><span class="sxs-lookup"><span data-stu-id="ffd95-223">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="ffd95-224">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-224">bluetoothBlockModification</span></span>|<span data-ttu-id="ffd95-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffd95-225">Boolean</span></span>|<span data-ttu-id="ffd95-226">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-226">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="ffd95-227">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-227">cameraBlocked</span></span>|<span data-ttu-id="ffd95-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-228">Boolean</span></span>|<span data-ttu-id="ffd95-229">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ffd95-229">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="ffd95-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="ffd95-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="ffd95-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-231">Boolean</span></span>|<span data-ttu-id="ffd95-232">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="ffd95-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="ffd95-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="ffd95-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-234">Boolean</span></span>|<span data-ttu-id="ffd95-235">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="ffd95-235">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="ffd95-236">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-236">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="ffd95-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-237">Boolean</span></span>|<span data-ttu-id="ffd95-238">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-238">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-239">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="ffd95-239">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="ffd95-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-240">Boolean</span></span>|<span data-ttu-id="ffd95-241">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-241">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="ffd95-242">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-242">cellularBlockPlanModification</span></span>|<span data-ttu-id="ffd95-243">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-243">Boolean</span></span>|<span data-ttu-id="ffd95-244">Indica se os usuários poderão ou não alterar as configurações do plano de celular em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-244">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="ffd95-245">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="ffd95-245">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="ffd95-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-246">Boolean</span></span>|<span data-ttu-id="ffd95-247">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-247">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="ffd95-248">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="ffd95-248">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="ffd95-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-249">Boolean</span></span>|<span data-ttu-id="ffd95-250">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="ffd95-250">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="ffd95-251">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ffd95-251">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="ffd95-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-252">Boolean</span></span>|<span data-ttu-id="ffd95-253">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-253">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ffd95-254">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ffd95-254">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="ffd95-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-255">Boolean</span></span>|<span data-ttu-id="ffd95-256">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-256">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-257">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="ffd95-257">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="ffd95-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-258">Boolean</span></span>|<span data-ttu-id="ffd95-259">Indica se a permissão será ou não automaticamente atribuído às solicitações do professor, sem avisar o aluno, quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-259">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-260">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="ffd95-260">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="ffd95-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-261">Boolean</span></span>|<span data-ttu-id="ffd95-262">Indica se o professor deve ou não bloquear aplicativos ou o dispositivo sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="ffd95-262">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="ffd95-263">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-263">Supervised only.</span></span>|
|<span data-ttu-id="ffd95-264">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="ffd95-264">compliantAppsList</span></span>|<span data-ttu-id="ffd95-265">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ffd95-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ffd95-266">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="ffd95-266">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="ffd95-267">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="ffd95-267">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ffd95-268">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="ffd95-268">compliantAppListType</span></span>|[<span data-ttu-id="ffd95-269">appListType</span><span class="sxs-lookup"><span data-stu-id="ffd95-269">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="ffd95-270">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="ffd95-270">List that is in the AppComplianceList.</span></span> <span data-ttu-id="ffd95-271">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="ffd95-271">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ffd95-272">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="ffd95-272">configurationProfileBlockChanges</span></span>|<span data-ttu-id="ffd95-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-273">Boolean</span></span>|<span data-ttu-id="ffd95-274">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-274">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-275">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-275">definitionLookupBlocked</span></span>|<span data-ttu-id="ffd95-276">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-276">Boolean</span></span>|<span data-ttu-id="ffd95-277">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-277">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="ffd95-278">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="ffd95-278">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="ffd95-279">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-279">Boolean</span></span>|<span data-ttu-id="ffd95-280">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-280">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-281">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="ffd95-281">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="ffd95-282">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-282">Boolean</span></span>|<span data-ttu-id="ffd95-283">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-283">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-284">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-284">deviceBlockNameModification</span></span>|<span data-ttu-id="ffd95-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-285">Boolean</span></span>|<span data-ttu-id="ffd95-286">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-286">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ffd95-287">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="ffd95-287">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="ffd95-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-288">Boolean</span></span>|<span data-ttu-id="ffd95-289">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-289">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="ffd95-290">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-290">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="ffd95-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-291">Boolean</span></span>|<span data-ttu-id="ffd95-292">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-292">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="ffd95-293">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="ffd95-293">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="ffd95-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-294">Boolean</span></span>|<span data-ttu-id="ffd95-295">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="ffd95-295">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="ffd95-296">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="ffd95-296">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="ffd95-297">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-297">Boolean</span></span>|<span data-ttu-id="ffd95-298">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="ffd95-298">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="ffd95-299">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="ffd95-299">emailInDomainSuffixes</span></span>|<span data-ttu-id="ffd95-300">String collection</span><span class="sxs-lookup"><span data-stu-id="ffd95-300">String collection</span></span>|<span data-ttu-id="ffd95-301">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="ffd95-301">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="ffd95-302">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="ffd95-302">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="ffd95-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-303">Boolean</span></span>|<span data-ttu-id="ffd95-304">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="ffd95-304">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="ffd95-305">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-305">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="ffd95-306">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-306">Boolean</span></span>|<span data-ttu-id="ffd95-307">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="ffd95-307">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="ffd95-308">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-308">esimBlockModification</span></span>|<span data-ttu-id="ffd95-309">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-309">Boolean</span></span>|<span data-ttu-id="ffd95-310">Indica se a adição ou a remoção de planos da rede celular deve ou não ser permitida no eSIM de um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-310">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="ffd95-311">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-311">faceTimeBlocked</span></span>|<span data-ttu-id="ffd95-312">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-312">Boolean</span></span>|<span data-ttu-id="ffd95-313">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="ffd95-313">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="ffd95-314">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-314">findMyFriendsBlocked</span></span>|<span data-ttu-id="ffd95-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-315">Boolean</span></span>|<span data-ttu-id="ffd95-316">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-316">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-317">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="ffd95-317">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="ffd95-318">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-318">Boolean</span></span>|<span data-ttu-id="ffd95-319">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="ffd95-319">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="ffd95-320">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="ffd95-320">gamingBlockMultiplayer</span></span>|<span data-ttu-id="ffd95-321">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-321">Boolean</span></span>|<span data-ttu-id="ffd95-322">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="ffd95-322">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="ffd95-323">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-323">gameCenterBlocked</span></span>|<span data-ttu-id="ffd95-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffd95-324">Boolean</span></span>|<span data-ttu-id="ffd95-325">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-325">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-326">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-326">hostPairingBlocked</span></span>|<span data-ttu-id="ffd95-327">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-327">Boolean</span></span>|<span data-ttu-id="ffd95-328">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-328">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-329">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-329">iBooksStoreBlocked</span></span>|<span data-ttu-id="ffd95-330">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-330">Boolean</span></span>|<span data-ttu-id="ffd95-331">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-331">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-332">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="ffd95-332">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="ffd95-333">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-333">Boolean</span></span>|<span data-ttu-id="ffd95-334">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="ffd95-334">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="ffd95-335">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="ffd95-335">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="ffd95-336">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-336">Boolean</span></span>|<span data-ttu-id="ffd95-337">Indica se o usuário será ou não impedido de continuar um trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="ffd95-337">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="ffd95-338">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="ffd95-338">iCloudBlockBackup</span></span>|<span data-ttu-id="ffd95-339">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-339">Boolean</span></span>|<span data-ttu-id="ffd95-340">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-340">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="ffd95-341">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="ffd95-341">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="ffd95-342">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-342">Boolean</span></span>|<span data-ttu-id="ffd95-343">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ffd95-343">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="ffd95-344">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="ffd95-344">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="ffd95-345">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-345">Boolean</span></span>|<span data-ttu-id="ffd95-346">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ffd95-346">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="ffd95-347">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="ffd95-347">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="ffd95-348">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-348">Boolean</span></span>|<span data-ttu-id="ffd95-349">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ffd95-349">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="ffd95-350">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="ffd95-350">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="ffd95-351">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-351">Boolean</span></span>|<span data-ttu-id="ffd95-352">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ffd95-352">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="ffd95-353">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="ffd95-353">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="ffd95-354">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-354">Boolean</span></span>|<span data-ttu-id="ffd95-355">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ffd95-355">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="ffd95-356">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="ffd95-356">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="ffd95-357">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-357">Boolean</span></span>|<span data-ttu-id="ffd95-358">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="ffd95-358">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="ffd95-359">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="ffd95-359">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="ffd95-360">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-360">Boolean</span></span>|<span data-ttu-id="ffd95-361">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="ffd95-361">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="ffd95-362">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="ffd95-362">iTunesBlockMusicService</span></span>|<span data-ttu-id="ffd95-363">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-363">Boolean</span></span>|<span data-ttu-id="ffd95-364">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-364">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="ffd95-365">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="ffd95-365">iTunesBlockRadio</span></span>|<span data-ttu-id="ffd95-366">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-366">Boolean</span></span>|<span data-ttu-id="ffd95-367">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-367">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ffd95-368">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="ffd95-368">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="ffd95-369">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-369">Boolean</span></span>|<span data-ttu-id="ffd95-370">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-370">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ffd95-371">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="ffd95-371">keyboardBlockDictation</span></span>|<span data-ttu-id="ffd95-372">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-372">Boolean</span></span>|<span data-ttu-id="ffd95-373">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-373">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-374">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="ffd95-374">keyboardBlockPredictive</span></span>|<span data-ttu-id="ffd95-375">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-375">Boolean</span></span>|<span data-ttu-id="ffd95-376">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-376">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ffd95-377">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="ffd95-377">keyboardBlockShortcuts</span></span>|<span data-ttu-id="ffd95-378">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-378">Boolean</span></span>|<span data-ttu-id="ffd95-379">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-379">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ffd95-380">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="ffd95-380">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="ffd95-381">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-381">Boolean</span></span>|<span data-ttu-id="ffd95-382">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-382">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ffd95-383">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="ffd95-383">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="ffd95-384">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-384">Boolean</span></span>|<span data-ttu-id="ffd95-385">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-385">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-386">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="ffd95-386">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="ffd95-387">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-387">Boolean</span></span>|<span data-ttu-id="ffd95-388">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-388">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-389">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="ffd95-389">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="ffd95-390">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-390">Boolean</span></span>|<span data-ttu-id="ffd95-391">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-391">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="ffd95-392">O funcionalidade desta propriedade é redundante com o padrão do sistema operacional e é preterido.</span><span class="sxs-lookup"><span data-stu-id="ffd95-392">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="ffd95-393">Use KioskModeBlockAutoLock em vez disso.</span><span class="sxs-lookup"><span data-stu-id="ffd95-393">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="ffd95-394">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="ffd95-394">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="ffd95-395">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-395">Boolean</span></span>|<span data-ttu-id="ffd95-396">Indica se o bloqueio automático do dispositivo deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-396">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-397">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="ffd95-397">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="ffd95-398">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-398">Boolean</span></span>|<span data-ttu-id="ffd95-399">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-399">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-400">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="ffd95-400">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="ffd95-401">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-401">Boolean</span></span>|<span data-ttu-id="ffd95-402">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-402">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="ffd95-403">O funcionalidade desta propriedade é redundante com o padrão do sistema operacional e é preterido.</span><span class="sxs-lookup"><span data-stu-id="ffd95-403">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="ffd95-404">Use KioskModeBlockRingerSwitch em vez disso.</span><span class="sxs-lookup"><span data-stu-id="ffd95-404">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="ffd95-405">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="ffd95-405">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="ffd95-406">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-406">Boolean</span></span>|<span data-ttu-id="ffd95-407">Indica se o uso do comutador de toque deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-407">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-408">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="ffd95-408">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="ffd95-409">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-409">Boolean</span></span>|<span data-ttu-id="ffd95-410">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-410">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="ffd95-411">O funcionalidade desta propriedade é redundante com o padrão do sistema operacional e é preterido.</span><span class="sxs-lookup"><span data-stu-id="ffd95-411">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="ffd95-412">Use KioskModeBlockScreenRotation em vez disso.</span><span class="sxs-lookup"><span data-stu-id="ffd95-412">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="ffd95-413">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="ffd95-413">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="ffd95-414">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-414">Boolean</span></span>|<span data-ttu-id="ffd95-415">Indica se a rotação de tela deve ou não ser bloqueada enquanto estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-415">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-416">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="ffd95-416">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="ffd95-417">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-417">Boolean</span></span>|<span data-ttu-id="ffd95-418">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-418">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="ffd95-419">O funcionalidade desta propriedade é redundante com o padrão do sistema operacional e é preterido.</span><span class="sxs-lookup"><span data-stu-id="ffd95-419">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="ffd95-420">Use KioskModeBlockSleepButton em vez disso.</span><span class="sxs-lookup"><span data-stu-id="ffd95-420">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="ffd95-421">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="ffd95-421">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="ffd95-422">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-422">Boolean</span></span>|<span data-ttu-id="ffd95-423">Indica se o uso do botão de suspensão deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-423">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-424">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="ffd95-424">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="ffd95-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffd95-425">Boolean</span></span>|<span data-ttu-id="ffd95-426">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-426">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="ffd95-427">O funcionalidade desta propriedade é redundante com o padrão do sistema operacional e é preterido.</span><span class="sxs-lookup"><span data-stu-id="ffd95-427">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="ffd95-428">Use KioskModeBlockTouchscreen em vez disso.</span><span class="sxs-lookup"><span data-stu-id="ffd95-428">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="ffd95-429">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="ffd95-429">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="ffd95-430">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-430">Boolean</span></span>|<span data-ttu-id="ffd95-431">Indica se o uso da tela de toque deve ou não ser bloqueado enquanto estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-431">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-432">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="ffd95-432">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="ffd95-433">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-433">Boolean</span></span>|<span data-ttu-id="ffd95-434">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-434">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-435">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="ffd95-435">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="ffd95-436">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-436">Boolean</span></span>|<span data-ttu-id="ffd95-437">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-437">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="ffd95-438">O funcionalidade desta propriedade é redundante com o padrão do sistema operacional e é preterido.</span><span class="sxs-lookup"><span data-stu-id="ffd95-438">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="ffd95-439">Use KioskModeBlockVolumeButtons em vez disso.</span><span class="sxs-lookup"><span data-stu-id="ffd95-439">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="ffd95-440">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="ffd95-440">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="ffd95-441">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-441">Boolean</span></span>|<span data-ttu-id="ffd95-442">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-442">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="ffd95-443">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="ffd95-443">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="ffd95-444">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-444">Boolean</span></span>|<span data-ttu-id="ffd95-445">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-445">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-446">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ffd95-446">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="ffd95-447">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ffd95-447">String</span></span>|<span data-ttu-id="ffd95-448">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-448">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="ffd95-449">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="ffd95-449">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="ffd95-450">Propriedadekioskmodebuiltinappid</span><span class="sxs-lookup"><span data-stu-id="ffd95-450">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="ffd95-451">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ffd95-451">String</span></span>|<span data-ttu-id="ffd95-452">ID para aplicativos internos a serem usados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-452">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="ffd95-453">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidos.</span><span class="sxs-lookup"><span data-stu-id="ffd95-453">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="ffd95-454">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="ffd95-454">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="ffd95-455">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-455">Boolean</span></span>|<span data-ttu-id="ffd95-456">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-456">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-457">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="ffd95-457">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="ffd95-458">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-458">Boolean</span></span>|<span data-ttu-id="ffd95-459">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-459">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-460">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="ffd95-460">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="ffd95-461">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-461">Boolean</span></span>|<span data-ttu-id="ffd95-462">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-462">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-463">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="ffd95-463">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="ffd95-464">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-464">Boolean</span></span>|<span data-ttu-id="ffd95-465">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-465">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-466">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="ffd95-466">kioskModeRequireZoom</span></span>|<span data-ttu-id="ffd95-467">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-467">Boolean</span></span>|<span data-ttu-id="ffd95-468">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-468">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="ffd95-469">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="ffd95-469">kioskModeManagedAppId</span></span>|<span data-ttu-id="ffd95-470">String</span><span class="sxs-lookup"><span data-stu-id="ffd95-470">String</span></span>|<span data-ttu-id="ffd95-471">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="ffd95-471">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="ffd95-472">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="ffd95-472">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="ffd95-473">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="ffd95-473">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="ffd95-474">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-474">Boolean</span></span>|<span data-ttu-id="ffd95-475">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="ffd95-475">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="ffd95-476">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="ffd95-476">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="ffd95-477">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-477">Boolean</span></span>|<span data-ttu-id="ffd95-478">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="ffd95-478">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="ffd95-479">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="ffd95-479">lockScreenBlockPassbook</span></span>|<span data-ttu-id="ffd95-480">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-480">Boolean</span></span>|<span data-ttu-id="ffd95-481">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="ffd95-481">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="ffd95-482">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="ffd95-482">lockScreenBlockTodayView</span></span>|<span data-ttu-id="ffd95-483">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-483">Boolean</span></span>|<span data-ttu-id="ffd95-484">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="ffd95-484">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="ffd95-485">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ffd95-485">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="ffd95-486">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ffd95-486">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="ffd95-487">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="ffd95-487">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="ffd95-488">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ffd95-488">mediaContentRatingCanada</span></span>|[<span data-ttu-id="ffd95-489">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ffd95-489">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="ffd95-490">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="ffd95-490">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="ffd95-491">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ffd95-491">mediaContentRatingFrance</span></span>|[<span data-ttu-id="ffd95-492">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ffd95-492">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="ffd95-493">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="ffd95-493">Media content rating settings for France</span></span>|
|<span data-ttu-id="ffd95-494">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ffd95-494">mediaContentRatingGermany</span></span>|[<span data-ttu-id="ffd95-495">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ffd95-495">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="ffd95-496">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="ffd95-496">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="ffd95-497">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ffd95-497">mediaContentRatingIreland</span></span>|[<span data-ttu-id="ffd95-498">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ffd95-498">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="ffd95-499">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="ffd95-499">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="ffd95-500">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ffd95-500">mediaContentRatingJapan</span></span>|[<span data-ttu-id="ffd95-501">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ffd95-501">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="ffd95-502">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="ffd95-502">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="ffd95-503">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ffd95-503">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="ffd95-504">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ffd95-504">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="ffd95-505">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="ffd95-505">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="ffd95-506">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ffd95-506">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="ffd95-507">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ffd95-507">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="ffd95-508">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="ffd95-508">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="ffd95-509">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ffd95-509">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="ffd95-510">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ffd95-510">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="ffd95-511">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="ffd95-511">Media content rating settings for United States</span></span>|
|<span data-ttu-id="ffd95-512">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="ffd95-512">networkUsageRules</span></span>|<span data-ttu-id="ffd95-513">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="ffd95-513">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="ffd95-514">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="ffd95-514">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="ffd95-515">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="ffd95-515">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ffd95-516">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="ffd95-516">mediaContentRatingApps</span></span>|[<span data-ttu-id="ffd95-517">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="ffd95-517">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="ffd95-518">Configurações de classificação de conteúdo de mídia para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ffd95-518">Media content rating settings for Apps.</span></span> <span data-ttu-id="ffd95-519">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="ffd95-519">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="ffd95-520">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-520">messagesBlocked</span></span>|<span data-ttu-id="ffd95-521">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-521">Boolean</span></span>|<span data-ttu-id="ffd95-522">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-522">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="ffd95-523">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-523">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="ffd95-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffd95-524">Boolean</span></span>|<span data-ttu-id="ffd95-525">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-525">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ffd95-526">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="ffd95-526">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="ffd95-527">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-527">Boolean</span></span>|<span data-ttu-id="ffd95-528">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-528">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="ffd95-529">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-529">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="ffd95-530">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-530">Boolean</span></span>|<span data-ttu-id="ffd95-531">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-531">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-532">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-532">passcodeBlockModification</span></span>|<span data-ttu-id="ffd95-533">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-533">Boolean</span></span>|<span data-ttu-id="ffd95-534">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-534">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ffd95-535">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ffd95-535">passcodeBlockSimple</span></span>|<span data-ttu-id="ffd95-536">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-536">Boolean</span></span>|<span data-ttu-id="ffd95-537">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="ffd95-537">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="ffd95-538">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ffd95-538">passcodeExpirationDays</span></span>|<span data-ttu-id="ffd95-539">Int32</span><span class="sxs-lookup"><span data-stu-id="ffd95-539">Int32</span></span>|<span data-ttu-id="ffd95-540">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="ffd95-540">Number of days before the passcode expires.</span></span> <span data-ttu-id="ffd95-541">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="ffd95-541">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="ffd95-542">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ffd95-542">passcodeMinimumLength</span></span>|<span data-ttu-id="ffd95-543">Int32</span><span class="sxs-lookup"><span data-stu-id="ffd95-543">Int32</span></span>|<span data-ttu-id="ffd95-544">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="ffd95-544">Minimum length of passcode.</span></span> <span data-ttu-id="ffd95-545">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="ffd95-545">Valid values 4 to 14</span></span>|
|<span data-ttu-id="ffd95-546">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ffd95-546">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ffd95-547">Int32</span><span class="sxs-lookup"><span data-stu-id="ffd95-547">Int32</span></span>|<span data-ttu-id="ffd95-548">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="ffd95-548">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="ffd95-549">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ffd95-549">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ffd95-550">Int32</span><span class="sxs-lookup"><span data-stu-id="ffd95-550">Int32</span></span>|<span data-ttu-id="ffd95-551">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="ffd95-551">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ffd95-552">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ffd95-552">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="ffd95-553">Int32</span><span class="sxs-lookup"><span data-stu-id="ffd95-553">Int32</span></span>|<span data-ttu-id="ffd95-554">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="ffd95-554">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="ffd95-555">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="ffd95-555">Valid values 0 to 4</span></span>|
|<span data-ttu-id="ffd95-556">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="ffd95-556">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="ffd95-557">Int32</span><span class="sxs-lookup"><span data-stu-id="ffd95-557">Int32</span></span>|<span data-ttu-id="ffd95-558">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="ffd95-558">Number of previous passcodes to block.</span></span> <span data-ttu-id="ffd95-559">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="ffd95-559">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ffd95-560">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="ffd95-560">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="ffd95-561">Int32</span><span class="sxs-lookup"><span data-stu-id="ffd95-561">Int32</span></span>|<span data-ttu-id="ffd95-562">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ffd95-562">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="ffd95-563">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="ffd95-563">Valid values 4 to 11</span></span>|
|<span data-ttu-id="ffd95-564">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="ffd95-564">passcodeRequiredType</span></span>|[<span data-ttu-id="ffd95-565">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ffd95-565">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ffd95-566">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="ffd95-566">Type of passcode that is required.</span></span> <span data-ttu-id="ffd95-567">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ffd95-567">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ffd95-568">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="ffd95-568">passcodeRequired</span></span>|<span data-ttu-id="ffd95-569">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-569">Boolean</span></span>|<span data-ttu-id="ffd95-570">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="ffd95-570">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="ffd95-571">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-571">podcastsBlocked</span></span>|<span data-ttu-id="ffd95-572">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-572">Boolean</span></span>|<span data-ttu-id="ffd95-573">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-573">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="ffd95-574">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="ffd95-574">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="ffd95-575">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-575">Boolean</span></span>|<span data-ttu-id="ffd95-576">Indica se o prompt deve ou não ser habilitado para configurar dispositivos próximos com um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-576">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="ffd95-577">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ffd95-577">safariBlockAutofill</span></span>|<span data-ttu-id="ffd95-578">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-578">Boolean</span></span>|<span data-ttu-id="ffd95-579">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="ffd95-579">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="ffd95-580">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="ffd95-580">safariBlockJavaScript</span></span>|<span data-ttu-id="ffd95-581">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-581">Boolean</span></span>|<span data-ttu-id="ffd95-582">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="ffd95-582">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="ffd95-583">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="ffd95-583">safariBlockPopups</span></span>|<span data-ttu-id="ffd95-584">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-584">Boolean</span></span>|<span data-ttu-id="ffd95-585">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="ffd95-585">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="ffd95-586">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-586">safariBlocked</span></span>|<span data-ttu-id="ffd95-587">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-587">Boolean</span></span>|<span data-ttu-id="ffd95-588">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="ffd95-588">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="ffd95-589">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ffd95-589">safariCookieSettings</span></span>|[<span data-ttu-id="ffd95-590">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ffd95-590">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="ffd95-591">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="ffd95-591">Cookie settings for Safari.</span></span> <span data-ttu-id="ffd95-592">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="ffd95-592">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="ffd95-593">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="ffd95-593">safariManagedDomains</span></span>|<span data-ttu-id="ffd95-594">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ffd95-594">String collection</span></span>|<span data-ttu-id="ffd95-595">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="ffd95-595">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="ffd95-596">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="ffd95-596">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="ffd95-597">String collection</span><span class="sxs-lookup"><span data-stu-id="ffd95-597">String collection</span></span>|<span data-ttu-id="ffd95-598">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="ffd95-598">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="ffd95-599">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-599">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ffd95-600">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="ffd95-600">safariRequireFraudWarning</span></span>|<span data-ttu-id="ffd95-601">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-601">Boolean</span></span>|<span data-ttu-id="ffd95-602">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="ffd95-602">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="ffd95-603">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-603">screenCaptureBlocked</span></span>|<span data-ttu-id="ffd95-604">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-604">Boolean</span></span>|<span data-ttu-id="ffd95-605">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="ffd95-605">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="ffd95-606">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-606">siriBlocked</span></span>|<span data-ttu-id="ffd95-607">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-607">Boolean</span></span>|<span data-ttu-id="ffd95-608">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="ffd95-608">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="ffd95-609">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-609">siriBlockedWhenLocked</span></span>|<span data-ttu-id="ffd95-610">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-610">Boolean</span></span>|<span data-ttu-id="ffd95-611">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-611">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="ffd95-612">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="ffd95-612">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="ffd95-613">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-613">Boolean</span></span>|<span data-ttu-id="ffd95-614">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-614">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="ffd95-615">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="ffd95-615">siriRequireProfanityFilter</span></span>|<span data-ttu-id="ffd95-616">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffd95-616">Boolean</span></span>|<span data-ttu-id="ffd95-617">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-617">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="ffd95-618">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="ffd95-618">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="ffd95-619">Int32</span><span class="sxs-lookup"><span data-stu-id="ffd95-619">Int32</span></span>|<span data-ttu-id="ffd95-620">Define o número de dias que uma atualização de software será delyed para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-620">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="ffd95-621">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="ffd95-621">Valid values 0 to 90</span></span>|
|<span data-ttu-id="ffd95-622">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="ffd95-622">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="ffd95-623">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-623">Boolean</span></span>|<span data-ttu-id="ffd95-624">Indica se o usuário deve ou não atrasar a visibilidade de atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-624">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-625">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="ffd95-625">spotlightBlockInternetResults</span></span>|<span data-ttu-id="ffd95-626">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-626">Boolean</span></span>|<span data-ttu-id="ffd95-627">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-627">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="ffd95-628">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-628">voiceDialingBlocked</span></span>|<span data-ttu-id="ffd95-629">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-629">Boolean</span></span>|<span data-ttu-id="ffd95-630">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ffd95-630">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="ffd95-631">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-631">wallpaperBlockModification</span></span>|<span data-ttu-id="ffd95-632">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-632">Boolean</span></span>|<span data-ttu-id="ffd95-633">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-633">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="ffd95-634">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="ffd95-634">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="ffd95-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffd95-635">Boolean</span></span>|<span data-ttu-id="ffd95-636">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-636">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ffd95-637">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="ffd95-637">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="ffd95-638">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-638">Boolean</span></span>|<span data-ttu-id="ffd95-639">Indica se um aluno inscrito em um curso não gerenciado via sala de aula solicitará permissão do professor ao tentar sair do curso (iOS 11,3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-639">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="ffd95-640">Propriedadeskeychainblockcloudsync</span><span class="sxs-lookup"><span data-stu-id="ffd95-640">keychainBlockCloudSync</span></span>|<span data-ttu-id="ffd95-641">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-641">Boolean</span></span>|<span data-ttu-id="ffd95-642">Indica se a sincronização de chaves do iCloud está bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="ffd95-642">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="ffd95-643">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="ffd95-643">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="ffd95-644">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-644">Boolean</span></span>|<span data-ttu-id="ffd95-645">Indica se as atualizações de PKI de over-the-Air serão bloqueadas ou não.</span><span class="sxs-lookup"><span data-stu-id="ffd95-645">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="ffd95-646">A definição dessa restrição como false não desabilita as verificações de CRL e OCSP (iOS 7,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-646">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="ffd95-647">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="ffd95-647">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="ffd95-648">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-648">Boolean</span></span>|<span data-ttu-id="ffd95-649">Indica se o controle do AD é limitado. (iOS 7,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-649">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="ffd95-650">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="ffd95-650">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="ffd95-651">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-651">Boolean</span></span>|<span data-ttu-id="ffd95-652">Indica se o backup do catálogo empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ffd95-652">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="ffd95-653">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="ffd95-653">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="ffd95-654">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-654">Boolean</span></span>|<span data-ttu-id="ffd95-655">Indica se a sincronização de notas e destaques do catálogo empresarial será bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ffd95-655">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="ffd95-656">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-656">airPrintBlocked</span></span>|<span data-ttu-id="ffd95-657">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-657">Boolean</span></span>|<span data-ttu-id="ffd95-658">Indica se o arquivo de impressão está bloqueado ou não (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-658">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ffd95-659">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="ffd95-659">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="ffd95-660">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-660">Boolean</span></span>|<span data-ttu-id="ffd95-661">Indica se o armazenamento de chaves de nome de usuário e a senha para impressão de uma ou não é bloqueado (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-661">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ffd95-662">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="ffd95-662">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="ffd95-663">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-663">Boolean</span></span>|<span data-ttu-id="ffd95-664">Indica se os certificados confiáveis são necessários para a comunicação de impressão TLS (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-664">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ffd95-665">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="ffd95-665">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="ffd95-666">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-666">Boolean</span></span>|<span data-ttu-id="ffd95-667">Indica se a descoberta de impressoras de impressão do iBeacon está ou não bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ffd95-667">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="ffd95-668">Isso impede os beacons Bluetooth de impressão de mensagens de phishing para tráfego de rede (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-668">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ffd95-669">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="ffd95-669">blockSystemAppRemoval</span></span>|<span data-ttu-id="ffd95-670">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-670">Boolean</span></span>|<span data-ttu-id="ffd95-671">Indica se a remoção de aplicativos do sistema do dispositivo é bloqueada em um dispositivo supervisionado (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-671">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ffd95-672">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="ffd95-672">vpnBlockCreation</span></span>|<span data-ttu-id="ffd95-673">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-673">Boolean</span></span>|<span data-ttu-id="ffd95-674">Indica se a criação de configurações de VPN está bloqueada (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-674">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ffd95-675">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-675">appRemovalBlocked</span></span>|<span data-ttu-id="ffd95-676">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-676">Boolean</span></span>|<span data-ttu-id="ffd95-677">Indica se a remoção de aplicativos é permitida.</span><span class="sxs-lookup"><span data-stu-id="ffd95-677">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="ffd95-678">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="ffd95-678">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="ffd95-679">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-679">Boolean</span></span>|<span data-ttu-id="ffd95-680">Indica se a conexão a acessórios USB enquanto o dispositivo está bloqueado é permitida (iOS 11.4.1 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-680">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="ffd95-681">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="ffd95-681">passwordBlockAutoFill</span></span>|<span data-ttu-id="ffd95-682">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-682">Boolean</span></span>|<span data-ttu-id="ffd95-683">Indica se o recurso de senha de preenchimento automático é permitido (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-683">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ffd95-684">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="ffd95-684">passwordBlockProximityRequests</span></span>|<span data-ttu-id="ffd95-685">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-685">Boolean</span></span>|<span data-ttu-id="ffd95-686">Indica se as senhas de solicitação devem ou não ser bloqueadas de dispositivos próximos (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-686">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ffd95-687">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="ffd95-687">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="ffd95-688">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-688">Boolean</span></span>|<span data-ttu-id="ffd95-689">Indica se as senhas de compartilhamento devem ou não ser bloqueadas com o recurso de senhas de soltura de estours iOS 12,0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="ffd95-689">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ffd95-690">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="ffd95-690">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="ffd95-691">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-691">Boolean</span></span>|<span data-ttu-id="ffd95-692">Indica se o recurso "definir automaticamente" de data e hora está habilitado e não pode ser desativado pelo usuário (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-692">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ffd95-693">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="ffd95-693">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="ffd95-694">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-694">Boolean</span></span>|<span data-ttu-id="ffd95-695">Indica se os aplicativos gerenciados podem ou não gravar contatos para contas de contatos não gerenciados (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-695">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ffd95-696">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="ffd95-696">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="ffd95-697">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-697">Boolean</span></span>|<span data-ttu-id="ffd95-698">Indica se os aplicativos não gerenciados podem ler de contas de contatos gerenciados (iOS 12,0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-698">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="ffd95-699">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="ffd95-699">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="ffd95-700">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-700">Boolean</span></span>|<span data-ttu-id="ffd95-701">Indica se o usuário será ou não impedido de modificar a configuração de hotspot pessoal (iOS 12,2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-701">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="ffd95-702">siriDisableServerLogging</span><span class="sxs-lookup"><span data-stu-id="ffd95-702">siriDisableServerLogging</span></span>|<span data-ttu-id="ffd95-703">Booliano</span><span class="sxs-lookup"><span data-stu-id="ffd95-703">Boolean</span></span>|<span data-ttu-id="ffd95-704">Indica se o registro em log do lado do servidor do Siri está desabilitado (iOS 12,2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ffd95-704">Indicates whether or not server-side Siri logging is disabled (iOS 12.2 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="ffd95-705">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffd95-705">Response</span></span>
<span data-ttu-id="ffd95-706">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ffd95-706">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffd95-707">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ffd95-707">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffd95-708">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ffd95-708">Request</span></span>
<span data-ttu-id="ffd95-709">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ffd95-709">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 9386

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "esimBlockModification": true,
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
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
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
  "proximityBlockSetupToNewDevice": true,
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
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
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
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "siriDisableServerLogging": true
}
```

### <a name="response"></a><span data-ttu-id="ffd95-710">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffd95-710">Response</span></span>
<span data-ttu-id="ffd95-p139">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ffd95-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9558

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
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "esimBlockModification": true,
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
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
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
  "proximityBlockSetupToNewDevice": true,
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
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
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
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "siriDisableServerLogging": true
}
```




