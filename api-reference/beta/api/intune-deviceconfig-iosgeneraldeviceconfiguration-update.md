---
title: Atualizar iosGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto iosGeneralDeviceConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8b6a6800722645a272b538bef94de7b0dc1a08b7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42750492"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="59277-103">Atualizar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="59277-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="59277-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="59277-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59277-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="59277-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59277-106">Atualizar as propriedades de um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="59277-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="59277-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="59277-107">Prerequisites</span></span>
<span data-ttu-id="59277-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59277-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59277-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59277-110">Permission type</span></span>|<span data-ttu-id="59277-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="59277-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59277-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59277-112">Delegated (work or school account)</span></span>|<span data-ttu-id="59277-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59277-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="59277-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59277-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59277-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59277-115">Not supported.</span></span>|
|<span data-ttu-id="59277-116">Application</span><span class="sxs-lookup"><span data-stu-id="59277-116">Application</span></span>|<span data-ttu-id="59277-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59277-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="59277-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59277-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="59277-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59277-119">Request headers</span></span>
|<span data-ttu-id="59277-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="59277-120">Header</span></span>|<span data-ttu-id="59277-121">Valor</span><span class="sxs-lookup"><span data-stu-id="59277-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="59277-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="59277-122">Authorization</span></span>|<span data-ttu-id="59277-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59277-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="59277-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="59277-124">Accept</span></span>|<span data-ttu-id="59277-125">application/json</span><span class="sxs-lookup"><span data-stu-id="59277-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="59277-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59277-126">Request body</span></span>
<span data-ttu-id="59277-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="59277-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="59277-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="59277-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="59277-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59277-129">Property</span></span>|<span data-ttu-id="59277-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="59277-130">Type</span></span>|<span data-ttu-id="59277-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="59277-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59277-132">id</span><span class="sxs-lookup"><span data-stu-id="59277-132">id</span></span>|<span data-ttu-id="59277-133">String</span><span class="sxs-lookup"><span data-stu-id="59277-133">String</span></span>|<span data-ttu-id="59277-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="59277-134">Key of the entity.</span></span> <span data-ttu-id="59277-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59277-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59277-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="59277-136">lastModifiedDateTime</span></span>|<span data-ttu-id="59277-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59277-137">DateTimeOffset</span></span>|<span data-ttu-id="59277-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="59277-138">DateTime the object was last modified.</span></span> <span data-ttu-id="59277-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59277-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59277-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="59277-140">roleScopeTagIds</span></span>|<span data-ttu-id="59277-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="59277-141">String collection</span></span>|<span data-ttu-id="59277-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="59277-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="59277-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59277-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59277-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="59277-144">supportsScopeTags</span></span>|<span data-ttu-id="59277-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-145">Boolean</span></span>|<span data-ttu-id="59277-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="59277-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="59277-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="59277-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="59277-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="59277-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="59277-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="59277-149">This property is read-only.</span></span> <span data-ttu-id="59277-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59277-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59277-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="59277-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="59277-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="59277-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="59277-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="59277-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="59277-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59277-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59277-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="59277-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="59277-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="59277-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="59277-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="59277-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="59277-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59277-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59277-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="59277-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="59277-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="59277-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="59277-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="59277-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="59277-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59277-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59277-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="59277-163">createdDateTime</span></span>|<span data-ttu-id="59277-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59277-164">DateTimeOffset</span></span>|<span data-ttu-id="59277-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="59277-165">DateTime the object was created.</span></span> <span data-ttu-id="59277-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59277-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59277-167">description</span><span class="sxs-lookup"><span data-stu-id="59277-167">description</span></span>|<span data-ttu-id="59277-168">String</span><span class="sxs-lookup"><span data-stu-id="59277-168">String</span></span>|<span data-ttu-id="59277-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59277-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="59277-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59277-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59277-171">displayName</span><span class="sxs-lookup"><span data-stu-id="59277-171">displayName</span></span>|<span data-ttu-id="59277-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59277-172">String</span></span>|<span data-ttu-id="59277-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59277-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="59277-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59277-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59277-175">versão</span><span class="sxs-lookup"><span data-stu-id="59277-175">version</span></span>|<span data-ttu-id="59277-176">Int32</span><span class="sxs-lookup"><span data-stu-id="59277-176">Int32</span></span>|<span data-ttu-id="59277-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59277-177">Version of the device configuration.</span></span> <span data-ttu-id="59277-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="59277-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="59277-179">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="59277-179">accountBlockModification</span></span>|<span data-ttu-id="59277-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-180">Boolean</span></span>|<span data-ttu-id="59277-181">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-181">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-182">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="59277-182">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="59277-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-183">Boolean</span></span>|<span data-ttu-id="59277-184">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-184">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="59277-185">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-185">airDropBlocked</span></span>|<span data-ttu-id="59277-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-186">Boolean</span></span>|<span data-ttu-id="59277-187">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-187">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-188">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="59277-188">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="59277-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-189">Boolean</span></span>|<span data-ttu-id="59277-190">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-190">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="59277-191">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="59277-191">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="59277-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-192">Boolean</span></span>|<span data-ttu-id="59277-193">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="59277-193">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="59277-194">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="59277-194">appleWatchBlockPairing</span></span>|<span data-ttu-id="59277-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-195">Boolean</span></span>|<span data-ttu-id="59277-196">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-196">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="59277-197">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="59277-197">appleWatchForceWristDetection</span></span>|<span data-ttu-id="59277-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-198">Boolean</span></span>|<span data-ttu-id="59277-199">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-199">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="59277-200">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-200">appleNewsBlocked</span></span>|<span data-ttu-id="59277-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-201">Boolean</span></span>|<span data-ttu-id="59277-202">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-202">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="59277-203">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="59277-203">appsSingleAppModeList</span></span>|<span data-ttu-id="59277-204">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="59277-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="59277-205">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="59277-205">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="59277-206">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-206">Supervised only.</span></span> <span data-ttu-id="59277-207">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-207">iOS 7.0 and later.</span></span> <span data-ttu-id="59277-208">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="59277-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="59277-209">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="59277-209">appsVisibilityList</span></span>|<span data-ttu-id="59277-210">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="59277-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="59277-211">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-211">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="59277-212">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="59277-212">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="59277-213">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="59277-213">appsVisibilityListType</span></span>|[<span data-ttu-id="59277-214">appListType</span><span class="sxs-lookup"><span data-stu-id="59277-214">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="59277-215">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="59277-215">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="59277-216">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="59277-216">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="59277-217">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="59277-217">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="59277-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-218">Boolean</span></span>|<span data-ttu-id="59277-219">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-219">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="59277-220">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-220">appStoreBlocked</span></span>|<span data-ttu-id="59277-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-221">Boolean</span></span>|<span data-ttu-id="59277-222">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="59277-222">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="59277-223">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-223">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="59277-224">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="59277-224">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="59277-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-225">Boolean</span></span>|<span data-ttu-id="59277-226">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59277-226">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="59277-227">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="59277-227">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="59277-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-228">Boolean</span></span>|<span data-ttu-id="59277-229">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="59277-229">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="59277-230">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-230">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="59277-231">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="59277-231">appStoreRequirePassword</span></span>|<span data-ttu-id="59277-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-232">Boolean</span></span>|<span data-ttu-id="59277-233">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="59277-233">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="59277-234">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="59277-234">autoFillForceAuthentication</span></span>|<span data-ttu-id="59277-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-235">Boolean</span></span>|<span data-ttu-id="59277-236">Indica se a autenticação do usuário deve ou não ser forçada antes de preencher automaticamente as informações de cartão de crédito e o Safari e outros aplicativos em dispositivos supervisionados.</span><span class="sxs-lookup"><span data-stu-id="59277-236">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="59277-237">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="59277-237">bluetoothBlockModification</span></span>|<span data-ttu-id="59277-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-238">Boolean</span></span>|<span data-ttu-id="59277-239">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-239">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="59277-240">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-240">cameraBlocked</span></span>|<span data-ttu-id="59277-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-241">Boolean</span></span>|<span data-ttu-id="59277-242">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59277-242">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="59277-243">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-243">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="59277-244">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="59277-244">cellularBlockDataRoaming</span></span>|<span data-ttu-id="59277-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-245">Boolean</span></span>|<span data-ttu-id="59277-246">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="59277-246">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="59277-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="59277-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="59277-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-248">Boolean</span></span>|<span data-ttu-id="59277-249">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="59277-249">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="59277-250">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="59277-250">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="59277-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-251">Boolean</span></span>|<span data-ttu-id="59277-252">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-252">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-253">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="59277-253">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="59277-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-254">Boolean</span></span>|<span data-ttu-id="59277-255">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="59277-255">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="59277-256">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="59277-256">cellularBlockPlanModification</span></span>|<span data-ttu-id="59277-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-257">Boolean</span></span>|<span data-ttu-id="59277-258">Indica se os usuários poderão ou não alterar as configurações do plano de celular em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-258">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="59277-259">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="59277-259">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="59277-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-260">Boolean</span></span>|<span data-ttu-id="59277-261">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="59277-261">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="59277-262">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="59277-262">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="59277-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-263">Boolean</span></span>|<span data-ttu-id="59277-264">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="59277-264">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="59277-265">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="59277-265">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="59277-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-266">Boolean</span></span>|<span data-ttu-id="59277-267">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-267">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="59277-268">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="59277-268">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="59277-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-269">Boolean</span></span>|<span data-ttu-id="59277-270">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-270">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-271">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="59277-271">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="59277-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-272">Boolean</span></span>|<span data-ttu-id="59277-273">Indica se a permissão será ou não automaticamente atribuído às solicitações do professor, sem avisar o aluno, quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-273">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-274">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="59277-274">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="59277-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-275">Boolean</span></span>|<span data-ttu-id="59277-276">Indica se o professor deve ou não bloquear aplicativos ou o dispositivo sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="59277-276">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="59277-277">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-277">Supervised only.</span></span>|
|<span data-ttu-id="59277-278">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="59277-278">compliantAppsList</span></span>|<span data-ttu-id="59277-279">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="59277-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="59277-280">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="59277-280">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="59277-281">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="59277-281">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="59277-282">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="59277-282">compliantAppListType</span></span>|[<span data-ttu-id="59277-283">appListType</span><span class="sxs-lookup"><span data-stu-id="59277-283">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="59277-284">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="59277-284">List that is in the AppComplianceList.</span></span> <span data-ttu-id="59277-285">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="59277-285">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="59277-286">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="59277-286">configurationProfileBlockChanges</span></span>|<span data-ttu-id="59277-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-287">Boolean</span></span>|<span data-ttu-id="59277-288">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-288">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-289">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-289">definitionLookupBlocked</span></span>|<span data-ttu-id="59277-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-290">Boolean</span></span>|<span data-ttu-id="59277-291">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-291">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="59277-292">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="59277-292">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="59277-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-293">Boolean</span></span>|<span data-ttu-id="59277-294">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-294">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-295">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="59277-295">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="59277-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-296">Boolean</span></span>|<span data-ttu-id="59277-297">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-297">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-298">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="59277-298">deviceBlockNameModification</span></span>|<span data-ttu-id="59277-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-299">Boolean</span></span>|<span data-ttu-id="59277-300">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-300">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="59277-301">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="59277-301">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="59277-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-302">Boolean</span></span>|<span data-ttu-id="59277-303">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="59277-303">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="59277-304">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="59277-304">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="59277-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-305">Boolean</span></span>|<span data-ttu-id="59277-306">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-306">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="59277-307">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="59277-307">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="59277-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-308">Boolean</span></span>|<span data-ttu-id="59277-309">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="59277-309">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="59277-310">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="59277-310">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="59277-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-311">Boolean</span></span>|<span data-ttu-id="59277-312">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="59277-312">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="59277-313">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="59277-313">emailInDomainSuffixes</span></span>|<span data-ttu-id="59277-314">String collection</span><span class="sxs-lookup"><span data-stu-id="59277-314">String collection</span></span>|<span data-ttu-id="59277-315">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="59277-315">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="59277-316">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="59277-316">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="59277-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-317">Boolean</span></span>|<span data-ttu-id="59277-318">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="59277-318">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="59277-319">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="59277-319">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="59277-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-320">Boolean</span></span>|<span data-ttu-id="59277-321">\[\] Preterido a definição dessa configuração e a definição do valor como ' true ' não tem efeito no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59277-321">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="59277-322">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="59277-322">esimBlockModification</span></span>|<span data-ttu-id="59277-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-323">Boolean</span></span>|<span data-ttu-id="59277-324">Indica se a adição ou a remoção de planos da rede celular deve ou não ser permitida no eSIM de um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-324">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="59277-325">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-325">faceTimeBlocked</span></span>|<span data-ttu-id="59277-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-326">Boolean</span></span>|<span data-ttu-id="59277-327">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="59277-327">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="59277-328">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-328">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="59277-329">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-329">findMyFriendsBlocked</span></span>|<span data-ttu-id="59277-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-330">Boolean</span></span>|<span data-ttu-id="59277-331">Indica se as alterações serão bloqueadas ou não para localizar meus amigos quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-331">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-332">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="59277-332">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="59277-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-333">Boolean</span></span>|<span data-ttu-id="59277-334">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="59277-334">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="59277-335">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-335">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="59277-336">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="59277-336">gamingBlockMultiplayer</span></span>|<span data-ttu-id="59277-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-337">Boolean</span></span>|<span data-ttu-id="59277-338">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="59277-338">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="59277-339">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-339">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="59277-340">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-340">gameCenterBlocked</span></span>|<span data-ttu-id="59277-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-341">Boolean</span></span>|<span data-ttu-id="59277-342">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-342">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-343">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-343">hostPairingBlocked</span></span>|<span data-ttu-id="59277-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-344">Boolean</span></span>|<span data-ttu-id="59277-345">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-345">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-346">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-346">iBooksStoreBlocked</span></span>|<span data-ttu-id="59277-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-347">Boolean</span></span>|<span data-ttu-id="59277-348">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-348">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-349">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="59277-349">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="59277-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-350">Boolean</span></span>|<span data-ttu-id="59277-351">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="59277-351">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="59277-352">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="59277-352">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="59277-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-353">Boolean</span></span>|<span data-ttu-id="59277-354">Indica se o usuário será ou não impedido de continuar o trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="59277-354">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="59277-355">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="59277-355">iCloudBlockBackup</span></span>|<span data-ttu-id="59277-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-356">Boolean</span></span>|<span data-ttu-id="59277-357">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="59277-357">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="59277-358">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-358">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="59277-359">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="59277-359">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="59277-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-360">Boolean</span></span>|<span data-ttu-id="59277-361">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada. Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-361">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="59277-362">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="59277-362">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="59277-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-363">Boolean</span></span>|<span data-ttu-id="59277-364">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="59277-364">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="59277-365">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="59277-365">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="59277-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-366">Boolean</span></span>|<span data-ttu-id="59277-367">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="59277-367">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="59277-368">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="59277-368">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="59277-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-369">Boolean</span></span>|<span data-ttu-id="59277-370">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="59277-370">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="59277-371">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="59277-371">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="59277-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-372">Boolean</span></span>|<span data-ttu-id="59277-373">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="59277-373">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="59277-374">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="59277-374">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="59277-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-375">Boolean</span></span>|<span data-ttu-id="59277-376">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="59277-376">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="59277-377">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="59277-377">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="59277-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-378">Boolean</span></span>|<span data-ttu-id="59277-379">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="59277-379">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="59277-380">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-380">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="59277-381">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="59277-381">iTunesBlockMusicService</span></span>|<span data-ttu-id="59277-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-382">Boolean</span></span>|<span data-ttu-id="59277-383">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-383">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="59277-384">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="59277-384">iTunesBlockRadio</span></span>|<span data-ttu-id="59277-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-385">Boolean</span></span>|<span data-ttu-id="59277-386">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-386">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="59277-387">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="59277-387">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="59277-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-388">Boolean</span></span>|<span data-ttu-id="59277-389">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-389">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="59277-390">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="59277-390">keyboardBlockDictation</span></span>|<span data-ttu-id="59277-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-391">Boolean</span></span>|<span data-ttu-id="59277-392">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-392">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-393">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="59277-393">keyboardBlockPredictive</span></span>|<span data-ttu-id="59277-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-394">Boolean</span></span>|<span data-ttu-id="59277-395">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-395">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="59277-396">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="59277-396">keyboardBlockShortcuts</span></span>|<span data-ttu-id="59277-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-397">Boolean</span></span>|<span data-ttu-id="59277-398">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-398">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="59277-399">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="59277-399">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="59277-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-400">Boolean</span></span>|<span data-ttu-id="59277-401">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-401">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="59277-402">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="59277-402">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="59277-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-403">Boolean</span></span>|<span data-ttu-id="59277-404">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-404">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-405">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="59277-405">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="59277-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-406">Boolean</span></span>|<span data-ttu-id="59277-407">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-407">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-408">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="59277-408">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="59277-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-409">Boolean</span></span>|<span data-ttu-id="59277-410">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-410">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="59277-411">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="59277-411">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="59277-412">Use KioskModeBlockAutoLock em vez disso.</span><span class="sxs-lookup"><span data-stu-id="59277-412">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="59277-413">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="59277-413">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="59277-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-414">Boolean</span></span>|<span data-ttu-id="59277-415">Indica se o bloqueio automático do dispositivo deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-415">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-416">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="59277-416">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="59277-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-417">Boolean</span></span>|<span data-ttu-id="59277-418">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-418">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-419">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="59277-419">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="59277-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-420">Boolean</span></span>|<span data-ttu-id="59277-421">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-421">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="59277-422">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="59277-422">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="59277-423">Use KioskModeBlockRingerSwitch em vez disso.</span><span class="sxs-lookup"><span data-stu-id="59277-423">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="59277-424">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="59277-424">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="59277-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-425">Boolean</span></span>|<span data-ttu-id="59277-426">Indica se o uso do comutador de toque deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-426">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-427">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="59277-427">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="59277-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-428">Boolean</span></span>|<span data-ttu-id="59277-429">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-429">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="59277-430">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="59277-430">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="59277-431">Use KioskModeBlockScreenRotation em vez disso.</span><span class="sxs-lookup"><span data-stu-id="59277-431">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="59277-432">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="59277-432">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="59277-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-433">Boolean</span></span>|<span data-ttu-id="59277-434">Indica se a rotação de tela deve ou não ser bloqueada enquanto estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-434">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-435">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="59277-435">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="59277-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-436">Boolean</span></span>|<span data-ttu-id="59277-437">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-437">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="59277-438">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="59277-438">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="59277-439">Use KioskModeBlockSleepButton em vez disso.</span><span class="sxs-lookup"><span data-stu-id="59277-439">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="59277-440">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="59277-440">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="59277-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-441">Boolean</span></span>|<span data-ttu-id="59277-442">Indica se o uso do botão de suspensão deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-442">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-443">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="59277-443">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="59277-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-444">Boolean</span></span>|<span data-ttu-id="59277-445">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-445">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="59277-446">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="59277-446">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="59277-447">Use KioskModeBlockTouchscreen em vez disso.</span><span class="sxs-lookup"><span data-stu-id="59277-447">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="59277-448">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="59277-448">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="59277-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-449">Boolean</span></span>|<span data-ttu-id="59277-450">Indica se o uso da tela de toque deve ou não ser bloqueado enquanto estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-450">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-451">kioskModeEnableVoiceControl</span><span class="sxs-lookup"><span data-stu-id="59277-451">kioskModeEnableVoiceControl</span></span>|<span data-ttu-id="59277-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-452">Boolean</span></span>|<span data-ttu-id="59277-453">Indica se o controle de voz deve ou não ser habilitado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-453">Indicates whether or not to enable voice control in kiosk mode.</span></span>|
|<span data-ttu-id="59277-454">kioskModeAllowVoiceControlModification</span><span class="sxs-lookup"><span data-stu-id="59277-454">kioskModeAllowVoiceControlModification</span></span>|<span data-ttu-id="59277-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-455">Boolean</span></span>|<span data-ttu-id="59277-456">Indica se o usuário deve ou não permitir a alternância de controle de voz no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-456">Indicates whether or not to allow the user to toggle voice control in kiosk mode.</span></span>|
|<span data-ttu-id="59277-457">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="59277-457">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="59277-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-458">Boolean</span></span>|<span data-ttu-id="59277-459">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-459">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-460">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="59277-460">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="59277-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-461">Boolean</span></span>|<span data-ttu-id="59277-462">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-462">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="59277-463">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="59277-463">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="59277-464">Use KioskModeBlockVolumeButtons em vez disso.</span><span class="sxs-lookup"><span data-stu-id="59277-464">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="59277-465">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="59277-465">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="59277-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-466">Boolean</span></span>|<span data-ttu-id="59277-467">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-467">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="59277-468">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="59277-468">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="59277-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-469">Boolean</span></span>|<span data-ttu-id="59277-470">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-470">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-471">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="59277-471">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="59277-472">String</span><span class="sxs-lookup"><span data-stu-id="59277-472">String</span></span>|<span data-ttu-id="59277-473">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-473">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="59277-474">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="59277-474">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="59277-475">Propriedadekioskmodebuiltinappid</span><span class="sxs-lookup"><span data-stu-id="59277-475">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="59277-476">String</span><span class="sxs-lookup"><span data-stu-id="59277-476">String</span></span>|<span data-ttu-id="59277-477">ID para aplicativos internos a serem usados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-477">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="59277-478">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidos.</span><span class="sxs-lookup"><span data-stu-id="59277-478">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="59277-479">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="59277-479">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="59277-480">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-480">Boolean</span></span>|<span data-ttu-id="59277-481">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-481">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-482">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="59277-482">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="59277-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-483">Boolean</span></span>|<span data-ttu-id="59277-484">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-484">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-485">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="59277-485">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="59277-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-486">Boolean</span></span>|<span data-ttu-id="59277-487">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-487">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-488">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="59277-488">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="59277-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-489">Boolean</span></span>|<span data-ttu-id="59277-490">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-490">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-491">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="59277-491">kioskModeRequireZoom</span></span>|<span data-ttu-id="59277-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-492">Boolean</span></span>|<span data-ttu-id="59277-493">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-493">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="59277-494">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="59277-494">kioskModeManagedAppId</span></span>|<span data-ttu-id="59277-495">String</span><span class="sxs-lookup"><span data-stu-id="59277-495">String</span></span>|<span data-ttu-id="59277-496">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-496">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="59277-497">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="59277-497">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="59277-498">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="59277-498">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="59277-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-499">Boolean</span></span>|<span data-ttu-id="59277-500">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="59277-500">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="59277-501">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="59277-501">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="59277-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-502">Boolean</span></span>|<span data-ttu-id="59277-503">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="59277-503">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="59277-504">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="59277-504">lockScreenBlockPassbook</span></span>|<span data-ttu-id="59277-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-505">Boolean</span></span>|<span data-ttu-id="59277-506">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="59277-506">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="59277-507">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="59277-507">lockScreenBlockTodayView</span></span>|<span data-ttu-id="59277-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-508">Boolean</span></span>|<span data-ttu-id="59277-509">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="59277-509">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="59277-510">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="59277-510">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="59277-511">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="59277-511">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="59277-512">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="59277-512">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="59277-513">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="59277-513">mediaContentRatingCanada</span></span>|[<span data-ttu-id="59277-514">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="59277-514">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="59277-515">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="59277-515">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="59277-516">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="59277-516">mediaContentRatingFrance</span></span>|[<span data-ttu-id="59277-517">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="59277-517">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="59277-518">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="59277-518">Media content rating settings for France</span></span>|
|<span data-ttu-id="59277-519">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="59277-519">mediaContentRatingGermany</span></span>|[<span data-ttu-id="59277-520">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="59277-520">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="59277-521">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="59277-521">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="59277-522">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="59277-522">mediaContentRatingIreland</span></span>|[<span data-ttu-id="59277-523">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="59277-523">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="59277-524">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="59277-524">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="59277-525">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="59277-525">mediaContentRatingJapan</span></span>|[<span data-ttu-id="59277-526">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="59277-526">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="59277-527">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="59277-527">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="59277-528">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="59277-528">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="59277-529">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="59277-529">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="59277-530">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="59277-530">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="59277-531">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="59277-531">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="59277-532">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="59277-532">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="59277-533">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="59277-533">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="59277-534">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="59277-534">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="59277-535">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="59277-535">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="59277-536">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="59277-536">Media content rating settings for United States</span></span>|
|<span data-ttu-id="59277-537">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="59277-537">networkUsageRules</span></span>|<span data-ttu-id="59277-538">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="59277-538">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="59277-539">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="59277-539">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="59277-540">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="59277-540">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="59277-541">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="59277-541">mediaContentRatingApps</span></span>|[<span data-ttu-id="59277-542">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="59277-542">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="59277-543">Configurações de classificação de conteúdo de mídia para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="59277-543">Media content rating settings for Apps.</span></span> <span data-ttu-id="59277-544">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="59277-544">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="59277-545">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-545">messagesBlocked</span></span>|<span data-ttu-id="59277-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-546">Boolean</span></span>|<span data-ttu-id="59277-547">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-547">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="59277-548">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="59277-548">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="59277-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-549">Boolean</span></span>|<span data-ttu-id="59277-550">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-550">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="59277-551">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="59277-551">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="59277-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-552">Boolean</span></span>|<span data-ttu-id="59277-553">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="59277-553">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="59277-554">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="59277-554">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="59277-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-555">Boolean</span></span>|<span data-ttu-id="59277-556">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-556">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="59277-557">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="59277-557">passcodeBlockModification</span></span>|<span data-ttu-id="59277-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-558">Boolean</span></span>|<span data-ttu-id="59277-559">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-559">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="59277-560">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="59277-560">passcodeBlockSimple</span></span>|<span data-ttu-id="59277-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-561">Boolean</span></span>|<span data-ttu-id="59277-562">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="59277-562">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="59277-563">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="59277-563">passcodeExpirationDays</span></span>|<span data-ttu-id="59277-564">Int32</span><span class="sxs-lookup"><span data-stu-id="59277-564">Int32</span></span>|<span data-ttu-id="59277-565">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="59277-565">Number of days before the passcode expires.</span></span> <span data-ttu-id="59277-566">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="59277-566">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="59277-567">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="59277-567">passcodeMinimumLength</span></span>|<span data-ttu-id="59277-568">Int32</span><span class="sxs-lookup"><span data-stu-id="59277-568">Int32</span></span>|<span data-ttu-id="59277-569">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="59277-569">Minimum length of passcode.</span></span> <span data-ttu-id="59277-570">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="59277-570">Valid values 4 to 14</span></span>|
|<span data-ttu-id="59277-571">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="59277-571">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="59277-572">Int32</span><span class="sxs-lookup"><span data-stu-id="59277-572">Int32</span></span>|<span data-ttu-id="59277-573">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="59277-573">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="59277-574">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="59277-574">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="59277-575">Int32</span><span class="sxs-lookup"><span data-stu-id="59277-575">Int32</span></span>|<span data-ttu-id="59277-576">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="59277-576">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="59277-577">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="59277-577">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="59277-578">Int32</span><span class="sxs-lookup"><span data-stu-id="59277-578">Int32</span></span>|<span data-ttu-id="59277-579">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="59277-579">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="59277-580">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="59277-580">Valid values 0 to 4</span></span>|
|<span data-ttu-id="59277-581">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="59277-581">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="59277-582">Int32</span><span class="sxs-lookup"><span data-stu-id="59277-582">Int32</span></span>|<span data-ttu-id="59277-583">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="59277-583">Number of previous passcodes to block.</span></span> <span data-ttu-id="59277-584">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="59277-584">Valid values 1 to 24</span></span>|
|<span data-ttu-id="59277-585">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="59277-585">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="59277-586">Int32</span><span class="sxs-lookup"><span data-stu-id="59277-586">Int32</span></span>|<span data-ttu-id="59277-587">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="59277-587">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="59277-588">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="59277-588">Valid values 4 to 11</span></span>|
|<span data-ttu-id="59277-589">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="59277-589">passcodeRequiredType</span></span>|[<span data-ttu-id="59277-590">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="59277-590">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="59277-591">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="59277-591">Type of passcode that is required.</span></span> <span data-ttu-id="59277-592">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="59277-592">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="59277-593">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="59277-593">passcodeRequired</span></span>|<span data-ttu-id="59277-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-594">Boolean</span></span>|<span data-ttu-id="59277-595">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="59277-595">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="59277-596">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-596">podcastsBlocked</span></span>|<span data-ttu-id="59277-597">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-597">Boolean</span></span>|<span data-ttu-id="59277-598">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-598">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="59277-599">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="59277-599">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="59277-600">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-600">Boolean</span></span>|<span data-ttu-id="59277-601">Indica se o prompt deve ou não ser habilitado para configurar dispositivos próximos com um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-601">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="59277-602">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="59277-602">safariBlockAutofill</span></span>|<span data-ttu-id="59277-603">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-603">Boolean</span></span>|<span data-ttu-id="59277-604">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="59277-604">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="59277-605">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-605">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="59277-606">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="59277-606">safariBlockJavaScript</span></span>|<span data-ttu-id="59277-607">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-607">Boolean</span></span>|<span data-ttu-id="59277-608">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="59277-608">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="59277-609">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="59277-609">safariBlockPopups</span></span>|<span data-ttu-id="59277-610">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-610">Boolean</span></span>|<span data-ttu-id="59277-611">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="59277-611">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="59277-612">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-612">safariBlocked</span></span>|<span data-ttu-id="59277-613">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-613">Boolean</span></span>|<span data-ttu-id="59277-614">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="59277-614">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="59277-615">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-615">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="59277-616">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="59277-616">safariCookieSettings</span></span>|[<span data-ttu-id="59277-617">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="59277-617">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="59277-618">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="59277-618">Cookie settings for Safari.</span></span> <span data-ttu-id="59277-619">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="59277-619">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="59277-620">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="59277-620">safariManagedDomains</span></span>|<span data-ttu-id="59277-621">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="59277-621">String collection</span></span>|<span data-ttu-id="59277-622">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="59277-622">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="59277-623">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="59277-623">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="59277-624">String collection</span><span class="sxs-lookup"><span data-stu-id="59277-624">String collection</span></span>|<span data-ttu-id="59277-625">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="59277-625">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="59277-626">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-626">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="59277-627">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="59277-627">safariRequireFraudWarning</span></span>|<span data-ttu-id="59277-628">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-628">Boolean</span></span>|<span data-ttu-id="59277-629">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="59277-629">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="59277-630">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-630">screenCaptureBlocked</span></span>|<span data-ttu-id="59277-631">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-631">Boolean</span></span>|<span data-ttu-id="59277-632">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="59277-632">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="59277-633">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-633">siriBlocked</span></span>|<span data-ttu-id="59277-634">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-634">Boolean</span></span>|<span data-ttu-id="59277-635">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="59277-635">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="59277-636">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="59277-636">siriBlockedWhenLocked</span></span>|<span data-ttu-id="59277-637">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-637">Boolean</span></span>|<span data-ttu-id="59277-638">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="59277-638">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="59277-639">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="59277-639">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="59277-640">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-640">Boolean</span></span>|<span data-ttu-id="59277-641">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-641">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="59277-642">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="59277-642">siriRequireProfanityFilter</span></span>|<span data-ttu-id="59277-643">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-643">Boolean</span></span>|<span data-ttu-id="59277-644">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-644">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="59277-645">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="59277-645">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="59277-646">Int32</span><span class="sxs-lookup"><span data-stu-id="59277-646">Int32</span></span>|<span data-ttu-id="59277-647">Define o número de dias que uma atualização de software será delyed para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-647">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="59277-648">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="59277-648">Valid values 0 to 90</span></span>|
|<span data-ttu-id="59277-649">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="59277-649">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="59277-650">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-650">Boolean</span></span>|<span data-ttu-id="59277-651">Indica se o usuário deve ou não atrasar a visibilidade de atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-651">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-652">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="59277-652">spotlightBlockInternetResults</span></span>|<span data-ttu-id="59277-653">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-653">Boolean</span></span>|<span data-ttu-id="59277-654">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-654">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="59277-655">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-655">voiceDialingBlocked</span></span>|<span data-ttu-id="59277-656">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-656">Boolean</span></span>|<span data-ttu-id="59277-657">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="59277-657">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="59277-658">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="59277-658">wallpaperBlockModification</span></span>|<span data-ttu-id="59277-659">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-659">Boolean</span></span>|<span data-ttu-id="59277-660">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-660">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="59277-661">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="59277-661">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="59277-662">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-662">Boolean</span></span>|<span data-ttu-id="59277-663">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="59277-663">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="59277-664">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="59277-664">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="59277-665">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-665">Boolean</span></span>|<span data-ttu-id="59277-666">Indica se um aluno inscrito em um curso não gerenciado via sala de aula solicitará permissão do professor ao tentar sair do curso (iOS 11,3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-666">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="59277-667">Propriedadeskeychainblockcloudsync</span><span class="sxs-lookup"><span data-stu-id="59277-667">keychainBlockCloudSync</span></span>|<span data-ttu-id="59277-668">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-668">Boolean</span></span>|<span data-ttu-id="59277-669">Indica se a sincronização de chaves do iCloud está bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="59277-669">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="59277-670">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-670">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="59277-671">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="59277-671">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="59277-672">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-672">Boolean</span></span>|<span data-ttu-id="59277-673">Indica se as atualizações de PKI de over-the-Air serão bloqueadas ou não.</span><span class="sxs-lookup"><span data-stu-id="59277-673">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="59277-674">A definição dessa restrição como false não desabilita as verificações de CRL e OCSP (iOS 7,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-674">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="59277-675">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="59277-675">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="59277-676">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-676">Boolean</span></span>|<span data-ttu-id="59277-677">Indica se o controle do AD é limitado. (iOS 7,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-677">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="59277-678">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="59277-678">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="59277-679">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-679">Boolean</span></span>|<span data-ttu-id="59277-680">Indica se o backup do catálogo empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="59277-680">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="59277-681">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="59277-681">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="59277-682">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-682">Boolean</span></span>|<span data-ttu-id="59277-683">Indica se a sincronização de notas e destaques do catálogo empresarial será bloqueada.</span><span class="sxs-lookup"><span data-stu-id="59277-683">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="59277-684">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-684">airPrintBlocked</span></span>|<span data-ttu-id="59277-685">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-685">Boolean</span></span>|<span data-ttu-id="59277-686">Indica se o arquivo de impressão está bloqueado ou não (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-686">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="59277-687">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="59277-687">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="59277-688">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-688">Boolean</span></span>|<span data-ttu-id="59277-689">Indica se o armazenamento de chaves de nome de usuário e a senha para impressão de uma ou não é bloqueado (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-689">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="59277-690">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="59277-690">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="59277-691">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-691">Boolean</span></span>|<span data-ttu-id="59277-692">Indica se os certificados confiáveis são necessários para a comunicação de impressão TLS (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-692">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="59277-693">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="59277-693">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="59277-694">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-694">Boolean</span></span>|<span data-ttu-id="59277-695">Indica se a descoberta de impressoras de impressão do iBeacon está ou não bloqueada.</span><span class="sxs-lookup"><span data-stu-id="59277-695">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="59277-696">Isso impede os beacons Bluetooth de impressão de mensagens de phishing para tráfego de rede (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-696">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="59277-697">filesNetworkDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-697">filesNetworkDriveAccessBlocked</span></span>|<span data-ttu-id="59277-698">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-698">Boolean</span></span>|<span data-ttu-id="59277-699">Indica se os dispositivos podem acessar arquivos ou outros recursos em um servidor de rede usando o protocolo SMB (bloco de mensagens de servidor).</span><span class="sxs-lookup"><span data-stu-id="59277-699">Indicates if devices can access files or other resources on a network server using the Server Message Block (SMB) protocol.</span></span> <span data-ttu-id="59277-700">Disponível para dispositivos que executam o iOS e o iPadOS, versões 13,0 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="59277-700">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="59277-701">filesUsbDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-701">filesUsbDriveAccessBlocked</span></span>|<span data-ttu-id="59277-702">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-702">Boolean</span></span>|<span data-ttu-id="59277-703">Indica se o sevices com o Access pode se conectar a arquivos e abri-los em uma unidade USB.</span><span class="sxs-lookup"><span data-stu-id="59277-703">Indicates if sevices with access can connect to and open files on a USB drive.</span></span> <span data-ttu-id="59277-704">Disponível para dispositivos que executam o iOS e o iPadOS, versões 13,0 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="59277-704">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="59277-705">wifiPowerOnForced</span><span class="sxs-lookup"><span data-stu-id="59277-705">wifiPowerOnForced</span></span>|<span data-ttu-id="59277-706">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-706">Boolean</span></span>|<span data-ttu-id="59277-707">Indica se o Wi-Fi permanecerá ou não, mesmo quando o dispositivo estiver no modo avião.</span><span class="sxs-lookup"><span data-stu-id="59277-707">Indicates whether or not Wi-Fi remains on, even when device is in airplane mode.</span></span> <span data-ttu-id="59277-708">Disponível para dispositivos que executam o iOS e o iPadOS, versões 13,0 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="59277-708">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="59277-709">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="59277-709">blockSystemAppRemoval</span></span>|<span data-ttu-id="59277-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-710">Boolean</span></span>|<span data-ttu-id="59277-711">Indica se a remoção de aplicativos do sistema do dispositivo é bloqueada em um dispositivo supervisionado (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-711">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="59277-712">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="59277-712">vpnBlockCreation</span></span>|<span data-ttu-id="59277-713">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-713">Boolean</span></span>|<span data-ttu-id="59277-714">Indica se a criação de configurações de VPN está bloqueada (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-714">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="59277-715">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-715">appRemovalBlocked</span></span>|<span data-ttu-id="59277-716">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-716">Boolean</span></span>|<span data-ttu-id="59277-717">Indica se a remoção de aplicativos é permitida.</span><span class="sxs-lookup"><span data-stu-id="59277-717">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="59277-718">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-718">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="59277-719">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-719">Boolean</span></span>|<span data-ttu-id="59277-720">Indica se a conexão a acessórios USB enquanto o dispositivo está bloqueado é permitida (iOS 11.4.1 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-720">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="59277-721">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="59277-721">passwordBlockAutoFill</span></span>|<span data-ttu-id="59277-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-722">Boolean</span></span>|<span data-ttu-id="59277-723">Indica se o recurso de senha de preenchimento automático é permitido (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-723">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="59277-724">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="59277-724">passwordBlockProximityRequests</span></span>|<span data-ttu-id="59277-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-725">Boolean</span></span>|<span data-ttu-id="59277-726">Indica se as senhas de solicitação devem ou não ser bloqueadas de dispositivos próximos (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-726">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="59277-727">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="59277-727">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="59277-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-728">Boolean</span></span>|<span data-ttu-id="59277-729">Indica se as senhas de compartilhamento devem ou não ser bloqueadas com o recurso de senhas de soltura de estours iOS 12,0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="59277-729">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="59277-730">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="59277-730">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="59277-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-731">Boolean</span></span>|<span data-ttu-id="59277-732">Indica se o recurso "definir automaticamente" de data e hora está habilitado e não pode ser desativado pelo usuário (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-732">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="59277-733">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="59277-733">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="59277-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-734">Boolean</span></span>|<span data-ttu-id="59277-735">Indica se os aplicativos gerenciados podem ou não gravar contatos para contas de contatos não gerenciados (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-735">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="59277-736">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="59277-736">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="59277-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-737">Boolean</span></span>|<span data-ttu-id="59277-738">Indica se os aplicativos não gerenciados podem ler de contas de contatos gerenciados (iOS 12,0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-738">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="59277-739">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="59277-739">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="59277-740">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-740">Boolean</span></span>|<span data-ttu-id="59277-741">Indica se o usuário será ou não impedido de modificar a configuração de hotspot pessoal (iOS 12,2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-741">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="59277-742">continuousPathKeyboardBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-742">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="59277-743">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-743">Boolean</span></span>|<span data-ttu-id="59277-744">Indica se o teclado de caminho contínuo será ou não bloqueado quando o dispositivo for supervisionado (iOS 13 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-744">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="59277-745">findMyDeviceInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-745">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="59277-746">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-746">Boolean</span></span>|<span data-ttu-id="59277-747">Indica se a localização do dispositivo deve ou não ser bloqueada quando o dispositivo é supervisionado (iOS 13 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-747">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="59277-748">findMyFriendsInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-748">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="59277-749">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-749">Boolean</span></span>|<span data-ttu-id="59277-750">Indica se a localização de meus amigos deve ou não ser bloqueada quando o dispositivo é supervisionado (iOS 13 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="59277-750">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="59277-751">iTunesBlocked</span><span class="sxs-lookup"><span data-stu-id="59277-751">iTunesBlocked</span></span>|<span data-ttu-id="59277-752">Boolean</span><span class="sxs-lookup"><span data-stu-id="59277-752">Boolean</span></span>|<span data-ttu-id="59277-753">Indica se o aplicativo iTunes deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="59277-753">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="59277-754">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="59277-754">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="59277-755">kioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="59277-755">kioskModeAppType</span></span>|[<span data-ttu-id="59277-756">iosKioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="59277-756">iosKioskModeAppType</span></span>](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|<span data-ttu-id="59277-757">Tipo de aplicativo a ser executado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="59277-757">Type of app to run in kiosk mode.</span></span> <span data-ttu-id="59277-758">Os valores possíveis são: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span><span class="sxs-lookup"><span data-stu-id="59277-758">Possible values are: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span></span>|



## <a name="response"></a><span data-ttu-id="59277-759">Resposta</span><span class="sxs-lookup"><span data-stu-id="59277-759">Response</span></span>
<span data-ttu-id="59277-760">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59277-760">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59277-761">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59277-761">Example</span></span>

### <a name="request"></a><span data-ttu-id="59277-762">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59277-762">Request</span></span>
<span data-ttu-id="59277-763">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59277-763">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 10518

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  "kioskModeEnableVoiceControl": true,
  "kioskModeAllowVoiceControlModification": true,
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
  "filesNetworkDriveAccessBlocked": true,
  "filesUsbDriveAccessBlocked": true,
  "wifiPowerOnForced": true,
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
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true,
  "kioskModeAppType": "appStoreApp"
}
```

### <a name="response"></a><span data-ttu-id="59277-764">Resposta</span><span class="sxs-lookup"><span data-stu-id="59277-764">Response</span></span>
<span data-ttu-id="59277-p157">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59277-p157">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10690

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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
  "kioskModeEnableVoiceControl": true,
  "kioskModeAllowVoiceControlModification": true,
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
  "filesNetworkDriveAccessBlocked": true,
  "filesUsbDriveAccessBlocked": true,
  "wifiPowerOnForced": true,
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
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true,
  "kioskModeAppType": "appStoreApp"
}
```




