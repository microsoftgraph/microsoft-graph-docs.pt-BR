---
title: Atualizar iosGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto iosGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be9a3efd2ea681e3d774250073b1631a1f04d23a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772801"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="ca132-103">Atualizar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca132-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="ca132-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca132-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca132-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca132-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca132-106">Atualizar as propriedades de um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca132-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca132-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca132-107">Prerequisites</span></span>
<span data-ttu-id="ca132-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca132-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca132-110">Permission type</span></span>|<span data-ttu-id="ca132-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca132-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca132-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca132-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca132-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca132-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca132-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca132-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca132-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca132-115">Not supported.</span></span>|
|<span data-ttu-id="ca132-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca132-116">Application</span></span>|<span data-ttu-id="ca132-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca132-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca132-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca132-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ca132-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca132-119">Request headers</span></span>
|<span data-ttu-id="ca132-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca132-120">Header</span></span>|<span data-ttu-id="ca132-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ca132-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca132-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca132-122">Authorization</span></span>|<span data-ttu-id="ca132-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca132-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca132-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca132-124">Accept</span></span>|<span data-ttu-id="ca132-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca132-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca132-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca132-126">Request body</span></span>
<span data-ttu-id="ca132-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca132-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="ca132-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca132-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="ca132-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca132-129">Property</span></span>|<span data-ttu-id="ca132-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca132-130">Type</span></span>|<span data-ttu-id="ca132-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca132-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca132-132">id</span><span class="sxs-lookup"><span data-stu-id="ca132-132">id</span></span>|<span data-ttu-id="ca132-133">String</span><span class="sxs-lookup"><span data-stu-id="ca132-133">String</span></span>|<span data-ttu-id="ca132-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ca132-134">Key of the entity.</span></span> <span data-ttu-id="ca132-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca132-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca132-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca132-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ca132-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca132-137">DateTimeOffset</span></span>|<span data-ttu-id="ca132-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ca132-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ca132-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca132-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca132-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca132-140">roleScopeTagIds</span></span>|<span data-ttu-id="ca132-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ca132-141">String collection</span></span>|<span data-ttu-id="ca132-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ca132-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ca132-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca132-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca132-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ca132-144">supportsScopeTags</span></span>|<span data-ttu-id="ca132-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-145">Boolean</span></span>|<span data-ttu-id="ca132-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ca132-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ca132-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ca132-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ca132-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ca132-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ca132-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca132-149">This property is read-only.</span></span> <span data-ttu-id="ca132-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca132-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca132-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca132-151">createdDateTime</span></span>|<span data-ttu-id="ca132-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca132-152">DateTimeOffset</span></span>|<span data-ttu-id="ca132-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ca132-153">DateTime the object was created.</span></span> <span data-ttu-id="ca132-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca132-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca132-155">description</span><span class="sxs-lookup"><span data-stu-id="ca132-155">description</span></span>|<span data-ttu-id="ca132-156">String</span><span class="sxs-lookup"><span data-stu-id="ca132-156">String</span></span>|<span data-ttu-id="ca132-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca132-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ca132-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca132-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca132-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ca132-159">displayName</span></span>|<span data-ttu-id="ca132-160">String</span><span class="sxs-lookup"><span data-stu-id="ca132-160">String</span></span>|<span data-ttu-id="ca132-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca132-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ca132-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca132-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca132-163">versão</span><span class="sxs-lookup"><span data-stu-id="ca132-163">version</span></span>|<span data-ttu-id="ca132-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ca132-164">Int32</span></span>|<span data-ttu-id="ca132-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca132-165">Version of the device configuration.</span></span> <span data-ttu-id="ca132-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ca132-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca132-167">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="ca132-167">accountBlockModification</span></span>|<span data-ttu-id="ca132-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-168">Boolean</span></span>|<span data-ttu-id="ca132-169">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-169">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-170">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="ca132-170">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="ca132-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-171">Boolean</span></span>|<span data-ttu-id="ca132-172">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-172">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="ca132-173">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-173">airDropBlocked</span></span>|<span data-ttu-id="ca132-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-174">Boolean</span></span>|<span data-ttu-id="ca132-175">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-175">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-176">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="ca132-176">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="ca132-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-177">Boolean</span></span>|<span data-ttu-id="ca132-178">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-178">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ca132-179">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="ca132-179">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="ca132-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-180">Boolean</span></span>|<span data-ttu-id="ca132-181">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="ca132-181">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="ca132-182">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="ca132-182">appleWatchBlockPairing</span></span>|<span data-ttu-id="ca132-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-183">Boolean</span></span>|<span data-ttu-id="ca132-184">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-184">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ca132-185">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="ca132-185">appleWatchForceWristDetection</span></span>|<span data-ttu-id="ca132-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-186">Boolean</span></span>|<span data-ttu-id="ca132-187">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-187">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="ca132-188">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-188">appleNewsBlocked</span></span>|<span data-ttu-id="ca132-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-189">Boolean</span></span>|<span data-ttu-id="ca132-190">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-190">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ca132-191">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="ca132-191">appsSingleAppModeList</span></span>|<span data-ttu-id="ca132-192">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ca132-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ca132-193">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="ca132-193">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="ca132-194">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-194">Supervised only.</span></span> <span data-ttu-id="ca132-195">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="ca132-195">iOS 7.0 and later.</span></span> <span data-ttu-id="ca132-196">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="ca132-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ca132-197">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="ca132-197">appsVisibilityList</span></span>|<span data-ttu-id="ca132-198">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ca132-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ca132-199">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-199">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="ca132-200">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="ca132-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ca132-201">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="ca132-201">appsVisibilityListType</span></span>|[<span data-ttu-id="ca132-202">appListType</span><span class="sxs-lookup"><span data-stu-id="ca132-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="ca132-203">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="ca132-203">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="ca132-204">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="ca132-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ca132-205">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="ca132-205">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="ca132-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-206">Boolean</span></span>|<span data-ttu-id="ca132-207">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-207">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ca132-208">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-208">appStoreBlocked</span></span>|<span data-ttu-id="ca132-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-209">Boolean</span></span>|<span data-ttu-id="ca132-210">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="ca132-210">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="ca132-211">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="ca132-211">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="ca132-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-212">Boolean</span></span>|<span data-ttu-id="ca132-213">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ca132-213">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="ca132-214">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ca132-214">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="ca132-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-215">Boolean</span></span>|<span data-ttu-id="ca132-216">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="ca132-216">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="ca132-217">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-217">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ca132-218">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="ca132-218">appStoreRequirePassword</span></span>|<span data-ttu-id="ca132-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca132-219">Boolean</span></span>|<span data-ttu-id="ca132-220">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ca132-220">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="ca132-221">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="ca132-221">autoFillForceAuthentication</span></span>|<span data-ttu-id="ca132-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-222">Boolean</span></span>|<span data-ttu-id="ca132-223">Indica se a autenticação do usuário deve ou não ser forçada antes de preencher automaticamente as informações de cartão de crédito e o Safari e outros aplicativos em dispositivos supervisionados.</span><span class="sxs-lookup"><span data-stu-id="ca132-223">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="ca132-224">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="ca132-224">bluetoothBlockModification</span></span>|<span data-ttu-id="ca132-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-225">Boolean</span></span>|<span data-ttu-id="ca132-226">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-226">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="ca132-227">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-227">cameraBlocked</span></span>|<span data-ttu-id="ca132-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-228">Boolean</span></span>|<span data-ttu-id="ca132-229">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca132-229">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="ca132-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="ca132-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="ca132-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-231">Boolean</span></span>|<span data-ttu-id="ca132-232">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ca132-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="ca132-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="ca132-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="ca132-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-234">Boolean</span></span>|<span data-ttu-id="ca132-235">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="ca132-235">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="ca132-236">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="ca132-236">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="ca132-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-237">Boolean</span></span>|<span data-ttu-id="ca132-238">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-238">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-239">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="ca132-239">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="ca132-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-240">Boolean</span></span>|<span data-ttu-id="ca132-241">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ca132-241">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="ca132-242">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="ca132-242">cellularBlockPlanModification</span></span>|<span data-ttu-id="ca132-243">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-243">Boolean</span></span>|<span data-ttu-id="ca132-244">Indica se os usuários poderão ou não alterar as configurações do plano de celular em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-244">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="ca132-245">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="ca132-245">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="ca132-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-246">Boolean</span></span>|<span data-ttu-id="ca132-247">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ca132-247">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="ca132-248">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="ca132-248">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="ca132-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-249">Boolean</span></span>|<span data-ttu-id="ca132-250">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="ca132-250">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="ca132-251">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ca132-251">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="ca132-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-252">Boolean</span></span>|<span data-ttu-id="ca132-253">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-253">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ca132-254">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ca132-254">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="ca132-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-255">Boolean</span></span>|<span data-ttu-id="ca132-256">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-256">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-257">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="ca132-257">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="ca132-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-258">Boolean</span></span>|<span data-ttu-id="ca132-259">Indica se a permissão será ou não automaticamente atribuído às solicitações do professor, sem avisar o aluno, quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-259">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-260">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="ca132-260">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="ca132-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-261">Boolean</span></span>|<span data-ttu-id="ca132-262">Indica se o professor deve ou não bloquear aplicativos ou o dispositivo sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="ca132-262">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="ca132-263">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-263">Supervised only.</span></span>|
|<span data-ttu-id="ca132-264">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="ca132-264">compliantAppsList</span></span>|<span data-ttu-id="ca132-265">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ca132-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ca132-266">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="ca132-266">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="ca132-267">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="ca132-267">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ca132-268">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="ca132-268">compliantAppListType</span></span>|[<span data-ttu-id="ca132-269">appListType</span><span class="sxs-lookup"><span data-stu-id="ca132-269">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="ca132-270">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="ca132-270">List that is in the AppComplianceList.</span></span> <span data-ttu-id="ca132-271">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="ca132-271">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ca132-272">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="ca132-272">configurationProfileBlockChanges</span></span>|<span data-ttu-id="ca132-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-273">Boolean</span></span>|<span data-ttu-id="ca132-274">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-274">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-275">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-275">definitionLookupBlocked</span></span>|<span data-ttu-id="ca132-276">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-276">Boolean</span></span>|<span data-ttu-id="ca132-277">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-277">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="ca132-278">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="ca132-278">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="ca132-279">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-279">Boolean</span></span>|<span data-ttu-id="ca132-280">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-280">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-281">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="ca132-281">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="ca132-282">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-282">Boolean</span></span>|<span data-ttu-id="ca132-283">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-283">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-284">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="ca132-284">deviceBlockNameModification</span></span>|<span data-ttu-id="ca132-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-285">Boolean</span></span>|<span data-ttu-id="ca132-286">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-286">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ca132-287">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="ca132-287">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="ca132-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-288">Boolean</span></span>|<span data-ttu-id="ca132-289">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ca132-289">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="ca132-290">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="ca132-290">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="ca132-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-291">Boolean</span></span>|<span data-ttu-id="ca132-292">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-292">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="ca132-293">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="ca132-293">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="ca132-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-294">Boolean</span></span>|<span data-ttu-id="ca132-295">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="ca132-295">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="ca132-296">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="ca132-296">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="ca132-297">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-297">Boolean</span></span>|<span data-ttu-id="ca132-298">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="ca132-298">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="ca132-299">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="ca132-299">emailInDomainSuffixes</span></span>|<span data-ttu-id="ca132-300">String collection</span><span class="sxs-lookup"><span data-stu-id="ca132-300">String collection</span></span>|<span data-ttu-id="ca132-301">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="ca132-301">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="ca132-302">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="ca132-302">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="ca132-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-303">Boolean</span></span>|<span data-ttu-id="ca132-304">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="ca132-304">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="ca132-305">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="ca132-305">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="ca132-306">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-306">Boolean</span></span>|<span data-ttu-id="ca132-307">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="ca132-307">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="ca132-308">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="ca132-308">esimBlockModification</span></span>|<span data-ttu-id="ca132-309">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-309">Boolean</span></span>|<span data-ttu-id="ca132-310">Indica se a adição ou a remoção de planos da rede celular deve ou não ser permitida no eSIM de um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-310">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="ca132-311">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-311">faceTimeBlocked</span></span>|<span data-ttu-id="ca132-312">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-312">Boolean</span></span>|<span data-ttu-id="ca132-313">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="ca132-313">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="ca132-314">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-314">findMyFriendsBlocked</span></span>|<span data-ttu-id="ca132-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-315">Boolean</span></span>|<span data-ttu-id="ca132-316">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-316">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-317">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="ca132-317">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="ca132-318">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-318">Boolean</span></span>|<span data-ttu-id="ca132-319">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="ca132-319">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="ca132-320">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="ca132-320">gamingBlockMultiplayer</span></span>|<span data-ttu-id="ca132-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca132-321">Boolean</span></span>|<span data-ttu-id="ca132-322">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="ca132-322">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="ca132-323">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-323">gameCenterBlocked</span></span>|<span data-ttu-id="ca132-324">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-324">Boolean</span></span>|<span data-ttu-id="ca132-325">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-325">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-326">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-326">hostPairingBlocked</span></span>|<span data-ttu-id="ca132-327">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-327">Boolean</span></span>|<span data-ttu-id="ca132-328">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-328">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-329">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-329">iBooksStoreBlocked</span></span>|<span data-ttu-id="ca132-330">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-330">Boolean</span></span>|<span data-ttu-id="ca132-331">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-331">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-332">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="ca132-332">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="ca132-333">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-333">Boolean</span></span>|<span data-ttu-id="ca132-334">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="ca132-334">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="ca132-335">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="ca132-335">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="ca132-336">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-336">Boolean</span></span>|<span data-ttu-id="ca132-337">Indica se o usuário será ou não impedido de continuar um trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="ca132-337">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="ca132-338">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="ca132-338">iCloudBlockBackup</span></span>|<span data-ttu-id="ca132-339">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-339">Boolean</span></span>|<span data-ttu-id="ca132-340">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ca132-340">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="ca132-341">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="ca132-341">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="ca132-342">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-342">Boolean</span></span>|<span data-ttu-id="ca132-343">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ca132-343">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="ca132-344">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="ca132-344">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="ca132-345">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-345">Boolean</span></span>|<span data-ttu-id="ca132-346">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ca132-346">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="ca132-347">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="ca132-347">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="ca132-348">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-348">Boolean</span></span>|<span data-ttu-id="ca132-349">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ca132-349">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="ca132-350">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="ca132-350">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="ca132-351">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-351">Boolean</span></span>|<span data-ttu-id="ca132-352">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ca132-352">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="ca132-353">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="ca132-353">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="ca132-354">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-354">Boolean</span></span>|<span data-ttu-id="ca132-355">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ca132-355">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="ca132-356">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="ca132-356">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="ca132-357">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-357">Boolean</span></span>|<span data-ttu-id="ca132-358">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="ca132-358">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="ca132-359">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="ca132-359">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="ca132-360">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-360">Boolean</span></span>|<span data-ttu-id="ca132-361">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="ca132-361">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="ca132-362">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="ca132-362">iTunesBlockMusicService</span></span>|<span data-ttu-id="ca132-363">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-363">Boolean</span></span>|<span data-ttu-id="ca132-364">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-364">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="ca132-365">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="ca132-365">iTunesBlockRadio</span></span>|<span data-ttu-id="ca132-366">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-366">Boolean</span></span>|<span data-ttu-id="ca132-367">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-367">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ca132-368">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="ca132-368">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="ca132-369">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-369">Boolean</span></span>|<span data-ttu-id="ca132-370">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-370">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ca132-371">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="ca132-371">keyboardBlockDictation</span></span>|<span data-ttu-id="ca132-372">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-372">Boolean</span></span>|<span data-ttu-id="ca132-373">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-373">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-374">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="ca132-374">keyboardBlockPredictive</span></span>|<span data-ttu-id="ca132-375">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-375">Boolean</span></span>|<span data-ttu-id="ca132-376">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-376">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ca132-377">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="ca132-377">keyboardBlockShortcuts</span></span>|<span data-ttu-id="ca132-378">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-378">Boolean</span></span>|<span data-ttu-id="ca132-379">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-379">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ca132-380">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="ca132-380">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="ca132-381">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-381">Boolean</span></span>|<span data-ttu-id="ca132-382">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-382">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ca132-383">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="ca132-383">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="ca132-384">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-384">Boolean</span></span>|<span data-ttu-id="ca132-385">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-385">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-386">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="ca132-386">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="ca132-387">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-387">Boolean</span></span>|<span data-ttu-id="ca132-388">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-388">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-389">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="ca132-389">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="ca132-390">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-390">Boolean</span></span>|<span data-ttu-id="ca132-391">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-391">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-392">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="ca132-392">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="ca132-393">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-393">Boolean</span></span>|<span data-ttu-id="ca132-394">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-394">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-395">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="ca132-395">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="ca132-396">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-396">Boolean</span></span>|<span data-ttu-id="ca132-397">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-397">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-398">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="ca132-398">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="ca132-399">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-399">Boolean</span></span>|<span data-ttu-id="ca132-400">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-400">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-401">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="ca132-401">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="ca132-402">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-402">Boolean</span></span>|<span data-ttu-id="ca132-403">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-403">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-404">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="ca132-404">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="ca132-405">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-405">Boolean</span></span>|<span data-ttu-id="ca132-406">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-406">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-407">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="ca132-407">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="ca132-408">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-408">Boolean</span></span>|<span data-ttu-id="ca132-409">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-409">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-410">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="ca132-410">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="ca132-411">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-411">Boolean</span></span>|<span data-ttu-id="ca132-412">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-412">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-413">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="ca132-413">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="ca132-414">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-414">Boolean</span></span>|<span data-ttu-id="ca132-415">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-415">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="ca132-416">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="ca132-416">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="ca132-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca132-417">Boolean</span></span>|<span data-ttu-id="ca132-418">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-418">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-419">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ca132-419">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="ca132-420">String</span><span class="sxs-lookup"><span data-stu-id="ca132-420">String</span></span>|<span data-ttu-id="ca132-421">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-421">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="ca132-422">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="ca132-422">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="ca132-423">Propriedadekioskmodebuiltinappid</span><span class="sxs-lookup"><span data-stu-id="ca132-423">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="ca132-424">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca132-424">String</span></span>|<span data-ttu-id="ca132-425">ID para aplicativos internos a serem usados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-425">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="ca132-426">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidos.</span><span class="sxs-lookup"><span data-stu-id="ca132-426">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="ca132-427">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="ca132-427">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="ca132-428">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-428">Boolean</span></span>|<span data-ttu-id="ca132-429">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-429">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-430">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="ca132-430">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="ca132-431">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-431">Boolean</span></span>|<span data-ttu-id="ca132-432">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-432">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-433">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="ca132-433">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="ca132-434">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-434">Boolean</span></span>|<span data-ttu-id="ca132-435">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-435">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-436">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="ca132-436">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="ca132-437">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-437">Boolean</span></span>|<span data-ttu-id="ca132-438">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-438">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-439">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="ca132-439">kioskModeRequireZoom</span></span>|<span data-ttu-id="ca132-440">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-440">Boolean</span></span>|<span data-ttu-id="ca132-441">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-441">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="ca132-442">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="ca132-442">kioskModeManagedAppId</span></span>|<span data-ttu-id="ca132-443">String</span><span class="sxs-lookup"><span data-stu-id="ca132-443">String</span></span>|<span data-ttu-id="ca132-444">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="ca132-444">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="ca132-445">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="ca132-445">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="ca132-446">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="ca132-446">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="ca132-447">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-447">Boolean</span></span>|<span data-ttu-id="ca132-448">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="ca132-448">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="ca132-449">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="ca132-449">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="ca132-450">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-450">Boolean</span></span>|<span data-ttu-id="ca132-451">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="ca132-451">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="ca132-452">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="ca132-452">lockScreenBlockPassbook</span></span>|<span data-ttu-id="ca132-453">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-453">Boolean</span></span>|<span data-ttu-id="ca132-454">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="ca132-454">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="ca132-455">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="ca132-455">lockScreenBlockTodayView</span></span>|<span data-ttu-id="ca132-456">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-456">Boolean</span></span>|<span data-ttu-id="ca132-457">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="ca132-457">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="ca132-458">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ca132-458">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="ca132-459">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ca132-459">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="ca132-460">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="ca132-460">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="ca132-461">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ca132-461">mediaContentRatingCanada</span></span>|[<span data-ttu-id="ca132-462">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ca132-462">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="ca132-463">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="ca132-463">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="ca132-464">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ca132-464">mediaContentRatingFrance</span></span>|[<span data-ttu-id="ca132-465">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ca132-465">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="ca132-466">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="ca132-466">Media content rating settings for France</span></span>|
|<span data-ttu-id="ca132-467">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ca132-467">mediaContentRatingGermany</span></span>|[<span data-ttu-id="ca132-468">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ca132-468">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="ca132-469">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="ca132-469">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="ca132-470">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ca132-470">mediaContentRatingIreland</span></span>|[<span data-ttu-id="ca132-471">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ca132-471">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="ca132-472">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="ca132-472">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="ca132-473">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ca132-473">mediaContentRatingJapan</span></span>|[<span data-ttu-id="ca132-474">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ca132-474">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="ca132-475">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="ca132-475">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="ca132-476">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ca132-476">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="ca132-477">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ca132-477">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="ca132-478">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="ca132-478">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="ca132-479">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ca132-479">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="ca132-480">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ca132-480">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="ca132-481">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="ca132-481">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="ca132-482">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ca132-482">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="ca132-483">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ca132-483">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="ca132-484">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="ca132-484">Media content rating settings for United States</span></span>|
|<span data-ttu-id="ca132-485">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="ca132-485">networkUsageRules</span></span>|<span data-ttu-id="ca132-486">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="ca132-486">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="ca132-487">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="ca132-487">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="ca132-488">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="ca132-488">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ca132-489">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="ca132-489">mediaContentRatingApps</span></span>|[<span data-ttu-id="ca132-490">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="ca132-490">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="ca132-491">Configurações de classificação de conteúdo de mídia para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ca132-491">Media content rating settings for Apps.</span></span> <span data-ttu-id="ca132-492">Os valores possíveis são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="ca132-492">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="ca132-493">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-493">messagesBlocked</span></span>|<span data-ttu-id="ca132-494">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-494">Boolean</span></span>|<span data-ttu-id="ca132-495">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-495">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="ca132-496">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="ca132-496">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="ca132-497">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-497">Boolean</span></span>|<span data-ttu-id="ca132-498">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-498">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ca132-499">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="ca132-499">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="ca132-500">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-500">Boolean</span></span>|<span data-ttu-id="ca132-501">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ca132-501">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="ca132-502">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="ca132-502">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="ca132-503">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-503">Boolean</span></span>|<span data-ttu-id="ca132-504">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-504">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="ca132-505">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="ca132-505">passcodeBlockModification</span></span>|<span data-ttu-id="ca132-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca132-506">Boolean</span></span>|<span data-ttu-id="ca132-507">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-507">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ca132-508">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ca132-508">passcodeBlockSimple</span></span>|<span data-ttu-id="ca132-509">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-509">Boolean</span></span>|<span data-ttu-id="ca132-510">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="ca132-510">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="ca132-511">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ca132-511">passcodeExpirationDays</span></span>|<span data-ttu-id="ca132-512">Int32</span><span class="sxs-lookup"><span data-stu-id="ca132-512">Int32</span></span>|<span data-ttu-id="ca132-513">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="ca132-513">Number of days before the passcode expires.</span></span> <span data-ttu-id="ca132-514">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="ca132-514">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="ca132-515">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ca132-515">passcodeMinimumLength</span></span>|<span data-ttu-id="ca132-516">Int32</span><span class="sxs-lookup"><span data-stu-id="ca132-516">Int32</span></span>|<span data-ttu-id="ca132-517">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="ca132-517">Minimum length of passcode.</span></span> <span data-ttu-id="ca132-518">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="ca132-518">Valid values 4 to 14</span></span>|
|<span data-ttu-id="ca132-519">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ca132-519">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ca132-520">Int32</span><span class="sxs-lookup"><span data-stu-id="ca132-520">Int32</span></span>|<span data-ttu-id="ca132-521">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="ca132-521">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="ca132-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ca132-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ca132-523">Int32</span><span class="sxs-lookup"><span data-stu-id="ca132-523">Int32</span></span>|<span data-ttu-id="ca132-524">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="ca132-524">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ca132-525">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ca132-525">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="ca132-526">Int32</span><span class="sxs-lookup"><span data-stu-id="ca132-526">Int32</span></span>|<span data-ttu-id="ca132-527">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="ca132-527">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="ca132-528">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="ca132-528">Valid values 0 to 4</span></span>|
|<span data-ttu-id="ca132-529">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="ca132-529">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="ca132-530">Int32</span><span class="sxs-lookup"><span data-stu-id="ca132-530">Int32</span></span>|<span data-ttu-id="ca132-531">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="ca132-531">Number of previous passcodes to block.</span></span> <span data-ttu-id="ca132-532">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="ca132-532">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ca132-533">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="ca132-533">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="ca132-534">Int32</span><span class="sxs-lookup"><span data-stu-id="ca132-534">Int32</span></span>|<span data-ttu-id="ca132-535">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca132-535">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="ca132-536">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="ca132-536">Valid values 4 to 11</span></span>|
|<span data-ttu-id="ca132-537">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="ca132-537">passcodeRequiredType</span></span>|[<span data-ttu-id="ca132-538">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ca132-538">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ca132-539">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="ca132-539">Type of passcode that is required.</span></span> <span data-ttu-id="ca132-540">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ca132-540">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ca132-541">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="ca132-541">passcodeRequired</span></span>|<span data-ttu-id="ca132-542">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-542">Boolean</span></span>|<span data-ttu-id="ca132-543">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="ca132-543">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="ca132-544">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-544">podcastsBlocked</span></span>|<span data-ttu-id="ca132-545">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-545">Boolean</span></span>|<span data-ttu-id="ca132-546">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-546">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="ca132-547">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="ca132-547">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="ca132-548">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-548">Boolean</span></span>|<span data-ttu-id="ca132-549">Indica se o prompt deve ou não ser habilitado para configurar dispositivos próximos com um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-549">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="ca132-550">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ca132-550">safariBlockAutofill</span></span>|<span data-ttu-id="ca132-551">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-551">Boolean</span></span>|<span data-ttu-id="ca132-552">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="ca132-552">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="ca132-553">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="ca132-553">safariBlockJavaScript</span></span>|<span data-ttu-id="ca132-554">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-554">Boolean</span></span>|<span data-ttu-id="ca132-555">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="ca132-555">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="ca132-556">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="ca132-556">safariBlockPopups</span></span>|<span data-ttu-id="ca132-557">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-557">Boolean</span></span>|<span data-ttu-id="ca132-558">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="ca132-558">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="ca132-559">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-559">safariBlocked</span></span>|<span data-ttu-id="ca132-560">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-560">Boolean</span></span>|<span data-ttu-id="ca132-561">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="ca132-561">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="ca132-562">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ca132-562">safariCookieSettings</span></span>|[<span data-ttu-id="ca132-563">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ca132-563">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="ca132-564">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="ca132-564">Cookie settings for Safari.</span></span> <span data-ttu-id="ca132-565">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="ca132-565">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="ca132-566">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="ca132-566">safariManagedDomains</span></span>|<span data-ttu-id="ca132-567">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ca132-567">String collection</span></span>|<span data-ttu-id="ca132-568">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="ca132-568">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="ca132-569">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="ca132-569">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="ca132-570">String collection</span><span class="sxs-lookup"><span data-stu-id="ca132-570">String collection</span></span>|<span data-ttu-id="ca132-571">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="ca132-571">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="ca132-572">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-572">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ca132-573">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="ca132-573">safariRequireFraudWarning</span></span>|<span data-ttu-id="ca132-574">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-574">Boolean</span></span>|<span data-ttu-id="ca132-575">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="ca132-575">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="ca132-576">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-576">screenCaptureBlocked</span></span>|<span data-ttu-id="ca132-577">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-577">Boolean</span></span>|<span data-ttu-id="ca132-578">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="ca132-578">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="ca132-579">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-579">siriBlocked</span></span>|<span data-ttu-id="ca132-580">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-580">Boolean</span></span>|<span data-ttu-id="ca132-581">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="ca132-581">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="ca132-582">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="ca132-582">siriBlockedWhenLocked</span></span>|<span data-ttu-id="ca132-583">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-583">Boolean</span></span>|<span data-ttu-id="ca132-584">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ca132-584">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="ca132-585">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="ca132-585">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="ca132-586">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-586">Boolean</span></span>|<span data-ttu-id="ca132-587">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-587">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="ca132-588">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="ca132-588">siriRequireProfanityFilter</span></span>|<span data-ttu-id="ca132-589">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-589">Boolean</span></span>|<span data-ttu-id="ca132-590">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-590">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="ca132-591">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="ca132-591">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="ca132-592">Int32</span><span class="sxs-lookup"><span data-stu-id="ca132-592">Int32</span></span>|<span data-ttu-id="ca132-593">Define o número de dias que uma atualização de software será delyed para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-593">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="ca132-594">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="ca132-594">Valid values 0 to 90</span></span>|
|<span data-ttu-id="ca132-595">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="ca132-595">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="ca132-596">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-596">Boolean</span></span>|<span data-ttu-id="ca132-597">Indica se o usuário deve ou não atrasar a visibilidade de atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-597">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-598">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="ca132-598">spotlightBlockInternetResults</span></span>|<span data-ttu-id="ca132-599">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-599">Boolean</span></span>|<span data-ttu-id="ca132-600">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-600">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="ca132-601">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-601">voiceDialingBlocked</span></span>|<span data-ttu-id="ca132-602">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-602">Boolean</span></span>|<span data-ttu-id="ca132-603">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ca132-603">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="ca132-604">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="ca132-604">wallpaperBlockModification</span></span>|<span data-ttu-id="ca132-605">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-605">Boolean</span></span>|<span data-ttu-id="ca132-606">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-606">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="ca132-607">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="ca132-607">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="ca132-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca132-608">Boolean</span></span>|<span data-ttu-id="ca132-609">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="ca132-609">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ca132-610">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="ca132-610">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="ca132-611">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-611">Boolean</span></span>|<span data-ttu-id="ca132-612">Indica se um aluno inscrito em um curso não gerenciado via sala de aula solicitará permissão do professor ao tentar sair do curso (iOS 11,3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-612">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="ca132-613">Propriedadeskeychainblockcloudsync</span><span class="sxs-lookup"><span data-stu-id="ca132-613">keychainBlockCloudSync</span></span>|<span data-ttu-id="ca132-614">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-614">Boolean</span></span>|<span data-ttu-id="ca132-615">Indica se a sincronização de chaves do iCloud está bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="ca132-615">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="ca132-616">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="ca132-616">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="ca132-617">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-617">Boolean</span></span>|<span data-ttu-id="ca132-618">Indica se as atualizações de PKI de over-the-Air serão bloqueadas ou não.</span><span class="sxs-lookup"><span data-stu-id="ca132-618">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="ca132-619">A definição dessa restrição como false não desabilita as verificações de CRL e OCSP (iOS 7,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-619">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="ca132-620">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="ca132-620">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="ca132-621">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-621">Boolean</span></span>|<span data-ttu-id="ca132-622">Indica se o controle do AD é limitado. (iOS 7,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-622">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="ca132-623">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="ca132-623">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="ca132-624">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-624">Boolean</span></span>|<span data-ttu-id="ca132-625">Indica se o backup do catálogo empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ca132-625">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="ca132-626">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="ca132-626">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="ca132-627">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-627">Boolean</span></span>|<span data-ttu-id="ca132-628">Indica se a sincronização de notas e destaques do catálogo empresarial será bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ca132-628">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="ca132-629">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-629">airPrintBlocked</span></span>|<span data-ttu-id="ca132-630">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-630">Boolean</span></span>|<span data-ttu-id="ca132-631">Indica se o arquivo de impressão está bloqueado ou não (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-631">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ca132-632">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="ca132-632">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="ca132-633">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-633">Boolean</span></span>|<span data-ttu-id="ca132-634">Indica se o armazenamento de chaves de nome de usuário e a senha para impressão de uma ou não é bloqueado (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-634">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ca132-635">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="ca132-635">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="ca132-636">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-636">Boolean</span></span>|<span data-ttu-id="ca132-637">Indica se os certificados confiáveis são necessários para a comunicação de impressão TLS (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-637">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ca132-638">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="ca132-638">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="ca132-639">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-639">Boolean</span></span>|<span data-ttu-id="ca132-640">Indica se a descoberta de impressoras de impressão do iBeacon está ou não bloqueada.</span><span class="sxs-lookup"><span data-stu-id="ca132-640">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="ca132-641">Isso impede os beacons Bluetooth de impressão de mensagens de phishing para tráfego de rede (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-641">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ca132-642">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="ca132-642">blockSystemAppRemoval</span></span>|<span data-ttu-id="ca132-643">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-643">Boolean</span></span>|<span data-ttu-id="ca132-644">Indica se a remoção de aplicativos do sistema do dispositivo é bloqueada em um dispositivo supervisionado (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-644">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ca132-645">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="ca132-645">vpnBlockCreation</span></span>|<span data-ttu-id="ca132-646">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-646">Boolean</span></span>|<span data-ttu-id="ca132-647">Indica se a criação de configurações de VPN está bloqueada (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-647">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ca132-648">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-648">appRemovalBlocked</span></span>|<span data-ttu-id="ca132-649">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-649">Boolean</span></span>|<span data-ttu-id="ca132-650">Indica se a remoção de aplicativos é permitida.</span><span class="sxs-lookup"><span data-stu-id="ca132-650">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="ca132-651">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="ca132-651">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="ca132-652">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-652">Boolean</span></span>|<span data-ttu-id="ca132-653">Indica se a conexão a acessórios USB enquanto o dispositivo está bloqueado é permitida (iOS 11.4.1 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-653">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="ca132-654">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="ca132-654">passwordBlockAutoFill</span></span>|<span data-ttu-id="ca132-655">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-655">Boolean</span></span>|<span data-ttu-id="ca132-656">Indica se o recurso de senha de preenchimento automático é permitido (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-656">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ca132-657">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="ca132-657">passwordBlockProximityRequests</span></span>|<span data-ttu-id="ca132-658">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-658">Boolean</span></span>|<span data-ttu-id="ca132-659">Indica se as senhas de solicitação devem ou não ser bloqueadas de dispositivos próximos (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-659">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ca132-660">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="ca132-660">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="ca132-661">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-661">Boolean</span></span>|<span data-ttu-id="ca132-662">Indica se as senhas de compartilhamento devem ou não ser bloqueadas com o recurso de senhas de soltura de estours iOS 12,0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="ca132-662">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ca132-663">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="ca132-663">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="ca132-664">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-664">Boolean</span></span>|<span data-ttu-id="ca132-665">Indica se o recurso "definir automaticamente" de data e hora está habilitado e não pode ser desativado pelo usuário (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-665">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ca132-666">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="ca132-666">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="ca132-667">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-667">Boolean</span></span>|<span data-ttu-id="ca132-668">Indica se os aplicativos gerenciados podem ou não gravar contatos para contas de contatos não gerenciados (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-668">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ca132-669">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="ca132-669">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="ca132-670">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca132-670">Boolean</span></span>|<span data-ttu-id="ca132-671">Indica se os aplicativos não gerenciados podem ler de contas de contatos gerenciados (iOS 12,0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="ca132-671">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="ca132-672">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca132-672">Response</span></span>
<span data-ttu-id="ca132-673">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca132-673">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca132-674">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca132-674">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca132-675">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca132-675">Request</span></span>
<span data-ttu-id="ca132-676">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca132-676">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 9105

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
  "contactsAllowUnmanagedToManagedRead": true
}
```

### <a name="response"></a><span data-ttu-id="ca132-677">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca132-677">Response</span></span>
<span data-ttu-id="ca132-p133">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca132-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9277

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
  "contactsAllowUnmanagedToManagedRead": true
}
```





