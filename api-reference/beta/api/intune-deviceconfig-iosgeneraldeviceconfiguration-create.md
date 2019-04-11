---
title: Criar iosGeneralDeviceConfiguration
description: Cria um novo objeto iosGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e97b15f484511d3bbf333014ed6804e603a0cf09
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776539"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="eb999-103">Criar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="eb999-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="eb999-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb999-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb999-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb999-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb999-106">Cria um novo objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb999-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb999-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb999-107">Prerequisites</span></span>
<span data-ttu-id="eb999-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb999-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb999-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb999-110">Permission type</span></span>|<span data-ttu-id="eb999-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb999-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb999-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb999-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb999-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb999-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb999-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb999-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb999-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb999-115">Not supported.</span></span>|
|<span data-ttu-id="eb999-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb999-116">Application</span></span>|<span data-ttu-id="eb999-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb999-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb999-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb999-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="eb999-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb999-119">Request headers</span></span>
|<span data-ttu-id="eb999-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb999-120">Header</span></span>|<span data-ttu-id="eb999-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eb999-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb999-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb999-122">Authorization</span></span>|<span data-ttu-id="eb999-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb999-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb999-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb999-124">Accept</span></span>|<span data-ttu-id="eb999-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb999-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb999-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb999-126">Request body</span></span>
<span data-ttu-id="eb999-127">No corpo da solicitação, forneça uma representação JSON do objeto iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="eb999-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="eb999-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="eb999-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="eb999-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb999-129">Property</span></span>|<span data-ttu-id="eb999-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb999-130">Type</span></span>|<span data-ttu-id="eb999-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb999-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb999-132">id</span><span class="sxs-lookup"><span data-stu-id="eb999-132">id</span></span>|<span data-ttu-id="eb999-133">String</span><span class="sxs-lookup"><span data-stu-id="eb999-133">String</span></span>|<span data-ttu-id="eb999-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="eb999-134">Key of the entity.</span></span> <span data-ttu-id="eb999-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb999-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb999-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb999-136">lastModifiedDateTime</span></span>|<span data-ttu-id="eb999-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb999-137">DateTimeOffset</span></span>|<span data-ttu-id="eb999-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="eb999-138">DateTime the object was last modified.</span></span> <span data-ttu-id="eb999-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb999-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb999-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eb999-140">roleScopeTagIds</span></span>|<span data-ttu-id="eb999-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="eb999-141">String collection</span></span>|<span data-ttu-id="eb999-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="eb999-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="eb999-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb999-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb999-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="eb999-144">supportsScopeTags</span></span>|<span data-ttu-id="eb999-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-145">Boolean</span></span>|<span data-ttu-id="eb999-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="eb999-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="eb999-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="eb999-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="eb999-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="eb999-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="eb999-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb999-149">This property is read-only.</span></span> <span data-ttu-id="eb999-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb999-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb999-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb999-151">createdDateTime</span></span>|<span data-ttu-id="eb999-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb999-152">DateTimeOffset</span></span>|<span data-ttu-id="eb999-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="eb999-153">DateTime the object was created.</span></span> <span data-ttu-id="eb999-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb999-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb999-155">description</span><span class="sxs-lookup"><span data-stu-id="eb999-155">description</span></span>|<span data-ttu-id="eb999-156">String</span><span class="sxs-lookup"><span data-stu-id="eb999-156">String</span></span>|<span data-ttu-id="eb999-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eb999-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eb999-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb999-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb999-159">displayName</span><span class="sxs-lookup"><span data-stu-id="eb999-159">displayName</span></span>|<span data-ttu-id="eb999-160">String</span><span class="sxs-lookup"><span data-stu-id="eb999-160">String</span></span>|<span data-ttu-id="eb999-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eb999-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eb999-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb999-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb999-163">versão</span><span class="sxs-lookup"><span data-stu-id="eb999-163">version</span></span>|<span data-ttu-id="eb999-164">Int32</span><span class="sxs-lookup"><span data-stu-id="eb999-164">Int32</span></span>|<span data-ttu-id="eb999-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eb999-165">Version of the device configuration.</span></span> <span data-ttu-id="eb999-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb999-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb999-167">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="eb999-167">accountBlockModification</span></span>|<span data-ttu-id="eb999-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-168">Boolean</span></span>|<span data-ttu-id="eb999-169">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-169">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-170">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="eb999-170">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="eb999-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-171">Boolean</span></span>|<span data-ttu-id="eb999-172">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-172">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="eb999-173">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-173">airDropBlocked</span></span>|<span data-ttu-id="eb999-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-174">Boolean</span></span>|<span data-ttu-id="eb999-175">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-175">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-176">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="eb999-176">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="eb999-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-177">Boolean</span></span>|<span data-ttu-id="eb999-178">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-178">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="eb999-179">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="eb999-179">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="eb999-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-180">Boolean</span></span>|<span data-ttu-id="eb999-181">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="eb999-181">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="eb999-182">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="eb999-182">appleWatchBlockPairing</span></span>|<span data-ttu-id="eb999-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-183">Boolean</span></span>|<span data-ttu-id="eb999-184">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-184">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="eb999-185">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="eb999-185">appleWatchForceWristDetection</span></span>|<span data-ttu-id="eb999-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-186">Boolean</span></span>|<span data-ttu-id="eb999-187">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-187">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="eb999-188">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-188">appleNewsBlocked</span></span>|<span data-ttu-id="eb999-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-189">Boolean</span></span>|<span data-ttu-id="eb999-190">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-190">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="eb999-191">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="eb999-191">appsSingleAppModeList</span></span>|<span data-ttu-id="eb999-192">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="eb999-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="eb999-193">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="eb999-193">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="eb999-194">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-194">Supervised only.</span></span> <span data-ttu-id="eb999-195">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="eb999-195">iOS 7.0 and later.</span></span> <span data-ttu-id="eb999-196">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="eb999-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="eb999-197">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="eb999-197">appsVisibilityList</span></span>|<span data-ttu-id="eb999-198">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="eb999-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="eb999-199">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-199">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="eb999-200">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="eb999-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="eb999-201">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="eb999-201">appsVisibilityListType</span></span>|[<span data-ttu-id="eb999-202">appListType</span><span class="sxs-lookup"><span data-stu-id="eb999-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="eb999-203">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="eb999-203">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="eb999-204">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="eb999-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="eb999-205">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="eb999-205">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="eb999-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-206">Boolean</span></span>|<span data-ttu-id="eb999-207">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-207">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="eb999-208">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-208">appStoreBlocked</span></span>|<span data-ttu-id="eb999-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-209">Boolean</span></span>|<span data-ttu-id="eb999-210">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="eb999-210">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="eb999-211">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="eb999-211">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="eb999-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-212">Boolean</span></span>|<span data-ttu-id="eb999-213">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eb999-213">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="eb999-214">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="eb999-214">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="eb999-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-215">Boolean</span></span>|<span data-ttu-id="eb999-216">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="eb999-216">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="eb999-217">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-217">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="eb999-218">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="eb999-218">appStoreRequirePassword</span></span>|<span data-ttu-id="eb999-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb999-219">Boolean</span></span>|<span data-ttu-id="eb999-220">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="eb999-220">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="eb999-221">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="eb999-221">autoFillForceAuthentication</span></span>|<span data-ttu-id="eb999-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-222">Boolean</span></span>|<span data-ttu-id="eb999-223">Indica se a autenticação do usuário deve ou não ser forçada antes de preencher automaticamente as informações de cartão de crédito e o Safari e outros aplicativos em dispositivos supervisionados.</span><span class="sxs-lookup"><span data-stu-id="eb999-223">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="eb999-224">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="eb999-224">bluetoothBlockModification</span></span>|<span data-ttu-id="eb999-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-225">Boolean</span></span>|<span data-ttu-id="eb999-226">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-226">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="eb999-227">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-227">cameraBlocked</span></span>|<span data-ttu-id="eb999-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-228">Boolean</span></span>|<span data-ttu-id="eb999-229">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eb999-229">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="eb999-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="eb999-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="eb999-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-231">Boolean</span></span>|<span data-ttu-id="eb999-232">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="eb999-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="eb999-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="eb999-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="eb999-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-234">Boolean</span></span>|<span data-ttu-id="eb999-235">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="eb999-235">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="eb999-236">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="eb999-236">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="eb999-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-237">Boolean</span></span>|<span data-ttu-id="eb999-238">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-238">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-239">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="eb999-239">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="eb999-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-240">Boolean</span></span>|<span data-ttu-id="eb999-241">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="eb999-241">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="eb999-242">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="eb999-242">cellularBlockPlanModification</span></span>|<span data-ttu-id="eb999-243">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-243">Boolean</span></span>|<span data-ttu-id="eb999-244">Indica se os usuários poderão ou não alterar as configurações do plano de celular em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-244">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="eb999-245">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="eb999-245">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="eb999-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-246">Boolean</span></span>|<span data-ttu-id="eb999-247">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="eb999-247">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="eb999-248">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="eb999-248">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="eb999-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-249">Boolean</span></span>|<span data-ttu-id="eb999-250">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="eb999-250">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="eb999-251">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="eb999-251">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="eb999-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-252">Boolean</span></span>|<span data-ttu-id="eb999-253">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-253">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="eb999-254">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="eb999-254">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="eb999-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-255">Boolean</span></span>|<span data-ttu-id="eb999-256">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-256">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-257">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="eb999-257">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="eb999-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-258">Boolean</span></span>|<span data-ttu-id="eb999-259">Indica se a permissão será ou não automaticamente atribuído às solicitações do professor, sem avisar o aluno, quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-259">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-260">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="eb999-260">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="eb999-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-261">Boolean</span></span>|<span data-ttu-id="eb999-262">Indica se o professor deve ou não bloquear aplicativos ou o dispositivo sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="eb999-262">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="eb999-263">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-263">Supervised only.</span></span>|
|<span data-ttu-id="eb999-264">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="eb999-264">compliantAppsList</span></span>|<span data-ttu-id="eb999-265">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="eb999-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="eb999-266">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="eb999-266">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="eb999-267">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="eb999-267">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="eb999-268">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="eb999-268">compliantAppListType</span></span>|[<span data-ttu-id="eb999-269">appListType</span><span class="sxs-lookup"><span data-stu-id="eb999-269">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="eb999-270">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="eb999-270">List that is in the AppComplianceList.</span></span> <span data-ttu-id="eb999-271">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="eb999-271">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="eb999-272">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="eb999-272">configurationProfileBlockChanges</span></span>|<span data-ttu-id="eb999-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-273">Boolean</span></span>|<span data-ttu-id="eb999-274">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-274">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-275">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-275">definitionLookupBlocked</span></span>|<span data-ttu-id="eb999-276">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-276">Boolean</span></span>|<span data-ttu-id="eb999-277">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-277">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="eb999-278">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="eb999-278">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="eb999-279">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-279">Boolean</span></span>|<span data-ttu-id="eb999-280">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-280">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-281">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="eb999-281">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="eb999-282">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-282">Boolean</span></span>|<span data-ttu-id="eb999-283">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-283">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-284">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="eb999-284">deviceBlockNameModification</span></span>|<span data-ttu-id="eb999-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-285">Boolean</span></span>|<span data-ttu-id="eb999-286">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-286">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="eb999-287">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="eb999-287">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="eb999-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-288">Boolean</span></span>|<span data-ttu-id="eb999-289">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="eb999-289">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="eb999-290">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="eb999-290">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="eb999-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-291">Boolean</span></span>|<span data-ttu-id="eb999-292">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-292">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="eb999-293">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="eb999-293">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="eb999-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-294">Boolean</span></span>|<span data-ttu-id="eb999-295">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="eb999-295">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="eb999-296">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="eb999-296">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="eb999-297">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-297">Boolean</span></span>|<span data-ttu-id="eb999-298">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="eb999-298">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="eb999-299">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="eb999-299">emailInDomainSuffixes</span></span>|<span data-ttu-id="eb999-300">String collection</span><span class="sxs-lookup"><span data-stu-id="eb999-300">String collection</span></span>|<span data-ttu-id="eb999-301">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="eb999-301">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="eb999-302">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="eb999-302">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="eb999-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-303">Boolean</span></span>|<span data-ttu-id="eb999-304">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="eb999-304">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="eb999-305">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="eb999-305">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="eb999-306">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-306">Boolean</span></span>|<span data-ttu-id="eb999-307">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="eb999-307">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="eb999-308">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="eb999-308">esimBlockModification</span></span>|<span data-ttu-id="eb999-309">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-309">Boolean</span></span>|<span data-ttu-id="eb999-310">Indica se a adição ou a remoção de planos da rede celular deve ou não ser permitida no eSIM de um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-310">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="eb999-311">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-311">faceTimeBlocked</span></span>|<span data-ttu-id="eb999-312">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-312">Boolean</span></span>|<span data-ttu-id="eb999-313">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="eb999-313">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="eb999-314">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-314">findMyFriendsBlocked</span></span>|<span data-ttu-id="eb999-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-315">Boolean</span></span>|<span data-ttu-id="eb999-316">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-316">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-317">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="eb999-317">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="eb999-318">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-318">Boolean</span></span>|<span data-ttu-id="eb999-319">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="eb999-319">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="eb999-320">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="eb999-320">gamingBlockMultiplayer</span></span>|<span data-ttu-id="eb999-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb999-321">Boolean</span></span>|<span data-ttu-id="eb999-322">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="eb999-322">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="eb999-323">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-323">gameCenterBlocked</span></span>|<span data-ttu-id="eb999-324">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-324">Boolean</span></span>|<span data-ttu-id="eb999-325">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-325">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-326">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-326">hostPairingBlocked</span></span>|<span data-ttu-id="eb999-327">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-327">Boolean</span></span>|<span data-ttu-id="eb999-328">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-328">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-329">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-329">iBooksStoreBlocked</span></span>|<span data-ttu-id="eb999-330">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-330">Boolean</span></span>|<span data-ttu-id="eb999-331">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-331">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-332">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="eb999-332">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="eb999-333">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-333">Boolean</span></span>|<span data-ttu-id="eb999-334">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="eb999-334">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="eb999-335">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="eb999-335">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="eb999-336">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-336">Boolean</span></span>|<span data-ttu-id="eb999-337">Indica se o usuário será ou não impedido de continuar um trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="eb999-337">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="eb999-338">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="eb999-338">iCloudBlockBackup</span></span>|<span data-ttu-id="eb999-339">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-339">Boolean</span></span>|<span data-ttu-id="eb999-340">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="eb999-340">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="eb999-341">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="eb999-341">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="eb999-342">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-342">Boolean</span></span>|<span data-ttu-id="eb999-343">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="eb999-343">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="eb999-344">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="eb999-344">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="eb999-345">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-345">Boolean</span></span>|<span data-ttu-id="eb999-346">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="eb999-346">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="eb999-347">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="eb999-347">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="eb999-348">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-348">Boolean</span></span>|<span data-ttu-id="eb999-349">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="eb999-349">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="eb999-350">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="eb999-350">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="eb999-351">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-351">Boolean</span></span>|<span data-ttu-id="eb999-352">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="eb999-352">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="eb999-353">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="eb999-353">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="eb999-354">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-354">Boolean</span></span>|<span data-ttu-id="eb999-355">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="eb999-355">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="eb999-356">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="eb999-356">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="eb999-357">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-357">Boolean</span></span>|<span data-ttu-id="eb999-358">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="eb999-358">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="eb999-359">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="eb999-359">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="eb999-360">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-360">Boolean</span></span>|<span data-ttu-id="eb999-361">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="eb999-361">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="eb999-362">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="eb999-362">iTunesBlockMusicService</span></span>|<span data-ttu-id="eb999-363">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-363">Boolean</span></span>|<span data-ttu-id="eb999-364">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-364">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="eb999-365">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="eb999-365">iTunesBlockRadio</span></span>|<span data-ttu-id="eb999-366">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-366">Boolean</span></span>|<span data-ttu-id="eb999-367">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-367">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="eb999-368">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="eb999-368">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="eb999-369">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-369">Boolean</span></span>|<span data-ttu-id="eb999-370">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-370">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="eb999-371">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="eb999-371">keyboardBlockDictation</span></span>|<span data-ttu-id="eb999-372">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-372">Boolean</span></span>|<span data-ttu-id="eb999-373">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-373">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-374">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="eb999-374">keyboardBlockPredictive</span></span>|<span data-ttu-id="eb999-375">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-375">Boolean</span></span>|<span data-ttu-id="eb999-376">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-376">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="eb999-377">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="eb999-377">keyboardBlockShortcuts</span></span>|<span data-ttu-id="eb999-378">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-378">Boolean</span></span>|<span data-ttu-id="eb999-379">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-379">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="eb999-380">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="eb999-380">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="eb999-381">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-381">Boolean</span></span>|<span data-ttu-id="eb999-382">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-382">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="eb999-383">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="eb999-383">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="eb999-384">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-384">Boolean</span></span>|<span data-ttu-id="eb999-385">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-385">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-386">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="eb999-386">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="eb999-387">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-387">Boolean</span></span>|<span data-ttu-id="eb999-388">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-388">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-389">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="eb999-389">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="eb999-390">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-390">Boolean</span></span>|<span data-ttu-id="eb999-391">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-391">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-392">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="eb999-392">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="eb999-393">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-393">Boolean</span></span>|<span data-ttu-id="eb999-394">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-394">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-395">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="eb999-395">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="eb999-396">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-396">Boolean</span></span>|<span data-ttu-id="eb999-397">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-397">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-398">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="eb999-398">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="eb999-399">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-399">Boolean</span></span>|<span data-ttu-id="eb999-400">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-400">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-401">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="eb999-401">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="eb999-402">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-402">Boolean</span></span>|<span data-ttu-id="eb999-403">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-403">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-404">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="eb999-404">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="eb999-405">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-405">Boolean</span></span>|<span data-ttu-id="eb999-406">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-406">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-407">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="eb999-407">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="eb999-408">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-408">Boolean</span></span>|<span data-ttu-id="eb999-409">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-409">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-410">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="eb999-410">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="eb999-411">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-411">Boolean</span></span>|<span data-ttu-id="eb999-412">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-412">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-413">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="eb999-413">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="eb999-414">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-414">Boolean</span></span>|<span data-ttu-id="eb999-415">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-415">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="eb999-416">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="eb999-416">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="eb999-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb999-417">Boolean</span></span>|<span data-ttu-id="eb999-418">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-418">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-419">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="eb999-419">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="eb999-420">String</span><span class="sxs-lookup"><span data-stu-id="eb999-420">String</span></span>|<span data-ttu-id="eb999-421">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-421">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="eb999-422">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="eb999-422">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="eb999-423">Propriedadekioskmodebuiltinappid</span><span class="sxs-lookup"><span data-stu-id="eb999-423">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="eb999-424">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb999-424">String</span></span>|<span data-ttu-id="eb999-425">ID para aplicativos internos a serem usados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-425">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="eb999-426">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidos.</span><span class="sxs-lookup"><span data-stu-id="eb999-426">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="eb999-427">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="eb999-427">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="eb999-428">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-428">Boolean</span></span>|<span data-ttu-id="eb999-429">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-429">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-430">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="eb999-430">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="eb999-431">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-431">Boolean</span></span>|<span data-ttu-id="eb999-432">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-432">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-433">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="eb999-433">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="eb999-434">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-434">Boolean</span></span>|<span data-ttu-id="eb999-435">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-435">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-436">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="eb999-436">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="eb999-437">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-437">Boolean</span></span>|<span data-ttu-id="eb999-438">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-438">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-439">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="eb999-439">kioskModeRequireZoom</span></span>|<span data-ttu-id="eb999-440">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-440">Boolean</span></span>|<span data-ttu-id="eb999-441">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-441">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="eb999-442">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="eb999-442">kioskModeManagedAppId</span></span>|<span data-ttu-id="eb999-443">String</span><span class="sxs-lookup"><span data-stu-id="eb999-443">String</span></span>|<span data-ttu-id="eb999-444">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="eb999-444">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="eb999-445">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="eb999-445">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="eb999-446">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="eb999-446">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="eb999-447">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-447">Boolean</span></span>|<span data-ttu-id="eb999-448">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="eb999-448">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="eb999-449">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="eb999-449">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="eb999-450">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-450">Boolean</span></span>|<span data-ttu-id="eb999-451">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="eb999-451">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="eb999-452">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="eb999-452">lockScreenBlockPassbook</span></span>|<span data-ttu-id="eb999-453">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-453">Boolean</span></span>|<span data-ttu-id="eb999-454">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="eb999-454">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="eb999-455">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="eb999-455">lockScreenBlockTodayView</span></span>|<span data-ttu-id="eb999-456">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-456">Boolean</span></span>|<span data-ttu-id="eb999-457">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="eb999-457">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="eb999-458">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="eb999-458">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="eb999-459">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="eb999-459">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="eb999-460">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="eb999-460">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="eb999-461">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="eb999-461">mediaContentRatingCanada</span></span>|[<span data-ttu-id="eb999-462">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="eb999-462">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="eb999-463">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="eb999-463">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="eb999-464">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="eb999-464">mediaContentRatingFrance</span></span>|[<span data-ttu-id="eb999-465">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="eb999-465">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="eb999-466">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="eb999-466">Media content rating settings for France</span></span>|
|<span data-ttu-id="eb999-467">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="eb999-467">mediaContentRatingGermany</span></span>|[<span data-ttu-id="eb999-468">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="eb999-468">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="eb999-469">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="eb999-469">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="eb999-470">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="eb999-470">mediaContentRatingIreland</span></span>|[<span data-ttu-id="eb999-471">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="eb999-471">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="eb999-472">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="eb999-472">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="eb999-473">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="eb999-473">mediaContentRatingJapan</span></span>|[<span data-ttu-id="eb999-474">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="eb999-474">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="eb999-475">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="eb999-475">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="eb999-476">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="eb999-476">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="eb999-477">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="eb999-477">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="eb999-478">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="eb999-478">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="eb999-479">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="eb999-479">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="eb999-480">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="eb999-480">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="eb999-481">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="eb999-481">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="eb999-482">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="eb999-482">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="eb999-483">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="eb999-483">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="eb999-484">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="eb999-484">Media content rating settings for United States</span></span>|
|<span data-ttu-id="eb999-485">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="eb999-485">networkUsageRules</span></span>|<span data-ttu-id="eb999-486">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="eb999-486">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="eb999-487">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="eb999-487">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="eb999-488">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="eb999-488">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="eb999-489">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="eb999-489">mediaContentRatingApps</span></span>|[<span data-ttu-id="eb999-490">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="eb999-490">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="eb999-491">Configurações de classificação de conteúdo de mídia para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="eb999-491">Media content rating settings for Apps.</span></span> <span data-ttu-id="eb999-492">Os valores possíveis são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="eb999-492">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="eb999-493">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-493">messagesBlocked</span></span>|<span data-ttu-id="eb999-494">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-494">Boolean</span></span>|<span data-ttu-id="eb999-495">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-495">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="eb999-496">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="eb999-496">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="eb999-497">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-497">Boolean</span></span>|<span data-ttu-id="eb999-498">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-498">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="eb999-499">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="eb999-499">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="eb999-500">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-500">Boolean</span></span>|<span data-ttu-id="eb999-501">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="eb999-501">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="eb999-502">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="eb999-502">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="eb999-503">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-503">Boolean</span></span>|<span data-ttu-id="eb999-504">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-504">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="eb999-505">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="eb999-505">passcodeBlockModification</span></span>|<span data-ttu-id="eb999-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb999-506">Boolean</span></span>|<span data-ttu-id="eb999-507">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-507">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="eb999-508">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="eb999-508">passcodeBlockSimple</span></span>|<span data-ttu-id="eb999-509">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-509">Boolean</span></span>|<span data-ttu-id="eb999-510">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="eb999-510">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="eb999-511">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="eb999-511">passcodeExpirationDays</span></span>|<span data-ttu-id="eb999-512">Int32</span><span class="sxs-lookup"><span data-stu-id="eb999-512">Int32</span></span>|<span data-ttu-id="eb999-513">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="eb999-513">Number of days before the passcode expires.</span></span> <span data-ttu-id="eb999-514">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="eb999-514">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="eb999-515">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="eb999-515">passcodeMinimumLength</span></span>|<span data-ttu-id="eb999-516">Int32</span><span class="sxs-lookup"><span data-stu-id="eb999-516">Int32</span></span>|<span data-ttu-id="eb999-517">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="eb999-517">Minimum length of passcode.</span></span> <span data-ttu-id="eb999-518">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="eb999-518">Valid values 4 to 14</span></span>|
|<span data-ttu-id="eb999-519">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="eb999-519">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="eb999-520">Int32</span><span class="sxs-lookup"><span data-stu-id="eb999-520">Int32</span></span>|<span data-ttu-id="eb999-521">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="eb999-521">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="eb999-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="eb999-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="eb999-523">Int32</span><span class="sxs-lookup"><span data-stu-id="eb999-523">Int32</span></span>|<span data-ttu-id="eb999-524">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="eb999-524">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="eb999-525">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="eb999-525">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="eb999-526">Int32</span><span class="sxs-lookup"><span data-stu-id="eb999-526">Int32</span></span>|<span data-ttu-id="eb999-527">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="eb999-527">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="eb999-528">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="eb999-528">Valid values 0 to 4</span></span>|
|<span data-ttu-id="eb999-529">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="eb999-529">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="eb999-530">Int32</span><span class="sxs-lookup"><span data-stu-id="eb999-530">Int32</span></span>|<span data-ttu-id="eb999-531">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="eb999-531">Number of previous passcodes to block.</span></span> <span data-ttu-id="eb999-532">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="eb999-532">Valid values 1 to 24</span></span>|
|<span data-ttu-id="eb999-533">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="eb999-533">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="eb999-534">Int32</span><span class="sxs-lookup"><span data-stu-id="eb999-534">Int32</span></span>|<span data-ttu-id="eb999-535">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eb999-535">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="eb999-536">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="eb999-536">Valid values 4 to 11</span></span>|
|<span data-ttu-id="eb999-537">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="eb999-537">passcodeRequiredType</span></span>|[<span data-ttu-id="eb999-538">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="eb999-538">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="eb999-539">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="eb999-539">Type of passcode that is required.</span></span> <span data-ttu-id="eb999-540">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="eb999-540">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="eb999-541">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="eb999-541">passcodeRequired</span></span>|<span data-ttu-id="eb999-542">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-542">Boolean</span></span>|<span data-ttu-id="eb999-543">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="eb999-543">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="eb999-544">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-544">podcastsBlocked</span></span>|<span data-ttu-id="eb999-545">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-545">Boolean</span></span>|<span data-ttu-id="eb999-546">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-546">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="eb999-547">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="eb999-547">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="eb999-548">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-548">Boolean</span></span>|<span data-ttu-id="eb999-549">Indica se o prompt deve ou não ser habilitado para configurar dispositivos próximos com um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-549">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="eb999-550">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="eb999-550">safariBlockAutofill</span></span>|<span data-ttu-id="eb999-551">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-551">Boolean</span></span>|<span data-ttu-id="eb999-552">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="eb999-552">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="eb999-553">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="eb999-553">safariBlockJavaScript</span></span>|<span data-ttu-id="eb999-554">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-554">Boolean</span></span>|<span data-ttu-id="eb999-555">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="eb999-555">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="eb999-556">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="eb999-556">safariBlockPopups</span></span>|<span data-ttu-id="eb999-557">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-557">Boolean</span></span>|<span data-ttu-id="eb999-558">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="eb999-558">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="eb999-559">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-559">safariBlocked</span></span>|<span data-ttu-id="eb999-560">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-560">Boolean</span></span>|<span data-ttu-id="eb999-561">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="eb999-561">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="eb999-562">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="eb999-562">safariCookieSettings</span></span>|[<span data-ttu-id="eb999-563">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="eb999-563">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="eb999-564">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="eb999-564">Cookie settings for Safari.</span></span> <span data-ttu-id="eb999-565">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="eb999-565">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="eb999-566">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="eb999-566">safariManagedDomains</span></span>|<span data-ttu-id="eb999-567">Coleção String</span><span class="sxs-lookup"><span data-stu-id="eb999-567">String collection</span></span>|<span data-ttu-id="eb999-568">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="eb999-568">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="eb999-569">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="eb999-569">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="eb999-570">String collection</span><span class="sxs-lookup"><span data-stu-id="eb999-570">String collection</span></span>|<span data-ttu-id="eb999-571">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="eb999-571">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="eb999-572">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-572">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="eb999-573">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="eb999-573">safariRequireFraudWarning</span></span>|<span data-ttu-id="eb999-574">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-574">Boolean</span></span>|<span data-ttu-id="eb999-575">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="eb999-575">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="eb999-576">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-576">screenCaptureBlocked</span></span>|<span data-ttu-id="eb999-577">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-577">Boolean</span></span>|<span data-ttu-id="eb999-578">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="eb999-578">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="eb999-579">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-579">siriBlocked</span></span>|<span data-ttu-id="eb999-580">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-580">Boolean</span></span>|<span data-ttu-id="eb999-581">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="eb999-581">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="eb999-582">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="eb999-582">siriBlockedWhenLocked</span></span>|<span data-ttu-id="eb999-583">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-583">Boolean</span></span>|<span data-ttu-id="eb999-584">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="eb999-584">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="eb999-585">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="eb999-585">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="eb999-586">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-586">Boolean</span></span>|<span data-ttu-id="eb999-587">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-587">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="eb999-588">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="eb999-588">siriRequireProfanityFilter</span></span>|<span data-ttu-id="eb999-589">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-589">Boolean</span></span>|<span data-ttu-id="eb999-590">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-590">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="eb999-591">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="eb999-591">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="eb999-592">Int32</span><span class="sxs-lookup"><span data-stu-id="eb999-592">Int32</span></span>|<span data-ttu-id="eb999-593">Define o número de dias que uma atualização de software será delyed para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-593">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="eb999-594">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="eb999-594">Valid values 0 to 90</span></span>|
|<span data-ttu-id="eb999-595">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="eb999-595">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="eb999-596">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-596">Boolean</span></span>|<span data-ttu-id="eb999-597">Indica se o usuário deve ou não atrasar a visibilidade de atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-597">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-598">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="eb999-598">spotlightBlockInternetResults</span></span>|<span data-ttu-id="eb999-599">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-599">Boolean</span></span>|<span data-ttu-id="eb999-600">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-600">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="eb999-601">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-601">voiceDialingBlocked</span></span>|<span data-ttu-id="eb999-602">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-602">Boolean</span></span>|<span data-ttu-id="eb999-603">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="eb999-603">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="eb999-604">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="eb999-604">wallpaperBlockModification</span></span>|<span data-ttu-id="eb999-605">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-605">Boolean</span></span>|<span data-ttu-id="eb999-606">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-606">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="eb999-607">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="eb999-607">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="eb999-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb999-608">Boolean</span></span>|<span data-ttu-id="eb999-609">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="eb999-609">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="eb999-610">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="eb999-610">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="eb999-611">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-611">Boolean</span></span>|<span data-ttu-id="eb999-612">Indica se um aluno inscrito em um curso não gerenciado via sala de aula solicitará permissão do professor ao tentar sair do curso (iOS 11,3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-612">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="eb999-613">Propriedadeskeychainblockcloudsync</span><span class="sxs-lookup"><span data-stu-id="eb999-613">keychainBlockCloudSync</span></span>|<span data-ttu-id="eb999-614">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-614">Boolean</span></span>|<span data-ttu-id="eb999-615">Indica se a sincronização de chaves do iCloud está bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="eb999-615">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="eb999-616">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="eb999-616">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="eb999-617">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-617">Boolean</span></span>|<span data-ttu-id="eb999-618">Indica se as atualizações de PKI de over-the-Air serão bloqueadas ou não.</span><span class="sxs-lookup"><span data-stu-id="eb999-618">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="eb999-619">A definição dessa restrição como false não desabilita as verificações de CRL e OCSP (iOS 7,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-619">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="eb999-620">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="eb999-620">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="eb999-621">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-621">Boolean</span></span>|<span data-ttu-id="eb999-622">Indica se o controle do AD é limitado. (iOS 7,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-622">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="eb999-623">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="eb999-623">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="eb999-624">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-624">Boolean</span></span>|<span data-ttu-id="eb999-625">Indica se o backup do catálogo empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="eb999-625">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="eb999-626">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="eb999-626">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="eb999-627">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-627">Boolean</span></span>|<span data-ttu-id="eb999-628">Indica se a sincronização de notas e destaques do catálogo empresarial será bloqueada.</span><span class="sxs-lookup"><span data-stu-id="eb999-628">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="eb999-629">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-629">airPrintBlocked</span></span>|<span data-ttu-id="eb999-630">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-630">Boolean</span></span>|<span data-ttu-id="eb999-631">Indica se o arquivo de impressão está bloqueado ou não (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-631">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="eb999-632">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="eb999-632">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="eb999-633">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-633">Boolean</span></span>|<span data-ttu-id="eb999-634">Indica se o armazenamento de chaves de nome de usuário e a senha para impressão de uma ou não é bloqueado (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-634">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="eb999-635">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="eb999-635">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="eb999-636">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-636">Boolean</span></span>|<span data-ttu-id="eb999-637">Indica se os certificados confiáveis são necessários para a comunicação de impressão TLS (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-637">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="eb999-638">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="eb999-638">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="eb999-639">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-639">Boolean</span></span>|<span data-ttu-id="eb999-640">Indica se a descoberta de impressoras de impressão do iBeacon está ou não bloqueada.</span><span class="sxs-lookup"><span data-stu-id="eb999-640">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="eb999-641">Isso impede os beacons Bluetooth de impressão de mensagens de phishing para tráfego de rede (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-641">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="eb999-642">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="eb999-642">blockSystemAppRemoval</span></span>|<span data-ttu-id="eb999-643">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-643">Boolean</span></span>|<span data-ttu-id="eb999-644">Indica se a remoção de aplicativos do sistema do dispositivo é bloqueada em um dispositivo supervisionado (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-644">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="eb999-645">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="eb999-645">vpnBlockCreation</span></span>|<span data-ttu-id="eb999-646">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-646">Boolean</span></span>|<span data-ttu-id="eb999-647">Indica se a criação de configurações de VPN está bloqueada (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-647">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="eb999-648">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-648">appRemovalBlocked</span></span>|<span data-ttu-id="eb999-649">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-649">Boolean</span></span>|<span data-ttu-id="eb999-650">Indica se a remoção de aplicativos é permitida.</span><span class="sxs-lookup"><span data-stu-id="eb999-650">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="eb999-651">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="eb999-651">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="eb999-652">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-652">Boolean</span></span>|<span data-ttu-id="eb999-653">Indica se a conexão a acessórios USB enquanto o dispositivo está bloqueado é permitida (iOS 11.4.1 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-653">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="eb999-654">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="eb999-654">passwordBlockAutoFill</span></span>|<span data-ttu-id="eb999-655">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-655">Boolean</span></span>|<span data-ttu-id="eb999-656">Indica se o recurso de senha de preenchimento automático é permitido (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-656">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="eb999-657">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="eb999-657">passwordBlockProximityRequests</span></span>|<span data-ttu-id="eb999-658">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-658">Boolean</span></span>|<span data-ttu-id="eb999-659">Indica se as senhas de solicitação devem ou não ser bloqueadas de dispositivos próximos (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-659">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="eb999-660">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="eb999-660">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="eb999-661">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-661">Boolean</span></span>|<span data-ttu-id="eb999-662">Indica se as senhas de compartilhamento devem ou não ser bloqueadas com o recurso de senhas de soltura de estours iOS 12,0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="eb999-662">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="eb999-663">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="eb999-663">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="eb999-664">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-664">Boolean</span></span>|<span data-ttu-id="eb999-665">Indica se o recurso "definir automaticamente" de data e hora está habilitado e não pode ser desativado pelo usuário (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-665">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="eb999-666">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="eb999-666">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="eb999-667">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-667">Boolean</span></span>|<span data-ttu-id="eb999-668">Indica se os aplicativos gerenciados podem ou não gravar contatos para contas de contatos não gerenciados (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-668">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="eb999-669">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="eb999-669">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="eb999-670">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb999-670">Boolean</span></span>|<span data-ttu-id="eb999-671">Indica se os aplicativos não gerenciados podem ler de contas de contatos gerenciados (iOS 12,0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="eb999-671">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="eb999-672">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb999-672">Response</span></span>
<span data-ttu-id="eb999-673">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb999-673">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb999-674">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb999-674">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb999-675">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb999-675">Request</span></span>
<span data-ttu-id="eb999-676">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb999-676">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="eb999-677">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb999-677">Response</span></span>
<span data-ttu-id="eb999-p133">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb999-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





