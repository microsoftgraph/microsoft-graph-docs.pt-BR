---
title: Criar iosGeneralDeviceConfiguration
description: Cria um novo objeto iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b99635930039df180bf5caf8de86f01892748f80
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147928"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="bc42a-103">Criar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bc42a-103">Create iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="bc42a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc42a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc42a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc42a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc42a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc42a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc42a-107">Cria um novo objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bc42a-107">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc42a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bc42a-108">Prerequisites</span></span>
<span data-ttu-id="bc42a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc42a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc42a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc42a-111">Permission type</span></span>|<span data-ttu-id="bc42a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc42a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc42a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc42a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc42a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc42a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc42a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc42a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc42a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc42a-116">Not supported.</span></span>|
|<span data-ttu-id="bc42a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc42a-117">Application</span></span>|<span data-ttu-id="bc42a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc42a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc42a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc42a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bc42a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc42a-120">Request headers</span></span>
|<span data-ttu-id="bc42a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bc42a-121">Header</span></span>|<span data-ttu-id="bc42a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bc42a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc42a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc42a-123">Authorization</span></span>|<span data-ttu-id="bc42a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc42a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc42a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bc42a-125">Accept</span></span>|<span data-ttu-id="bc42a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc42a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc42a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc42a-127">Request body</span></span>
<span data-ttu-id="bc42a-128">No corpo da solicitação, forneça uma representação JSON do objeto iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bc42a-128">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="bc42a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bc42a-129">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="bc42a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc42a-130">Property</span></span>|<span data-ttu-id="bc42a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc42a-131">Type</span></span>|<span data-ttu-id="bc42a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc42a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc42a-133">id</span><span class="sxs-lookup"><span data-stu-id="bc42a-133">id</span></span>|<span data-ttu-id="bc42a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc42a-134">String</span></span>|<span data-ttu-id="bc42a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bc42a-135">Key of the entity.</span></span> <span data-ttu-id="bc42a-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc42a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc42a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bc42a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc42a-138">DateTimeOffset</span></span>|<span data-ttu-id="bc42a-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bc42a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bc42a-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc42a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bc42a-141">roleScopeTagIds</span></span>|<span data-ttu-id="bc42a-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc42a-142">String collection</span></span>|<span data-ttu-id="bc42a-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="bc42a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bc42a-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc42a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bc42a-145">supportsScopeTags</span></span>|<span data-ttu-id="bc42a-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-146">Boolean</span></span>|<span data-ttu-id="bc42a-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="bc42a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bc42a-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="bc42a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bc42a-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="bc42a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bc42a-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc42a-150">This property is read-only.</span></span> <span data-ttu-id="bc42a-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc42a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bc42a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="bc42a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="bc42a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="bc42a-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="bc42a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="bc42a-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc42a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bc42a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="bc42a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="bc42a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="bc42a-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="bc42a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="bc42a-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc42a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bc42a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="bc42a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="bc42a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="bc42a-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="bc42a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="bc42a-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc42a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc42a-164">createdDateTime</span></span>|<span data-ttu-id="bc42a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc42a-165">DateTimeOffset</span></span>|<span data-ttu-id="bc42a-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-166">DateTime the object was created.</span></span> <span data-ttu-id="bc42a-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc42a-168">descrição</span><span class="sxs-lookup"><span data-stu-id="bc42a-168">description</span></span>|<span data-ttu-id="bc42a-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc42a-169">String</span></span>|<span data-ttu-id="bc42a-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc42a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bc42a-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc42a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="bc42a-172">displayName</span></span>|<span data-ttu-id="bc42a-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc42a-173">String</span></span>|<span data-ttu-id="bc42a-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc42a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bc42a-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc42a-176">versão</span><span class="sxs-lookup"><span data-stu-id="bc42a-176">version</span></span>|<span data-ttu-id="bc42a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bc42a-177">Int32</span></span>|<span data-ttu-id="bc42a-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc42a-178">Version of the device configuration.</span></span> <span data-ttu-id="bc42a-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bc42a-180">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-180">accountBlockModification</span></span>|<span data-ttu-id="bc42a-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-181">Boolean</span></span>|<span data-ttu-id="bc42a-182">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-182">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-183">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="bc42a-183">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="bc42a-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-184">Boolean</span></span>|<span data-ttu-id="bc42a-185">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-185">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="bc42a-186">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-186">airDropBlocked</span></span>|<span data-ttu-id="bc42a-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-187">Boolean</span></span>|<span data-ttu-id="bc42a-188">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-188">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-189">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="bc42a-189">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="bc42a-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-190">Boolean</span></span>|<span data-ttu-id="bc42a-191">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-191">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="bc42a-192">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="bc42a-192">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="bc42a-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-193">Boolean</span></span>|<span data-ttu-id="bc42a-194">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="bc42a-194">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="bc42a-195">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="bc42a-195">appleWatchBlockPairing</span></span>|<span data-ttu-id="bc42a-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-196">Boolean</span></span>|<span data-ttu-id="bc42a-197">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-197">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="bc42a-198">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="bc42a-198">appleWatchForceWristDetection</span></span>|<span data-ttu-id="bc42a-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-199">Boolean</span></span>|<span data-ttu-id="bc42a-200">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-200">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="bc42a-201">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-201">appleNewsBlocked</span></span>|<span data-ttu-id="bc42a-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-202">Boolean</span></span>|<span data-ttu-id="bc42a-203">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-203">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="bc42a-204">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="bc42a-204">appsSingleAppModeList</span></span>|<span data-ttu-id="bc42a-205">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bc42a-206">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="bc42a-206">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="bc42a-207">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-207">Supervised only.</span></span> <span data-ttu-id="bc42a-208">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-208">iOS 7.0 and later.</span></span> <span data-ttu-id="bc42a-209">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="bc42a-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="bc42a-210">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="bc42a-210">appsVisibilityList</span></span>|<span data-ttu-id="bc42a-211">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-211">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bc42a-212">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-212">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="bc42a-213">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="bc42a-213">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="bc42a-214">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="bc42a-214">appsVisibilityListType</span></span>|[<span data-ttu-id="bc42a-215">appListType</span><span class="sxs-lookup"><span data-stu-id="bc42a-215">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="bc42a-216">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="bc42a-216">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="bc42a-217">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="bc42a-217">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="bc42a-218">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="bc42a-218">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="bc42a-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-219">Boolean</span></span>|<span data-ttu-id="bc42a-220">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-220">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="bc42a-221">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-221">appStoreBlocked</span></span>|<span data-ttu-id="bc42a-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-222">Boolean</span></span>|<span data-ttu-id="bc42a-223">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="bc42a-223">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="bc42a-224">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-224">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="bc42a-225">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="bc42a-225">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="bc42a-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-226">Boolean</span></span>|<span data-ttu-id="bc42a-227">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bc42a-227">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="bc42a-228">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="bc42a-228">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="bc42a-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-229">Boolean</span></span>|<span data-ttu-id="bc42a-230">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="bc42a-230">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="bc42a-231">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-231">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="bc42a-232">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="bc42a-232">appStoreRequirePassword</span></span>|<span data-ttu-id="bc42a-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-233">Boolean</span></span>|<span data-ttu-id="bc42a-234">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="bc42a-234">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="bc42a-235">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="bc42a-235">autoFillForceAuthentication</span></span>|<span data-ttu-id="bc42a-236">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-236">Boolean</span></span>|<span data-ttu-id="bc42a-237">Indica se a autenticação do usuário deve ou não forçar o preenchimento automático de senhas e informações de cartão de crédito no Safari e em outros aplicativos em dispositivos supervisionados.</span><span class="sxs-lookup"><span data-stu-id="bc42a-237">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="bc42a-238">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-238">bluetoothBlockModification</span></span>|<span data-ttu-id="bc42a-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-239">Boolean</span></span>|<span data-ttu-id="bc42a-240">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-240">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="bc42a-241">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-241">cameraBlocked</span></span>|<span data-ttu-id="bc42a-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-242">Boolean</span></span>|<span data-ttu-id="bc42a-243">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc42a-243">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="bc42a-244">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-244">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="bc42a-245">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="bc42a-245">cellularBlockDataRoaming</span></span>|<span data-ttu-id="bc42a-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-246">Boolean</span></span>|<span data-ttu-id="bc42a-247">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-247">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="bc42a-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="bc42a-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="bc42a-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-249">Boolean</span></span>|<span data-ttu-id="bc42a-250">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="bc42a-250">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="bc42a-251">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-251">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="bc42a-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-252">Boolean</span></span>|<span data-ttu-id="bc42a-253">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-253">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-254">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="bc42a-254">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="bc42a-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-255">Boolean</span></span>|<span data-ttu-id="bc42a-256">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-256">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="bc42a-257">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-257">cellularBlockPlanModification</span></span>|<span data-ttu-id="bc42a-258">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-258">Boolean</span></span>|<span data-ttu-id="bc42a-259">Indica se os usuários podem ou não permitir que os usuários alterem as configurações do plano celular em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-259">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="bc42a-260">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="bc42a-260">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="bc42a-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-261">Boolean</span></span>|<span data-ttu-id="bc42a-262">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-262">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="bc42a-263">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="bc42a-263">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="bc42a-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-264">Boolean</span></span>|<span data-ttu-id="bc42a-265">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="bc42a-265">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="bc42a-266">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="bc42a-266">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="bc42a-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-267">Boolean</span></span>|<span data-ttu-id="bc42a-268">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-268">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="bc42a-269">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="bc42a-269">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="bc42a-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-270">Boolean</span></span>|<span data-ttu-id="bc42a-271">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-271">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-272">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="bc42a-272">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="bc42a-273">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-273">Boolean</span></span>|<span data-ttu-id="bc42a-274">Indica se o usuário deve ou não dar permissão automaticamente às solicitações do professor, sem solicitar ao aluno, quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-274">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-275">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="bc42a-275">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="bc42a-276">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-276">Boolean</span></span>|<span data-ttu-id="bc42a-277">Indica se o professor deve ou não permitir que o professor bloqueie aplicativos ou o dispositivo sem solicitar ao aluno.</span><span class="sxs-lookup"><span data-stu-id="bc42a-277">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="bc42a-278">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-278">Supervised only.</span></span>|
|<span data-ttu-id="bc42a-279">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="bc42a-279">compliantAppsList</span></span>|<span data-ttu-id="bc42a-280">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-280">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="bc42a-281">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="bc42a-281">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="bc42a-282">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="bc42a-282">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="bc42a-283">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="bc42a-283">compliantAppListType</span></span>|[<span data-ttu-id="bc42a-284">appListType</span><span class="sxs-lookup"><span data-stu-id="bc42a-284">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="bc42a-285">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="bc42a-285">List that is in the AppComplianceList.</span></span> <span data-ttu-id="bc42a-286">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="bc42a-286">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="bc42a-287">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="bc42a-287">configurationProfileBlockChanges</span></span>|<span data-ttu-id="bc42a-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-288">Boolean</span></span>|<span data-ttu-id="bc42a-289">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-289">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-290">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-290">definitionLookupBlocked</span></span>|<span data-ttu-id="bc42a-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-291">Boolean</span></span>|<span data-ttu-id="bc42a-292">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-292">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="bc42a-293">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="bc42a-293">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="bc42a-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-294">Boolean</span></span>|<span data-ttu-id="bc42a-295">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-295">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-296">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="bc42a-296">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="bc42a-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-297">Boolean</span></span>|<span data-ttu-id="bc42a-298">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-298">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-299">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-299">deviceBlockNameModification</span></span>|<span data-ttu-id="bc42a-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-300">Boolean</span></span>|<span data-ttu-id="bc42a-301">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-301">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="bc42a-302">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="bc42a-302">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="bc42a-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-303">Boolean</span></span>|<span data-ttu-id="bc42a-304">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-304">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="bc42a-305">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-305">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="bc42a-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-306">Boolean</span></span>|<span data-ttu-id="bc42a-307">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-307">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="bc42a-308">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="bc42a-308">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="bc42a-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-309">Boolean</span></span>|<span data-ttu-id="bc42a-310">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="bc42a-310">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="bc42a-311">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="bc42a-311">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="bc42a-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-312">Boolean</span></span>|<span data-ttu-id="bc42a-313">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="bc42a-313">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="bc42a-314">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="bc42a-314">emailInDomainSuffixes</span></span>|<span data-ttu-id="bc42a-315">String collection</span><span class="sxs-lookup"><span data-stu-id="bc42a-315">String collection</span></span>|<span data-ttu-id="bc42a-316">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="bc42a-316">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="bc42a-317">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="bc42a-317">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="bc42a-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-318">Boolean</span></span>|<span data-ttu-id="bc42a-319">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="bc42a-319">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="bc42a-320">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-320">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="bc42a-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-321">Boolean</span></span>|<span data-ttu-id="bc42a-322">\[Preterido Configurar essa configuração e definir o valor como \] "true" não tem efeito no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc42a-322">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="bc42a-323">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-323">esimBlockModification</span></span>|<span data-ttu-id="bc42a-324">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-324">Boolean</span></span>|<span data-ttu-id="bc42a-325">Indica se é ou não para permitir a adição ou remoção de planos celulares no eSIM de um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-325">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="bc42a-326">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-326">faceTimeBlocked</span></span>|<span data-ttu-id="bc42a-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-327">Boolean</span></span>|<span data-ttu-id="bc42a-328">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="bc42a-328">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="bc42a-329">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-329">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="bc42a-330">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-330">findMyFriendsBlocked</span></span>|<span data-ttu-id="bc42a-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-331">Boolean</span></span>|<span data-ttu-id="bc42a-332">Indica se deve ou não bloquear as alterações para Encontrar Meus Amigos quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-332">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-333">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="bc42a-333">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="bc42a-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-334">Boolean</span></span>|<span data-ttu-id="bc42a-335">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="bc42a-335">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="bc42a-336">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-336">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="bc42a-337">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="bc42a-337">gamingBlockMultiplayer</span></span>|<span data-ttu-id="bc42a-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-338">Boolean</span></span>|<span data-ttu-id="bc42a-339">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="bc42a-339">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="bc42a-340">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-340">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="bc42a-341">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-341">gameCenterBlocked</span></span>|<span data-ttu-id="bc42a-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-342">Boolean</span></span>|<span data-ttu-id="bc42a-343">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-343">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-344">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-344">hostPairingBlocked</span></span>|<span data-ttu-id="bc42a-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-345">Boolean</span></span>|<span data-ttu-id="bc42a-346">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-346">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-347">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-347">iBooksStoreBlocked</span></span>|<span data-ttu-id="bc42a-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-348">Boolean</span></span>|<span data-ttu-id="bc42a-349">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-349">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-350">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="bc42a-350">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="bc42a-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-351">Boolean</span></span>|<span data-ttu-id="bc42a-352">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="bc42a-352">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="bc42a-353">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="bc42a-353">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="bc42a-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-354">Boolean</span></span>|<span data-ttu-id="bc42a-355">Indica se o usuário deve ou não bloquear o trabalho contínuo iniciado no dispositivo iOS para outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="bc42a-355">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="bc42a-356">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="bc42a-356">iCloudBlockBackup</span></span>|<span data-ttu-id="bc42a-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-357">Boolean</span></span>|<span data-ttu-id="bc42a-358">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-358">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="bc42a-359">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-359">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="bc42a-360">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="bc42a-360">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="bc42a-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-361">Boolean</span></span>|<span data-ttu-id="bc42a-362">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueado. Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-362">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="bc42a-363">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="bc42a-363">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="bc42a-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-364">Boolean</span></span>|<span data-ttu-id="bc42a-365">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="bc42a-365">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="bc42a-366">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="bc42a-366">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="bc42a-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-367">Boolean</span></span>|<span data-ttu-id="bc42a-368">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="bc42a-368">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="bc42a-369">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="bc42a-369">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="bc42a-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-370">Boolean</span></span>|<span data-ttu-id="bc42a-371">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="bc42a-371">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="bc42a-372">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="bc42a-372">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="bc42a-373">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-373">Boolean</span></span>|<span data-ttu-id="bc42a-374">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="bc42a-374">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="bc42a-375">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="bc42a-375">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="bc42a-376">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-376">Boolean</span></span>|<span data-ttu-id="bc42a-377">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="bc42a-377">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="bc42a-378">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="bc42a-378">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="bc42a-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-379">Boolean</span></span>|<span data-ttu-id="bc42a-380">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="bc42a-380">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="bc42a-381">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-381">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="bc42a-382">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="bc42a-382">iTunesBlockMusicService</span></span>|<span data-ttu-id="bc42a-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-383">Boolean</span></span>|<span data-ttu-id="bc42a-384">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-384">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="bc42a-385">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="bc42a-385">iTunesBlockRadio</span></span>|<span data-ttu-id="bc42a-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-386">Boolean</span></span>|<span data-ttu-id="bc42a-387">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-387">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="bc42a-388">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="bc42a-388">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="bc42a-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-389">Boolean</span></span>|<span data-ttu-id="bc42a-390">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-390">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="bc42a-391">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="bc42a-391">keyboardBlockDictation</span></span>|<span data-ttu-id="bc42a-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-392">Boolean</span></span>|<span data-ttu-id="bc42a-393">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-393">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-394">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="bc42a-394">keyboardBlockPredictive</span></span>|<span data-ttu-id="bc42a-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-395">Boolean</span></span>|<span data-ttu-id="bc42a-396">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-396">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="bc42a-397">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="bc42a-397">keyboardBlockShortcuts</span></span>|<span data-ttu-id="bc42a-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-398">Boolean</span></span>|<span data-ttu-id="bc42a-399">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-399">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="bc42a-400">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="bc42a-400">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="bc42a-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-401">Boolean</span></span>|<span data-ttu-id="bc42a-402">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-402">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="bc42a-403">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="bc42a-403">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="bc42a-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-404">Boolean</span></span>|<span data-ttu-id="bc42a-405">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-405">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-406">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="bc42a-406">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="bc42a-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-407">Boolean</span></span>|<span data-ttu-id="bc42a-408">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-408">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-409">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="bc42a-409">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="bc42a-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-410">Boolean</span></span>|<span data-ttu-id="bc42a-411">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-411">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="bc42a-412">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="bc42a-412">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="bc42a-413">Em vez disso, use KioskModeBlockAutoLock.</span><span class="sxs-lookup"><span data-stu-id="bc42a-413">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="bc42a-414">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="bc42a-414">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="bc42a-415">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-415">Boolean</span></span>|<span data-ttu-id="bc42a-416">Indica se o bloqueio automático do dispositivo deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-416">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-417">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="bc42a-417">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="bc42a-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-418">Boolean</span></span>|<span data-ttu-id="bc42a-419">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-419">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-420">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="bc42a-420">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="bc42a-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-421">Boolean</span></span>|<span data-ttu-id="bc42a-422">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-422">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="bc42a-423">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="bc42a-423">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="bc42a-424">Use KioskModeBlockRingerSwitch.</span><span class="sxs-lookup"><span data-stu-id="bc42a-424">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="bc42a-425">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="bc42a-425">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="bc42a-426">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-426">Boolean</span></span>|<span data-ttu-id="bc42a-427">Indica se o uso do aneler deve ou não ser bloqueado enquanto estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-427">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-428">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="bc42a-428">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="bc42a-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-429">Boolean</span></span>|<span data-ttu-id="bc42a-430">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-430">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="bc42a-431">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="bc42a-431">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="bc42a-432">Use KioskModeBlockScreenRotation em vez disso.</span><span class="sxs-lookup"><span data-stu-id="bc42a-432">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="bc42a-433">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="bc42a-433">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="bc42a-434">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-434">Boolean</span></span>|<span data-ttu-id="bc42a-435">Indica se a rotação da tela deve ou não ser bloqueado enquanto estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-435">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-436">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="bc42a-436">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="bc42a-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-437">Boolean</span></span>|<span data-ttu-id="bc42a-438">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-438">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="bc42a-439">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="bc42a-439">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="bc42a-440">Use KioskModeBlockSleepButton em vez disso.</span><span class="sxs-lookup"><span data-stu-id="bc42a-440">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="bc42a-441">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="bc42a-441">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="bc42a-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-442">Boolean</span></span>|<span data-ttu-id="bc42a-443">Indica se o uso do botão de sono deve ou não ser bloqueado enquanto estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-443">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-444">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="bc42a-444">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="bc42a-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-445">Boolean</span></span>|<span data-ttu-id="bc42a-446">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-446">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="bc42a-447">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="bc42a-447">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="bc42a-448">Use KioskModeBlockTouchscreen em vez disso.</span><span class="sxs-lookup"><span data-stu-id="bc42a-448">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="bc42a-449">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="bc42a-449">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="bc42a-450">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-450">Boolean</span></span>|<span data-ttu-id="bc42a-451">Indica se o uso da tela sensível ao toque deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-451">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-452">kioskModeEnableVoiceControl</span><span class="sxs-lookup"><span data-stu-id="bc42a-452">kioskModeEnableVoiceControl</span></span>|<span data-ttu-id="bc42a-453">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-453">Boolean</span></span>|<span data-ttu-id="bc42a-454">Indica se o controle de voz deve ou não ser habilitado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-454">Indicates whether or not to enable voice control in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-455">kioskModeAllowVoiceControlModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-455">kioskModeAllowVoiceControlModification</span></span>|<span data-ttu-id="bc42a-456">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-456">Boolean</span></span>|<span data-ttu-id="bc42a-457">Indica se o usuário pode ou não alternar o controle de voz no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-457">Indicates whether or not to allow the user to toggle voice control in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-458">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="bc42a-458">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="bc42a-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-459">Boolean</span></span>|<span data-ttu-id="bc42a-460">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-460">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-461">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="bc42a-461">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="bc42a-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-462">Boolean</span></span>|<span data-ttu-id="bc42a-463">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-463">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="bc42a-464">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="bc42a-464">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="bc42a-465">Use KioskModeBlockVolumeButtons.</span><span class="sxs-lookup"><span data-stu-id="bc42a-465">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="bc42a-466">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="bc42a-466">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="bc42a-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-467">Boolean</span></span>|<span data-ttu-id="bc42a-468">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-468">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="bc42a-469">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="bc42a-469">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="bc42a-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-470">Boolean</span></span>|<span data-ttu-id="bc42a-471">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-471">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-472">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="bc42a-472">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="bc42a-473">String</span><span class="sxs-lookup"><span data-stu-id="bc42a-473">String</span></span>|<span data-ttu-id="bc42a-474">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-474">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="bc42a-475">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="bc42a-475">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="bc42a-476">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="bc42a-476">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="bc42a-477">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc42a-477">String</span></span>|<span data-ttu-id="bc42a-478">ID para aplicativos integrados a usar no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-478">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="bc42a-479">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não estão definidos.</span><span class="sxs-lookup"><span data-stu-id="bc42a-479">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="bc42a-480">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="bc42a-480">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="bc42a-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-481">Boolean</span></span>|<span data-ttu-id="bc42a-482">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-482">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-483">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="bc42a-483">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="bc42a-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-484">Boolean</span></span>|<span data-ttu-id="bc42a-485">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-485">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-486">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="bc42a-486">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="bc42a-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-487">Boolean</span></span>|<span data-ttu-id="bc42a-488">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-488">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-489">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="bc42a-489">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="bc42a-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-490">Boolean</span></span>|<span data-ttu-id="bc42a-491">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-491">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-492">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="bc42a-492">kioskModeRequireZoom</span></span>|<span data-ttu-id="bc42a-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-493">Boolean</span></span>|<span data-ttu-id="bc42a-494">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-494">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="bc42a-495">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="bc42a-495">kioskModeManagedAppId</span></span>|<span data-ttu-id="bc42a-496">String</span><span class="sxs-lookup"><span data-stu-id="bc42a-496">String</span></span>|<span data-ttu-id="bc42a-497">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-497">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="bc42a-498">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="bc42a-498">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="bc42a-499">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="bc42a-499">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="bc42a-500">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-500">Boolean</span></span>|<span data-ttu-id="bc42a-501">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="bc42a-501">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="bc42a-502">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="bc42a-502">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="bc42a-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-503">Boolean</span></span>|<span data-ttu-id="bc42a-504">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="bc42a-504">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="bc42a-505">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="bc42a-505">lockScreenBlockPassbook</span></span>|<span data-ttu-id="bc42a-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-506">Boolean</span></span>|<span data-ttu-id="bc42a-507">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="bc42a-507">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="bc42a-508">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="bc42a-508">lockScreenBlockTodayView</span></span>|<span data-ttu-id="bc42a-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-509">Boolean</span></span>|<span data-ttu-id="bc42a-510">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="bc42a-510">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="bc42a-511">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="bc42a-511">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="bc42a-512">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="bc42a-512">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="bc42a-513">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="bc42a-513">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="bc42a-514">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="bc42a-514">mediaContentRatingCanada</span></span>|[<span data-ttu-id="bc42a-515">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="bc42a-515">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="bc42a-516">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="bc42a-516">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="bc42a-517">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="bc42a-517">mediaContentRatingFrance</span></span>|[<span data-ttu-id="bc42a-518">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="bc42a-518">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="bc42a-519">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="bc42a-519">Media content rating settings for France</span></span>|
|<span data-ttu-id="bc42a-520">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="bc42a-520">mediaContentRatingGermany</span></span>|[<span data-ttu-id="bc42a-521">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="bc42a-521">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="bc42a-522">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="bc42a-522">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="bc42a-523">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="bc42a-523">mediaContentRatingIreland</span></span>|[<span data-ttu-id="bc42a-524">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="bc42a-524">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="bc42a-525">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="bc42a-525">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="bc42a-526">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="bc42a-526">mediaContentRatingJapan</span></span>|[<span data-ttu-id="bc42a-527">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="bc42a-527">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="bc42a-528">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="bc42a-528">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="bc42a-529">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="bc42a-529">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="bc42a-530">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="bc42a-530">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="bc42a-531">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="bc42a-531">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="bc42a-532">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="bc42a-532">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="bc42a-533">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="bc42a-533">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="bc42a-534">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="bc42a-534">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="bc42a-535">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="bc42a-535">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="bc42a-536">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="bc42a-536">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="bc42a-537">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="bc42a-537">Media content rating settings for United States</span></span>|
|<span data-ttu-id="bc42a-538">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="bc42a-538">networkUsageRules</span></span>|<span data-ttu-id="bc42a-539">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="bc42a-539">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="bc42a-540">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="bc42a-540">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="bc42a-541">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="bc42a-541">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="bc42a-542">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="bc42a-542">mediaContentRatingApps</span></span>|[<span data-ttu-id="bc42a-543">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="bc42a-543">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="bc42a-544">Configurações de classificação de conteúdo de mídia para Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="bc42a-544">Media content rating settings for Apps.</span></span> <span data-ttu-id="bc42a-545">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="bc42a-545">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="bc42a-546">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-546">messagesBlocked</span></span>|<span data-ttu-id="bc42a-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-547">Boolean</span></span>|<span data-ttu-id="bc42a-548">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-548">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="bc42a-549">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-549">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="bc42a-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-550">Boolean</span></span>|<span data-ttu-id="bc42a-551">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-551">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="bc42a-552">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="bc42a-552">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="bc42a-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-553">Boolean</span></span>|<span data-ttu-id="bc42a-554">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-554">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="bc42a-555">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-555">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="bc42a-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-556">Boolean</span></span>|<span data-ttu-id="bc42a-557">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-557">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-558">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-558">passcodeBlockModification</span></span>|<span data-ttu-id="bc42a-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-559">Boolean</span></span>|<span data-ttu-id="bc42a-560">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-560">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="bc42a-561">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="bc42a-561">passcodeBlockSimple</span></span>|<span data-ttu-id="bc42a-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-562">Boolean</span></span>|<span data-ttu-id="bc42a-563">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="bc42a-563">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="bc42a-564">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="bc42a-564">passcodeExpirationDays</span></span>|<span data-ttu-id="bc42a-565">Int32</span><span class="sxs-lookup"><span data-stu-id="bc42a-565">Int32</span></span>|<span data-ttu-id="bc42a-566">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="bc42a-566">Number of days before the passcode expires.</span></span> <span data-ttu-id="bc42a-567">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="bc42a-567">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="bc42a-568">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="bc42a-568">passcodeMinimumLength</span></span>|<span data-ttu-id="bc42a-569">Int32</span><span class="sxs-lookup"><span data-stu-id="bc42a-569">Int32</span></span>|<span data-ttu-id="bc42a-570">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="bc42a-570">Minimum length of passcode.</span></span> <span data-ttu-id="bc42a-571">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="bc42a-571">Valid values 4 to 14</span></span>|
|<span data-ttu-id="bc42a-572">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="bc42a-572">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="bc42a-573">Int32</span><span class="sxs-lookup"><span data-stu-id="bc42a-573">Int32</span></span>|<span data-ttu-id="bc42a-574">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="bc42a-574">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="bc42a-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="bc42a-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="bc42a-576">Int32</span><span class="sxs-lookup"><span data-stu-id="bc42a-576">Int32</span></span>|<span data-ttu-id="bc42a-577">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="bc42a-577">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="bc42a-578">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="bc42a-578">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="bc42a-579">Int32</span><span class="sxs-lookup"><span data-stu-id="bc42a-579">Int32</span></span>|<span data-ttu-id="bc42a-580">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="bc42a-580">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="bc42a-581">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="bc42a-581">Valid values 0 to 4</span></span>|
|<span data-ttu-id="bc42a-582">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="bc42a-582">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="bc42a-583">Int32</span><span class="sxs-lookup"><span data-stu-id="bc42a-583">Int32</span></span>|<span data-ttu-id="bc42a-584">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="bc42a-584">Number of previous passcodes to block.</span></span> <span data-ttu-id="bc42a-585">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="bc42a-585">Valid values 1 to 24</span></span>|
|<span data-ttu-id="bc42a-586">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="bc42a-586">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="bc42a-587">Int32</span><span class="sxs-lookup"><span data-stu-id="bc42a-587">Int32</span></span>|<span data-ttu-id="bc42a-588">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc42a-588">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="bc42a-589">Valores válidos de 2 a 11</span><span class="sxs-lookup"><span data-stu-id="bc42a-589">Valid values 2 to 11</span></span>|
|<span data-ttu-id="bc42a-590">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="bc42a-590">passcodeRequiredType</span></span>|[<span data-ttu-id="bc42a-591">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="bc42a-591">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="bc42a-592">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="bc42a-592">Type of passcode that is required.</span></span> <span data-ttu-id="bc42a-593">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="bc42a-593">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="bc42a-594">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="bc42a-594">passcodeRequired</span></span>|<span data-ttu-id="bc42a-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-595">Boolean</span></span>|<span data-ttu-id="bc42a-596">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="bc42a-596">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="bc42a-597">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-597">podcastsBlocked</span></span>|<span data-ttu-id="bc42a-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-598">Boolean</span></span>|<span data-ttu-id="bc42a-599">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-599">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="bc42a-600">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="bc42a-600">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="bc42a-601">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-601">Boolean</span></span>|<span data-ttu-id="bc42a-602">Indica se o prompt deve ou não habilitar a instalação de dispositivos próximos com um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-602">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="bc42a-603">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="bc42a-603">safariBlockAutofill</span></span>|<span data-ttu-id="bc42a-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-604">Boolean</span></span>|<span data-ttu-id="bc42a-605">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="bc42a-605">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="bc42a-606">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-606">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="bc42a-607">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="bc42a-607">safariBlockJavaScript</span></span>|<span data-ttu-id="bc42a-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-608">Boolean</span></span>|<span data-ttu-id="bc42a-609">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="bc42a-609">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="bc42a-610">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="bc42a-610">safariBlockPopups</span></span>|<span data-ttu-id="bc42a-611">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-611">Boolean</span></span>|<span data-ttu-id="bc42a-612">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="bc42a-612">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="bc42a-613">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-613">safariBlocked</span></span>|<span data-ttu-id="bc42a-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-614">Boolean</span></span>|<span data-ttu-id="bc42a-615">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="bc42a-615">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="bc42a-616">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-616">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="bc42a-617">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="bc42a-617">safariCookieSettings</span></span>|[<span data-ttu-id="bc42a-618">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="bc42a-618">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="bc42a-619">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="bc42a-619">Cookie settings for Safari.</span></span> <span data-ttu-id="bc42a-620">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="bc42a-620">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="bc42a-621">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="bc42a-621">safariManagedDomains</span></span>|<span data-ttu-id="bc42a-622">String collection</span><span class="sxs-lookup"><span data-stu-id="bc42a-622">String collection</span></span>|<span data-ttu-id="bc42a-623">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="bc42a-623">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="bc42a-624">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="bc42a-624">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="bc42a-625">String collection</span><span class="sxs-lookup"><span data-stu-id="bc42a-625">String collection</span></span>|<span data-ttu-id="bc42a-626">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="bc42a-626">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="bc42a-627">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-627">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="bc42a-628">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="bc42a-628">safariRequireFraudWarning</span></span>|<span data-ttu-id="bc42a-629">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-629">Boolean</span></span>|<span data-ttu-id="bc42a-630">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="bc42a-630">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="bc42a-631">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-631">screenCaptureBlocked</span></span>|<span data-ttu-id="bc42a-632">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-632">Boolean</span></span>|<span data-ttu-id="bc42a-633">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="bc42a-633">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="bc42a-634">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-634">siriBlocked</span></span>|<span data-ttu-id="bc42a-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-635">Boolean</span></span>|<span data-ttu-id="bc42a-636">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="bc42a-636">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="bc42a-637">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-637">siriBlockedWhenLocked</span></span>|<span data-ttu-id="bc42a-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-638">Boolean</span></span>|<span data-ttu-id="bc42a-639">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-639">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="bc42a-640">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="bc42a-640">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="bc42a-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-641">Boolean</span></span>|<span data-ttu-id="bc42a-642">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-642">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="bc42a-643">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="bc42a-643">siriRequireProfanityFilter</span></span>|<span data-ttu-id="bc42a-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-644">Boolean</span></span>|<span data-ttu-id="bc42a-645">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-645">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="bc42a-646">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="bc42a-646">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="bc42a-647">Int32</span><span class="sxs-lookup"><span data-stu-id="bc42a-647">Int32</span></span>|<span data-ttu-id="bc42a-648">Define quantos dias uma atualização de software será usada para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-648">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="bc42a-649">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="bc42a-649">Valid values 0 to 90</span></span>|
|<span data-ttu-id="bc42a-650">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="bc42a-650">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="bc42a-651">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-651">Boolean</span></span>|<span data-ttu-id="bc42a-652">Indica se o usuário deve ou não atrasar a visibilidade das atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-652">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-653">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="bc42a-653">spotlightBlockInternetResults</span></span>|<span data-ttu-id="bc42a-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-654">Boolean</span></span>|<span data-ttu-id="bc42a-655">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-655">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="bc42a-656">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-656">voiceDialingBlocked</span></span>|<span data-ttu-id="bc42a-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-657">Boolean</span></span>|<span data-ttu-id="bc42a-658">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="bc42a-658">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="bc42a-659">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-659">wallpaperBlockModification</span></span>|<span data-ttu-id="bc42a-660">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-660">Boolean</span></span>|<span data-ttu-id="bc42a-661">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-661">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="bc42a-662">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="bc42a-662">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="bc42a-663">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc42a-663">Boolean</span></span>|<span data-ttu-id="bc42a-664">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-664">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="bc42a-665">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="bc42a-665">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="bc42a-666">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-666">Boolean</span></span>|<span data-ttu-id="bc42a-667">Indica se um aluno matriculado em um curso não controlado via Classroom solicitará permissão do professor ao tentar sair do curso (iOS 11.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-667">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="bc42a-668">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="bc42a-668">keychainBlockCloudSync</span></span>|<span data-ttu-id="bc42a-669">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-669">Boolean</span></span>|<span data-ttu-id="bc42a-670">Indica se a sincronização do chaveiro do iCloud está bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="bc42a-670">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="bc42a-671">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-671">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="bc42a-672">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="bc42a-672">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="bc42a-673">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-673">Boolean</span></span>|<span data-ttu-id="bc42a-674">Indica se as atualizações PKI sobre o ar estão ou não bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="bc42a-674">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="bc42a-675">Definir essa restrição como false não desabilita as verificações de CRL e OCSP (iOS 7.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-675">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="bc42a-676">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="bc42a-676">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="bc42a-677">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-677">Boolean</span></span>|<span data-ttu-id="bc42a-678">Indica se o controle de ad é limitado. (iOS 7.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-678">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="bc42a-679">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="bc42a-679">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="bc42a-680">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-680">Boolean</span></span>|<span data-ttu-id="bc42a-681">Indica se o back-up do livro enterprise está bloqueado ou não.</span><span class="sxs-lookup"><span data-stu-id="bc42a-681">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="bc42a-682">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="bc42a-682">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="bc42a-683">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-683">Boolean</span></span>|<span data-ttu-id="bc42a-684">Indica se a sincronização de anotações e realçamentos do livro enterprise ou não está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="bc42a-684">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="bc42a-685">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-685">airPrintBlocked</span></span>|<span data-ttu-id="bc42a-686">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-686">Boolean</span></span>|<span data-ttu-id="bc42a-687">Indica se o AirPrint está ou não bloqueado (iOS 11.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-687">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="bc42a-688">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="bc42a-688">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="bc42a-689">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-689">Boolean</span></span>|<span data-ttu-id="bc42a-690">Indica se o armazenamento de chaves de nome de usuário e senha para Airprint está bloqueado (iOS 11.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-690">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="bc42a-691">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="bc42a-691">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="bc42a-692">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-692">Boolean</span></span>|<span data-ttu-id="bc42a-693">Indica se certificados confiáveis são necessários para comunicação de impressão TLS (iOS 11.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-693">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="bc42a-694">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="bc42a-694">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="bc42a-695">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-695">Boolean</span></span>|<span data-ttu-id="bc42a-696">Indica se a descoberta iBeacon ou não de impressoras AirPrint está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="bc42a-696">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="bc42a-697">Isso impede que o AirPrint Bluetooth sinalizadores contra phishing para tráfego de rede (iOS 11.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-697">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="bc42a-698">filesNetworkDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-698">filesNetworkDriveAccessBlocked</span></span>|<span data-ttu-id="bc42a-699">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-699">Boolean</span></span>|<span data-ttu-id="bc42a-700">Indica se os dispositivos podem acessar arquivos ou outros recursos em um servidor de rede usando o protocolo SMB (Server Message Block).</span><span class="sxs-lookup"><span data-stu-id="bc42a-700">Indicates if devices can access files or other resources on a network server using the Server Message Block (SMB) protocol.</span></span> <span data-ttu-id="bc42a-701">Disponível para dispositivos que executam iOS e iPadOS, versões 13.0 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="bc42a-701">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="bc42a-702">filesUsbDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-702">filesUsbDriveAccessBlocked</span></span>|<span data-ttu-id="bc42a-703">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-703">Boolean</span></span>|<span data-ttu-id="bc42a-704">Indica se os sevices com acesso podem se conectar e abrir arquivos em uma unidade USB.</span><span class="sxs-lookup"><span data-stu-id="bc42a-704">Indicates if sevices with access can connect to and open files on a USB drive.</span></span> <span data-ttu-id="bc42a-705">Disponível para dispositivos que executam iOS e iPadOS, versões 13.0 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="bc42a-705">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="bc42a-706">wifiPowerOnForced</span><span class="sxs-lookup"><span data-stu-id="bc42a-706">wifiPowerOnForced</span></span>|<span data-ttu-id="bc42a-707">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-707">Boolean</span></span>|<span data-ttu-id="bc42a-708">Indica se o Wi-Fi permanece ou não, mesmo quando o dispositivo está no modo de avião.</span><span class="sxs-lookup"><span data-stu-id="bc42a-708">Indicates whether or not Wi-Fi remains on, even when device is in airplane mode.</span></span> <span data-ttu-id="bc42a-709">Disponível para dispositivos que executam iOS e iPadOS, versões 13.0 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="bc42a-709">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="bc42a-710">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="bc42a-710">blockSystemAppRemoval</span></span>|<span data-ttu-id="bc42a-711">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-711">Boolean</span></span>|<span data-ttu-id="bc42a-712">Indica se a remoção ou não de aplicativos do sistema do dispositivo está bloqueada em um dispositivo supervisionado (iOS 11.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-712">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="bc42a-713">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="bc42a-713">vpnBlockCreation</span></span>|<span data-ttu-id="bc42a-714">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-714">Boolean</span></span>|<span data-ttu-id="bc42a-715">Indica se a criação de configurações VPN está ou não bloqueada (iOS 11.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-715">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="bc42a-716">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-716">appRemovalBlocked</span></span>|<span data-ttu-id="bc42a-717">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-717">Boolean</span></span>|<span data-ttu-id="bc42a-718">Indica se a remoção de aplicativos é permitida.</span><span class="sxs-lookup"><span data-stu-id="bc42a-718">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="bc42a-719">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-719">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="bc42a-720">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-720">Boolean</span></span>|<span data-ttu-id="bc42a-721">Indica se a conexão com acessórios USB enquanto o dispositivo está bloqueado é permitida (iOS 11.4.1 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-721">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="bc42a-722">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="bc42a-722">passwordBlockAutoFill</span></span>|<span data-ttu-id="bc42a-723">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-723">Boolean</span></span>|<span data-ttu-id="bc42a-724">Indica se o recurso Senhas de Preenchimento Automático é permitido (iOS 12.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-724">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="bc42a-725">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="bc42a-725">passwordBlockProximityRequests</span></span>|<span data-ttu-id="bc42a-726">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-726">Boolean</span></span>|<span data-ttu-id="bc42a-727">Indica se deve ou não bloquear a solicitação de senhas de dispositivos próximos (iOS 12.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-727">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="bc42a-728">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="bc42a-728">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="bc42a-729">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-729">Boolean</span></span>|<span data-ttu-id="bc42a-730">Indica se deve ou não bloquear o compartilhamento de senhas com o recurso de senhas do AirDrop iOS 12.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-730">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="bc42a-731">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="bc42a-731">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="bc42a-732">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-732">Boolean</span></span>|<span data-ttu-id="bc42a-733">Indica se o recurso Data e Hora "Definir Automaticamente" está habilitado e não pode ser desligado pelo usuário (iOS 12.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-733">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="bc42a-734">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="bc42a-734">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="bc42a-735">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-735">Boolean</span></span>|<span data-ttu-id="bc42a-736">Indica se os aplicativos gerenciados podem ou não gravar contatos em contas de contatos não gerenciadas (iOS 12.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="bc42a-736">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="bc42a-737">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="bc42a-737">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="bc42a-738">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-738">Boolean</span></span>|<span data-ttu-id="bc42a-739">Indica se aplicativos não gerenciados podem ou não ler de contas de contatos gerenciados (iOS 12.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-739">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="bc42a-740">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="bc42a-740">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="bc42a-741">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-741">Boolean</span></span>|<span data-ttu-id="bc42a-742">Indica se o usuário deve ou não bloquear a modificação da configuração de hotspot pessoal (iOS 12.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-742">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="bc42a-743">continuousPathKeyboardBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-743">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="bc42a-744">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-744">Boolean</span></span>|<span data-ttu-id="bc42a-745">Indica se o teclado de caminho contínuo deve ou não ser bloqueado quando o dispositivo é supervisionado (iOS 13 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-745">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="bc42a-746">findMyDeviceInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-746">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="bc42a-747">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-747">Boolean</span></span>|<span data-ttu-id="bc42a-748">Indica se o dispositivo deve ou não ser bloqueado quando o dispositivo é supervisionado (iOS 13 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-748">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="bc42a-749">findMyFriendsInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-749">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="bc42a-750">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-750">Boolean</span></span>|<span data-ttu-id="bc42a-751">Indica se deve ou não bloquear Find My Friends quando o dispositivo é supervisionado (iOS 13 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="bc42a-751">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="bc42a-752">iTunesBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-752">iTunesBlocked</span></span>|<span data-ttu-id="bc42a-753">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-753">Boolean</span></span>|<span data-ttu-id="bc42a-754">Indica se o aplicativo iTunes deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="bc42a-754">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="bc42a-755">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-755">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="bc42a-756">sharedDeviceBlockTemporarySessions</span><span class="sxs-lookup"><span data-stu-id="bc42a-756">sharedDeviceBlockTemporarySessions</span></span>|<span data-ttu-id="bc42a-757">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-757">Boolean</span></span>|<span data-ttu-id="bc42a-758">Indica se as sessões temporárias de iPads compartilhados (iOS 13.4 ou posteriores) são ou não bloqueados.</span><span class="sxs-lookup"><span data-stu-id="bc42a-758">Indicates whether or not to block temporary sessions on Shared iPads (iOS 13.4 or later).</span></span>|
|<span data-ttu-id="bc42a-759">appClipsBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-759">appClipsBlocked</span></span>|<span data-ttu-id="bc42a-760">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-760">Boolean</span></span>|<span data-ttu-id="bc42a-761">Impede que um usuário adicione clipes de aplicativo e remova todos os Clipes de Aplicativo existentes no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bc42a-761">Prevents a user from adding any App Clips and removes any existing App Clips on the device.</span></span>|
|<span data-ttu-id="bc42a-762">applePersonalizedAdsBlocked</span><span class="sxs-lookup"><span data-stu-id="bc42a-762">applePersonalizedAdsBlocked</span></span>|<span data-ttu-id="bc42a-763">Booleano</span><span class="sxs-lookup"><span data-stu-id="bc42a-763">Boolean</span></span>|<span data-ttu-id="bc42a-764">Limita a publicidade personalizada da Apple quando true.</span><span class="sxs-lookup"><span data-stu-id="bc42a-764">Limits Apple personalized advertising when true.</span></span> <span data-ttu-id="bc42a-765">Disponível no iOS 14 e posterior.</span><span class="sxs-lookup"><span data-stu-id="bc42a-765">Available in iOS 14 and later.</span></span>|
|<span data-ttu-id="bc42a-766">kioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="bc42a-766">kioskModeAppType</span></span>|[<span data-ttu-id="bc42a-767">iosKioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="bc42a-767">iosKioskModeAppType</span></span>](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|<span data-ttu-id="bc42a-768">Tipo de aplicativo a ser executado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="bc42a-768">Type of app to run in kiosk mode.</span></span> <span data-ttu-id="bc42a-769">Os valores possíveis são: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span><span class="sxs-lookup"><span data-stu-id="bc42a-769">Possible values are: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span></span>|



## <a name="response"></a><span data-ttu-id="bc42a-770">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc42a-770">Response</span></span>
<span data-ttu-id="bc42a-771">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc42a-771">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc42a-772">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc42a-772">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc42a-773">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc42a-773">Request</span></span>
<span data-ttu-id="bc42a-774">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc42a-774">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10633

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
  "sharedDeviceBlockTemporarySessions": true,
  "appClipsBlocked": true,
  "applePersonalizedAdsBlocked": true,
  "kioskModeAppType": "appStoreApp"
}
```

### <a name="response"></a><span data-ttu-id="bc42a-775">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc42a-775">Response</span></span>
<span data-ttu-id="bc42a-p158">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bc42a-p158">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10805

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
  "sharedDeviceBlockTemporarySessions": true,
  "appClipsBlocked": true,
  "applePersonalizedAdsBlocked": true,
  "kioskModeAppType": "appStoreApp"
}
```




