---
title: Criar iosGeneralDeviceConfiguration
description: Cria um novo objeto iosGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ffd7c496bd385a783cb96b63ddcfa4beeb97258
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948233"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="1c092-103">Criar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c092-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="1c092-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c092-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c092-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c092-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c092-106">Cria um novo objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1c092-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c092-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1c092-107">Prerequisites</span></span>
<span data-ttu-id="1c092-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c092-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c092-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c092-110">Permission type</span></span>|<span data-ttu-id="1c092-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1c092-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c092-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c092-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c092-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c092-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1c092-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1c092-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c092-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c092-115">Not supported.</span></span>|
|<span data-ttu-id="1c092-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c092-116">Application</span></span>|<span data-ttu-id="1c092-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c092-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c092-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c092-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1c092-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c092-119">Request headers</span></span>
|<span data-ttu-id="1c092-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c092-120">Header</span></span>|<span data-ttu-id="1c092-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1c092-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c092-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c092-122">Authorization</span></span>|<span data-ttu-id="1c092-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c092-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c092-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1c092-124">Accept</span></span>|<span data-ttu-id="1c092-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c092-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c092-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c092-126">Request body</span></span>
<span data-ttu-id="1c092-127">No corpo da solicitação, forneça uma representação JSON do objeto iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1c092-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="1c092-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1c092-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="1c092-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c092-129">Property</span></span>|<span data-ttu-id="1c092-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c092-130">Type</span></span>|<span data-ttu-id="1c092-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c092-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c092-132">id</span><span class="sxs-lookup"><span data-stu-id="1c092-132">id</span></span>|<span data-ttu-id="1c092-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c092-133">String</span></span>|<span data-ttu-id="1c092-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1c092-134">Key of the entity.</span></span> <span data-ttu-id="1c092-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c092-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c092-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1c092-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c092-137">DateTimeOffset</span></span>|<span data-ttu-id="1c092-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1c092-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1c092-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c092-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1c092-140">roleScopeTagIds</span></span>|<span data-ttu-id="1c092-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c092-141">String collection</span></span>|<span data-ttu-id="1c092-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="1c092-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1c092-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c092-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1c092-144">supportsScopeTags</span></span>|<span data-ttu-id="1c092-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-145">Boolean</span></span>|<span data-ttu-id="1c092-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1c092-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1c092-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1c092-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1c092-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="1c092-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1c092-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1c092-149">This property is read-only.</span></span> <span data-ttu-id="1c092-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c092-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1c092-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1c092-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1c092-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1c092-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="1c092-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1c092-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c092-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1c092-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1c092-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1c092-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1c092-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="1c092-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1c092-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c092-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1c092-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1c092-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1c092-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1c092-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="1c092-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1c092-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c092-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1c092-163">createdDateTime</span></span>|<span data-ttu-id="1c092-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c092-164">DateTimeOffset</span></span>|<span data-ttu-id="1c092-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1c092-165">DateTime the object was created.</span></span> <span data-ttu-id="1c092-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c092-167">descrição</span><span class="sxs-lookup"><span data-stu-id="1c092-167">description</span></span>|<span data-ttu-id="1c092-168">String</span><span class="sxs-lookup"><span data-stu-id="1c092-168">String</span></span>|<span data-ttu-id="1c092-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1c092-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1c092-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c092-171">displayName</span><span class="sxs-lookup"><span data-stu-id="1c092-171">displayName</span></span>|<span data-ttu-id="1c092-172">String</span><span class="sxs-lookup"><span data-stu-id="1c092-172">String</span></span>|<span data-ttu-id="1c092-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1c092-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1c092-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c092-175">versão</span><span class="sxs-lookup"><span data-stu-id="1c092-175">version</span></span>|<span data-ttu-id="1c092-176">Int32</span><span class="sxs-lookup"><span data-stu-id="1c092-176">Int32</span></span>|<span data-ttu-id="1c092-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1c092-177">Version of the device configuration.</span></span> <span data-ttu-id="1c092-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1c092-179">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="1c092-179">accountBlockModification</span></span>|<span data-ttu-id="1c092-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-180">Boolean</span></span>|<span data-ttu-id="1c092-181">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-181">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-182">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="1c092-182">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="1c092-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-183">Boolean</span></span>|<span data-ttu-id="1c092-184">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-184">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="1c092-185">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-185">airDropBlocked</span></span>|<span data-ttu-id="1c092-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-186">Boolean</span></span>|<span data-ttu-id="1c092-187">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-187">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-188">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="1c092-188">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="1c092-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-189">Boolean</span></span>|<span data-ttu-id="1c092-190">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-190">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1c092-191">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="1c092-191">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="1c092-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-192">Boolean</span></span>|<span data-ttu-id="1c092-193">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="1c092-193">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="1c092-194">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="1c092-194">appleWatchBlockPairing</span></span>|<span data-ttu-id="1c092-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-195">Boolean</span></span>|<span data-ttu-id="1c092-196">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-196">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1c092-197">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="1c092-197">appleWatchForceWristDetection</span></span>|<span data-ttu-id="1c092-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-198">Boolean</span></span>|<span data-ttu-id="1c092-199">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-199">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="1c092-200">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-200">appleNewsBlocked</span></span>|<span data-ttu-id="1c092-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-201">Boolean</span></span>|<span data-ttu-id="1c092-202">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-202">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1c092-203">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="1c092-203">appsSingleAppModeList</span></span>|<span data-ttu-id="1c092-204">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1c092-205">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="1c092-205">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="1c092-206">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-206">Supervised only.</span></span> <span data-ttu-id="1c092-207">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="1c092-207">iOS 7.0 and later.</span></span> <span data-ttu-id="1c092-208">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="1c092-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1c092-209">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="1c092-209">appsVisibilityList</span></span>|<span data-ttu-id="1c092-210">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1c092-211">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-211">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="1c092-212">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="1c092-212">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="1c092-213">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="1c092-213">appsVisibilityListType</span></span>|[<span data-ttu-id="1c092-214">appListType</span><span class="sxs-lookup"><span data-stu-id="1c092-214">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="1c092-215">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="1c092-215">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="1c092-216">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="1c092-216">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="1c092-217">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="1c092-217">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="1c092-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-218">Boolean</span></span>|<span data-ttu-id="1c092-219">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-219">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1c092-220">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-220">appStoreBlocked</span></span>|<span data-ttu-id="1c092-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-221">Boolean</span></span>|<span data-ttu-id="1c092-222">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="1c092-222">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="1c092-223">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="1c092-223">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="1c092-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c092-224">Boolean</span></span>|<span data-ttu-id="1c092-225">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1c092-225">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="1c092-226">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1c092-226">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="1c092-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-227">Boolean</span></span>|<span data-ttu-id="1c092-228">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="1c092-228">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="1c092-229">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-229">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1c092-230">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="1c092-230">appStoreRequirePassword</span></span>|<span data-ttu-id="1c092-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-231">Boolean</span></span>|<span data-ttu-id="1c092-232">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="1c092-232">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="1c092-233">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="1c092-233">autoFillForceAuthentication</span></span>|<span data-ttu-id="1c092-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-234">Boolean</span></span>|<span data-ttu-id="1c092-235">Indica se a autenticação do usuário deve ou não ser forçada antes de preencher automaticamente as informações de cartão de crédito e o Safari e outros aplicativos em dispositivos supervisionados.</span><span class="sxs-lookup"><span data-stu-id="1c092-235">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="1c092-236">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="1c092-236">bluetoothBlockModification</span></span>|<span data-ttu-id="1c092-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-237">Boolean</span></span>|<span data-ttu-id="1c092-238">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-238">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="1c092-239">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-239">cameraBlocked</span></span>|<span data-ttu-id="1c092-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-240">Boolean</span></span>|<span data-ttu-id="1c092-241">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1c092-241">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="1c092-242">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="1c092-242">cellularBlockDataRoaming</span></span>|<span data-ttu-id="1c092-243">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-243">Boolean</span></span>|<span data-ttu-id="1c092-244">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1c092-244">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="1c092-245">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="1c092-245">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="1c092-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-246">Boolean</span></span>|<span data-ttu-id="1c092-247">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="1c092-247">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="1c092-248">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="1c092-248">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="1c092-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-249">Boolean</span></span>|<span data-ttu-id="1c092-250">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-250">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-251">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="1c092-251">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="1c092-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-252">Boolean</span></span>|<span data-ttu-id="1c092-253">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1c092-253">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="1c092-254">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="1c092-254">cellularBlockPlanModification</span></span>|<span data-ttu-id="1c092-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-255">Boolean</span></span>|<span data-ttu-id="1c092-256">Indica se os usuários poderão ou não alterar as configurações do plano de celular em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-256">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="1c092-257">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="1c092-257">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="1c092-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-258">Boolean</span></span>|<span data-ttu-id="1c092-259">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1c092-259">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="1c092-260">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="1c092-260">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="1c092-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-261">Boolean</span></span>|<span data-ttu-id="1c092-262">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="1c092-262">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="1c092-263">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="1c092-263">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="1c092-264">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-264">Boolean</span></span>|<span data-ttu-id="1c092-265">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-265">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="1c092-266">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="1c092-266">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="1c092-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-267">Boolean</span></span>|<span data-ttu-id="1c092-268">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-268">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-269">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="1c092-269">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="1c092-270">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-270">Boolean</span></span>|<span data-ttu-id="1c092-271">Indica se a permissão será ou não automaticamente atribuído às solicitações do professor, sem avisar o aluno, quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-271">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-272">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="1c092-272">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="1c092-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-273">Boolean</span></span>|<span data-ttu-id="1c092-274">Indica se o professor deve ou não bloquear aplicativos ou o dispositivo sem avisar o aluno.</span><span class="sxs-lookup"><span data-stu-id="1c092-274">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="1c092-275">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-275">Supervised only.</span></span>|
|<span data-ttu-id="1c092-276">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="1c092-276">compliantAppsList</span></span>|<span data-ttu-id="1c092-277">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-277">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1c092-278">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="1c092-278">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="1c092-279">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="1c092-279">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="1c092-280">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="1c092-280">compliantAppListType</span></span>|[<span data-ttu-id="1c092-281">appListType</span><span class="sxs-lookup"><span data-stu-id="1c092-281">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="1c092-282">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="1c092-282">List that is in the AppComplianceList.</span></span> <span data-ttu-id="1c092-283">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="1c092-283">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="1c092-284">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="1c092-284">configurationProfileBlockChanges</span></span>|<span data-ttu-id="1c092-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-285">Boolean</span></span>|<span data-ttu-id="1c092-286">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-286">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-287">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-287">definitionLookupBlocked</span></span>|<span data-ttu-id="1c092-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-288">Boolean</span></span>|<span data-ttu-id="1c092-289">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-289">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="1c092-290">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="1c092-290">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="1c092-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-291">Boolean</span></span>|<span data-ttu-id="1c092-292">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-292">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-293">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="1c092-293">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="1c092-294">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-294">Boolean</span></span>|<span data-ttu-id="1c092-295">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-295">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-296">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="1c092-296">deviceBlockNameModification</span></span>|<span data-ttu-id="1c092-297">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-297">Boolean</span></span>|<span data-ttu-id="1c092-298">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-298">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1c092-299">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="1c092-299">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="1c092-300">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-300">Boolean</span></span>|<span data-ttu-id="1c092-301">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1c092-301">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="1c092-302">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="1c092-302">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="1c092-303">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-303">Boolean</span></span>|<span data-ttu-id="1c092-304">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-304">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="1c092-305">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="1c092-305">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="1c092-306">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-306">Boolean</span></span>|<span data-ttu-id="1c092-307">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="1c092-307">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="1c092-308">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="1c092-308">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="1c092-309">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-309">Boolean</span></span>|<span data-ttu-id="1c092-310">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="1c092-310">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="1c092-311">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="1c092-311">emailInDomainSuffixes</span></span>|<span data-ttu-id="1c092-312">String collection</span><span class="sxs-lookup"><span data-stu-id="1c092-312">String collection</span></span>|<span data-ttu-id="1c092-313">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="1c092-313">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="1c092-314">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="1c092-314">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="1c092-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-315">Boolean</span></span>|<span data-ttu-id="1c092-316">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="1c092-316">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="1c092-317">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="1c092-317">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="1c092-318">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-318">Boolean</span></span>|<span data-ttu-id="1c092-319">Indica se o usuário será ou não impedido de modificar as configurações de confiança de um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="1c092-319">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="1c092-320">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="1c092-320">esimBlockModification</span></span>|<span data-ttu-id="1c092-321">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-321">Boolean</span></span>|<span data-ttu-id="1c092-322">Indica se a adição ou a remoção de planos da rede celular deve ou não ser permitida no eSIM de um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-322">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="1c092-323">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-323">faceTimeBlocked</span></span>|<span data-ttu-id="1c092-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c092-324">Boolean</span></span>|<span data-ttu-id="1c092-325">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="1c092-325">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="1c092-326">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-326">findMyFriendsBlocked</span></span>|<span data-ttu-id="1c092-327">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-327">Boolean</span></span>|<span data-ttu-id="1c092-328">Indica se Encontrar Meus Amigos será bloqueado ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-328">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-329">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="1c092-329">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="1c092-330">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-330">Boolean</span></span>|<span data-ttu-id="1c092-331">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="1c092-331">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="1c092-332">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="1c092-332">gamingBlockMultiplayer</span></span>|<span data-ttu-id="1c092-333">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-333">Boolean</span></span>|<span data-ttu-id="1c092-334">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="1c092-334">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="1c092-335">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-335">gameCenterBlocked</span></span>|<span data-ttu-id="1c092-336">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-336">Boolean</span></span>|<span data-ttu-id="1c092-337">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-337">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-338">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-338">hostPairingBlocked</span></span>|<span data-ttu-id="1c092-339">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-339">Boolean</span></span>|<span data-ttu-id="1c092-340">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-340">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-341">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-341">iBooksStoreBlocked</span></span>|<span data-ttu-id="1c092-342">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-342">Boolean</span></span>|<span data-ttu-id="1c092-343">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-343">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-344">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="1c092-344">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="1c092-345">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-345">Boolean</span></span>|<span data-ttu-id="1c092-346">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="1c092-346">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="1c092-347">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="1c092-347">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="1c092-348">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-348">Boolean</span></span>|<span data-ttu-id="1c092-349">Indica se o usuário será ou não impedido de continuar o trabalho que começou no dispositivo iOS em outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="1c092-349">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="1c092-350">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="1c092-350">iCloudBlockBackup</span></span>|<span data-ttu-id="1c092-351">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-351">Boolean</span></span>|<span data-ttu-id="1c092-352">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1c092-352">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="1c092-353">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="1c092-353">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="1c092-354">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-354">Boolean</span></span>|<span data-ttu-id="1c092-355">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1c092-355">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="1c092-356">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="1c092-356">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="1c092-357">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-357">Boolean</span></span>|<span data-ttu-id="1c092-358">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1c092-358">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="1c092-359">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="1c092-359">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="1c092-360">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-360">Boolean</span></span>|<span data-ttu-id="1c092-361">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1c092-361">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="1c092-362">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="1c092-362">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="1c092-363">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-363">Boolean</span></span>|<span data-ttu-id="1c092-364">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1c092-364">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="1c092-365">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="1c092-365">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="1c092-366">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-366">Boolean</span></span>|<span data-ttu-id="1c092-367">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1c092-367">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="1c092-368">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="1c092-368">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="1c092-369">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-369">Boolean</span></span>|<span data-ttu-id="1c092-370">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="1c092-370">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="1c092-371">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="1c092-371">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="1c092-372">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-372">Boolean</span></span>|<span data-ttu-id="1c092-373">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="1c092-373">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="1c092-374">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="1c092-374">iTunesBlockMusicService</span></span>|<span data-ttu-id="1c092-375">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-375">Boolean</span></span>|<span data-ttu-id="1c092-376">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-376">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="1c092-377">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="1c092-377">iTunesBlockRadio</span></span>|<span data-ttu-id="1c092-378">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-378">Boolean</span></span>|<span data-ttu-id="1c092-379">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-379">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="1c092-380">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="1c092-380">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="1c092-381">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-381">Boolean</span></span>|<span data-ttu-id="1c092-382">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-382">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="1c092-383">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="1c092-383">keyboardBlockDictation</span></span>|<span data-ttu-id="1c092-384">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-384">Boolean</span></span>|<span data-ttu-id="1c092-385">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-385">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-386">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="1c092-386">keyboardBlockPredictive</span></span>|<span data-ttu-id="1c092-387">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-387">Boolean</span></span>|<span data-ttu-id="1c092-388">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-388">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="1c092-389">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="1c092-389">keyboardBlockShortcuts</span></span>|<span data-ttu-id="1c092-390">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-390">Boolean</span></span>|<span data-ttu-id="1c092-391">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-391">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1c092-392">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="1c092-392">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="1c092-393">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-393">Boolean</span></span>|<span data-ttu-id="1c092-394">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-394">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="1c092-395">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="1c092-395">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="1c092-396">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-396">Boolean</span></span>|<span data-ttu-id="1c092-397">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-397">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-398">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="1c092-398">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="1c092-399">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-399">Boolean</span></span>|<span data-ttu-id="1c092-400">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-400">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-401">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="1c092-401">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="1c092-402">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-402">Boolean</span></span>|<span data-ttu-id="1c092-403">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-403">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="1c092-404">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="1c092-404">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="1c092-405">Use KioskModeBlockAutoLock em vez disso.</span><span class="sxs-lookup"><span data-stu-id="1c092-405">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="1c092-406">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="1c092-406">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="1c092-407">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-407">Boolean</span></span>|<span data-ttu-id="1c092-408">Indica se o bloqueio automático do dispositivo deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-408">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-409">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="1c092-409">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="1c092-410">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-410">Boolean</span></span>|<span data-ttu-id="1c092-411">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-411">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-412">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="1c092-412">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="1c092-413">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-413">Boolean</span></span>|<span data-ttu-id="1c092-414">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-414">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="1c092-415">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="1c092-415">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="1c092-416">Use KioskModeBlockRingerSwitch em vez disso.</span><span class="sxs-lookup"><span data-stu-id="1c092-416">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="1c092-417">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="1c092-417">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="1c092-418">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-418">Boolean</span></span>|<span data-ttu-id="1c092-419">Indica se o uso do comutador de toque deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-419">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-420">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="1c092-420">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="1c092-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c092-421">Boolean</span></span>|<span data-ttu-id="1c092-422">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-422">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="1c092-423">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="1c092-423">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="1c092-424">Use KioskModeBlockScreenRotation em vez disso.</span><span class="sxs-lookup"><span data-stu-id="1c092-424">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="1c092-425">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="1c092-425">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="1c092-426">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-426">Boolean</span></span>|<span data-ttu-id="1c092-427">Indica se a rotação de tela deve ou não ser bloqueada enquanto estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-427">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-428">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="1c092-428">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="1c092-429">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-429">Boolean</span></span>|<span data-ttu-id="1c092-430">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-430">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="1c092-431">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="1c092-431">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="1c092-432">Use KioskModeBlockSleepButton em vez disso.</span><span class="sxs-lookup"><span data-stu-id="1c092-432">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="1c092-433">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="1c092-433">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="1c092-434">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-434">Boolean</span></span>|<span data-ttu-id="1c092-435">Indica se o uso do botão de suspensão deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-435">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-436">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="1c092-436">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="1c092-437">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-437">Boolean</span></span>|<span data-ttu-id="1c092-438">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-438">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="1c092-439">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="1c092-439">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="1c092-440">Use KioskModeBlockTouchscreen em vez disso.</span><span class="sxs-lookup"><span data-stu-id="1c092-440">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="1c092-441">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="1c092-441">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="1c092-442">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-442">Boolean</span></span>|<span data-ttu-id="1c092-443">Indica se o uso da tela de toque deve ou não ser bloqueado enquanto estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-443">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-444">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="1c092-444">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="1c092-445">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-445">Boolean</span></span>|<span data-ttu-id="1c092-446">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-446">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-447">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="1c092-447">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="1c092-448">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-448">Boolean</span></span>|<span data-ttu-id="1c092-449">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-449">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="1c092-450">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="1c092-450">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="1c092-451">Use KioskModeBlockVolumeButtons em vez disso.</span><span class="sxs-lookup"><span data-stu-id="1c092-451">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="1c092-452">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="1c092-452">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="1c092-453">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-453">Boolean</span></span>|<span data-ttu-id="1c092-454">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-454">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="1c092-455">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="1c092-455">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="1c092-456">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-456">Boolean</span></span>|<span data-ttu-id="1c092-457">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-457">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-458">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1c092-458">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="1c092-459">String</span><span class="sxs-lookup"><span data-stu-id="1c092-459">String</span></span>|<span data-ttu-id="1c092-460">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-460">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="1c092-461">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="1c092-461">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="1c092-462">Propriedadekioskmodebuiltinappid</span><span class="sxs-lookup"><span data-stu-id="1c092-462">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="1c092-463">String</span><span class="sxs-lookup"><span data-stu-id="1c092-463">String</span></span>|<span data-ttu-id="1c092-464">ID para aplicativos internos a serem usados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-464">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="1c092-465">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não são definidos.</span><span class="sxs-lookup"><span data-stu-id="1c092-465">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="1c092-466">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="1c092-466">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="1c092-467">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-467">Boolean</span></span>|<span data-ttu-id="1c092-468">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-468">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-469">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="1c092-469">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="1c092-470">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-470">Boolean</span></span>|<span data-ttu-id="1c092-471">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-471">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-472">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="1c092-472">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="1c092-473">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-473">Boolean</span></span>|<span data-ttu-id="1c092-474">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-474">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-475">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="1c092-475">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="1c092-476">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-476">Boolean</span></span>|<span data-ttu-id="1c092-477">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-477">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-478">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="1c092-478">kioskModeRequireZoom</span></span>|<span data-ttu-id="1c092-479">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-479">Boolean</span></span>|<span data-ttu-id="1c092-480">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-480">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="1c092-481">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="1c092-481">kioskModeManagedAppId</span></span>|<span data-ttu-id="1c092-482">String</span><span class="sxs-lookup"><span data-stu-id="1c092-482">String</span></span>|<span data-ttu-id="1c092-483">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="1c092-483">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="1c092-484">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="1c092-484">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="1c092-485">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="1c092-485">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="1c092-486">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-486">Boolean</span></span>|<span data-ttu-id="1c092-487">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="1c092-487">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="1c092-488">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="1c092-488">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="1c092-489">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-489">Boolean</span></span>|<span data-ttu-id="1c092-490">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="1c092-490">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="1c092-491">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="1c092-491">lockScreenBlockPassbook</span></span>|<span data-ttu-id="1c092-492">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-492">Boolean</span></span>|<span data-ttu-id="1c092-493">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="1c092-493">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="1c092-494">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="1c092-494">lockScreenBlockTodayView</span></span>|<span data-ttu-id="1c092-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c092-495">Boolean</span></span>|<span data-ttu-id="1c092-496">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="1c092-496">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="1c092-497">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="1c092-497">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="1c092-498">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="1c092-498">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="1c092-499">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="1c092-499">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="1c092-500">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="1c092-500">mediaContentRatingCanada</span></span>|[<span data-ttu-id="1c092-501">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="1c092-501">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="1c092-502">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="1c092-502">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="1c092-503">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="1c092-503">mediaContentRatingFrance</span></span>|[<span data-ttu-id="1c092-504">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="1c092-504">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="1c092-505">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="1c092-505">Media content rating settings for France</span></span>|
|<span data-ttu-id="1c092-506">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="1c092-506">mediaContentRatingGermany</span></span>|[<span data-ttu-id="1c092-507">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="1c092-507">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="1c092-508">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="1c092-508">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="1c092-509">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="1c092-509">mediaContentRatingIreland</span></span>|[<span data-ttu-id="1c092-510">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="1c092-510">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="1c092-511">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="1c092-511">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="1c092-512">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="1c092-512">mediaContentRatingJapan</span></span>|[<span data-ttu-id="1c092-513">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="1c092-513">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="1c092-514">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="1c092-514">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="1c092-515">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="1c092-515">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="1c092-516">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="1c092-516">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="1c092-517">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="1c092-517">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="1c092-518">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="1c092-518">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="1c092-519">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="1c092-519">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="1c092-520">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="1c092-520">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="1c092-521">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="1c092-521">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="1c092-522">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="1c092-522">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="1c092-523">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="1c092-523">Media content rating settings for United States</span></span>|
|<span data-ttu-id="1c092-524">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="1c092-524">networkUsageRules</span></span>|<span data-ttu-id="1c092-525">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="1c092-525">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="1c092-526">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="1c092-526">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="1c092-527">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="1c092-527">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="1c092-528">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="1c092-528">mediaContentRatingApps</span></span>|[<span data-ttu-id="1c092-529">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="1c092-529">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="1c092-530">Configurações de classificação de conteúdo de mídia para aplicativos.</span><span class="sxs-lookup"><span data-stu-id="1c092-530">Media content rating settings for Apps.</span></span> <span data-ttu-id="1c092-531">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="1c092-531">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="1c092-532">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-532">messagesBlocked</span></span>|<span data-ttu-id="1c092-533">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-533">Boolean</span></span>|<span data-ttu-id="1c092-534">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-534">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="1c092-535">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="1c092-535">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="1c092-536">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-536">Boolean</span></span>|<span data-ttu-id="1c092-537">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-537">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="1c092-538">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="1c092-538">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="1c092-539">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-539">Boolean</span></span>|<span data-ttu-id="1c092-540">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1c092-540">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="1c092-541">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="1c092-541">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="1c092-542">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-542">Boolean</span></span>|<span data-ttu-id="1c092-543">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-543">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="1c092-544">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="1c092-544">passcodeBlockModification</span></span>|<span data-ttu-id="1c092-545">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-545">Boolean</span></span>|<span data-ttu-id="1c092-546">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-546">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1c092-547">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="1c092-547">passcodeBlockSimple</span></span>|<span data-ttu-id="1c092-548">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-548">Boolean</span></span>|<span data-ttu-id="1c092-549">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="1c092-549">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="1c092-550">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1c092-550">passcodeExpirationDays</span></span>|<span data-ttu-id="1c092-551">Int32</span><span class="sxs-lookup"><span data-stu-id="1c092-551">Int32</span></span>|<span data-ttu-id="1c092-552">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="1c092-552">Number of days before the passcode expires.</span></span> <span data-ttu-id="1c092-553">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="1c092-553">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="1c092-554">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1c092-554">passcodeMinimumLength</span></span>|<span data-ttu-id="1c092-555">Int32</span><span class="sxs-lookup"><span data-stu-id="1c092-555">Int32</span></span>|<span data-ttu-id="1c092-556">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="1c092-556">Minimum length of passcode.</span></span> <span data-ttu-id="1c092-557">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="1c092-557">Valid values 4 to 14</span></span>|
|<span data-ttu-id="1c092-558">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1c092-558">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1c092-559">Int32</span><span class="sxs-lookup"><span data-stu-id="1c092-559">Int32</span></span>|<span data-ttu-id="1c092-560">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="1c092-560">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="1c092-561">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1c092-561">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1c092-562">Int32</span><span class="sxs-lookup"><span data-stu-id="1c092-562">Int32</span></span>|<span data-ttu-id="1c092-563">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="1c092-563">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1c092-564">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="1c092-564">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="1c092-565">Int32</span><span class="sxs-lookup"><span data-stu-id="1c092-565">Int32</span></span>|<span data-ttu-id="1c092-566">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="1c092-566">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="1c092-567">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="1c092-567">Valid values 0 to 4</span></span>|
|<span data-ttu-id="1c092-568">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="1c092-568">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="1c092-569">Int32</span><span class="sxs-lookup"><span data-stu-id="1c092-569">Int32</span></span>|<span data-ttu-id="1c092-570">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="1c092-570">Number of previous passcodes to block.</span></span> <span data-ttu-id="1c092-571">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="1c092-571">Valid values 1 to 24</span></span>|
|<span data-ttu-id="1c092-572">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="1c092-572">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="1c092-573">Int32</span><span class="sxs-lookup"><span data-stu-id="1c092-573">Int32</span></span>|<span data-ttu-id="1c092-574">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1c092-574">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="1c092-575">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="1c092-575">Valid values 4 to 11</span></span>|
|<span data-ttu-id="1c092-576">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="1c092-576">passcodeRequiredType</span></span>|[<span data-ttu-id="1c092-577">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1c092-577">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="1c092-578">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="1c092-578">Type of passcode that is required.</span></span> <span data-ttu-id="1c092-579">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="1c092-579">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="1c092-580">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="1c092-580">passcodeRequired</span></span>|<span data-ttu-id="1c092-581">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-581">Boolean</span></span>|<span data-ttu-id="1c092-582">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="1c092-582">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="1c092-583">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-583">podcastsBlocked</span></span>|<span data-ttu-id="1c092-584">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-584">Boolean</span></span>|<span data-ttu-id="1c092-585">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-585">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="1c092-586">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="1c092-586">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="1c092-587">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-587">Boolean</span></span>|<span data-ttu-id="1c092-588">Indica se o prompt deve ou não ser habilitado para configurar dispositivos próximos com um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-588">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="1c092-589">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="1c092-589">safariBlockAutofill</span></span>|<span data-ttu-id="1c092-590">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-590">Boolean</span></span>|<span data-ttu-id="1c092-591">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="1c092-591">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="1c092-592">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="1c092-592">safariBlockJavaScript</span></span>|<span data-ttu-id="1c092-593">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-593">Boolean</span></span>|<span data-ttu-id="1c092-594">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="1c092-594">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="1c092-595">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="1c092-595">safariBlockPopups</span></span>|<span data-ttu-id="1c092-596">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-596">Boolean</span></span>|<span data-ttu-id="1c092-597">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="1c092-597">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="1c092-598">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-598">safariBlocked</span></span>|<span data-ttu-id="1c092-599">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-599">Boolean</span></span>|<span data-ttu-id="1c092-600">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="1c092-600">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="1c092-601">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="1c092-601">safariCookieSettings</span></span>|[<span data-ttu-id="1c092-602">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="1c092-602">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="1c092-603">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="1c092-603">Cookie settings for Safari.</span></span> <span data-ttu-id="1c092-604">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="1c092-604">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="1c092-605">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="1c092-605">safariManagedDomains</span></span>|<span data-ttu-id="1c092-606">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1c092-606">String collection</span></span>|<span data-ttu-id="1c092-607">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="1c092-607">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="1c092-608">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="1c092-608">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="1c092-609">String collection</span><span class="sxs-lookup"><span data-stu-id="1c092-609">String collection</span></span>|<span data-ttu-id="1c092-610">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="1c092-610">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="1c092-611">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-611">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="1c092-612">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="1c092-612">safariRequireFraudWarning</span></span>|<span data-ttu-id="1c092-613">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-613">Boolean</span></span>|<span data-ttu-id="1c092-614">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="1c092-614">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="1c092-615">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-615">screenCaptureBlocked</span></span>|<span data-ttu-id="1c092-616">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-616">Boolean</span></span>|<span data-ttu-id="1c092-617">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="1c092-617">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="1c092-618">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-618">siriBlocked</span></span>|<span data-ttu-id="1c092-619">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-619">Boolean</span></span>|<span data-ttu-id="1c092-620">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="1c092-620">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="1c092-621">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="1c092-621">siriBlockedWhenLocked</span></span>|<span data-ttu-id="1c092-622">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-622">Boolean</span></span>|<span data-ttu-id="1c092-623">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1c092-623">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="1c092-624">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="1c092-624">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="1c092-625">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c092-625">Boolean</span></span>|<span data-ttu-id="1c092-626">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-626">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="1c092-627">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="1c092-627">siriRequireProfanityFilter</span></span>|<span data-ttu-id="1c092-628">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-628">Boolean</span></span>|<span data-ttu-id="1c092-629">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-629">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="1c092-630">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="1c092-630">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="1c092-631">Int32</span><span class="sxs-lookup"><span data-stu-id="1c092-631">Int32</span></span>|<span data-ttu-id="1c092-632">Define o número de dias que uma atualização de software será delyed para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-632">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="1c092-633">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="1c092-633">Valid values 0 to 90</span></span>|
|<span data-ttu-id="1c092-634">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="1c092-634">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="1c092-635">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-635">Boolean</span></span>|<span data-ttu-id="1c092-636">Indica se o usuário deve ou não atrasar a visibilidade de atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-636">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-637">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="1c092-637">spotlightBlockInternetResults</span></span>|<span data-ttu-id="1c092-638">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-638">Boolean</span></span>|<span data-ttu-id="1c092-639">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-639">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="1c092-640">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-640">voiceDialingBlocked</span></span>|<span data-ttu-id="1c092-641">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-641">Boolean</span></span>|<span data-ttu-id="1c092-642">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1c092-642">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="1c092-643">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="1c092-643">wallpaperBlockModification</span></span>|<span data-ttu-id="1c092-644">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-644">Boolean</span></span>|<span data-ttu-id="1c092-645">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-645">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="1c092-646">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="1c092-646">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="1c092-647">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c092-647">Boolean</span></span>|<span data-ttu-id="1c092-648">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="1c092-648">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1c092-649">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="1c092-649">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="1c092-650">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-650">Boolean</span></span>|<span data-ttu-id="1c092-651">Indica se um aluno inscrito em um curso não gerenciado via sala de aula solicitará permissão do professor ao tentar sair do curso (iOS 11,3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-651">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="1c092-652">Propriedadeskeychainblockcloudsync</span><span class="sxs-lookup"><span data-stu-id="1c092-652">keychainBlockCloudSync</span></span>|<span data-ttu-id="1c092-653">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-653">Boolean</span></span>|<span data-ttu-id="1c092-654">Indica se a sincronização de chaves do iCloud está bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="1c092-654">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="1c092-655">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="1c092-655">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="1c092-656">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-656">Boolean</span></span>|<span data-ttu-id="1c092-657">Indica se as atualizações de PKI de over-the-Air serão bloqueadas ou não.</span><span class="sxs-lookup"><span data-stu-id="1c092-657">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="1c092-658">A definição dessa restrição como false não desabilita as verificações de CRL e OCSP (iOS 7,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-658">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="1c092-659">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="1c092-659">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="1c092-660">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-660">Boolean</span></span>|<span data-ttu-id="1c092-661">Indica se o controle do AD é limitado. (iOS 7,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-661">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="1c092-662">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="1c092-662">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="1c092-663">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-663">Boolean</span></span>|<span data-ttu-id="1c092-664">Indica se o backup do catálogo empresarial deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1c092-664">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="1c092-665">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="1c092-665">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="1c092-666">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-666">Boolean</span></span>|<span data-ttu-id="1c092-667">Indica se a sincronização de notas e destaques do catálogo empresarial será bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1c092-667">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="1c092-668">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-668">airPrintBlocked</span></span>|<span data-ttu-id="1c092-669">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-669">Boolean</span></span>|<span data-ttu-id="1c092-670">Indica se o arquivo de impressão está bloqueado ou não (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-670">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1c092-671">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="1c092-671">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="1c092-672">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-672">Boolean</span></span>|<span data-ttu-id="1c092-673">Indica se o armazenamento de chaves de nome de usuário e a senha para impressão de uma ou não é bloqueado (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-673">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1c092-674">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="1c092-674">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="1c092-675">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-675">Boolean</span></span>|<span data-ttu-id="1c092-676">Indica se os certificados confiáveis são necessários para a comunicação de impressão TLS (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-676">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1c092-677">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="1c092-677">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="1c092-678">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-678">Boolean</span></span>|<span data-ttu-id="1c092-679">Indica se a descoberta de impressoras de impressão do iBeacon está ou não bloqueada.</span><span class="sxs-lookup"><span data-stu-id="1c092-679">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="1c092-680">Isso impede os beacons Bluetooth de impressão de mensagens de phishing para tráfego de rede (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-680">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1c092-681">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="1c092-681">blockSystemAppRemoval</span></span>|<span data-ttu-id="1c092-682">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-682">Boolean</span></span>|<span data-ttu-id="1c092-683">Indica se a remoção de aplicativos do sistema do dispositivo é bloqueada em um dispositivo supervisionado (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-683">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1c092-684">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="1c092-684">vpnBlockCreation</span></span>|<span data-ttu-id="1c092-685">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-685">Boolean</span></span>|<span data-ttu-id="1c092-686">Indica se a criação de configurações de VPN está bloqueada (iOS 11,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-686">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1c092-687">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-687">appRemovalBlocked</span></span>|<span data-ttu-id="1c092-688">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-688">Boolean</span></span>|<span data-ttu-id="1c092-689">Indica se a remoção de aplicativos é permitida.</span><span class="sxs-lookup"><span data-stu-id="1c092-689">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="1c092-690">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="1c092-690">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="1c092-691">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-691">Boolean</span></span>|<span data-ttu-id="1c092-692">Indica se a conexão a acessórios USB enquanto o dispositivo está bloqueado é permitida (iOS 11.4.1 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-692">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="1c092-693">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="1c092-693">passwordBlockAutoFill</span></span>|<span data-ttu-id="1c092-694">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-694">Boolean</span></span>|<span data-ttu-id="1c092-695">Indica se o recurso de senha de preenchimento automático é permitido (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-695">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="1c092-696">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="1c092-696">passwordBlockProximityRequests</span></span>|<span data-ttu-id="1c092-697">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-697">Boolean</span></span>|<span data-ttu-id="1c092-698">Indica se as senhas de solicitação devem ou não ser bloqueadas de dispositivos próximos (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-698">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="1c092-699">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="1c092-699">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="1c092-700">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-700">Boolean</span></span>|<span data-ttu-id="1c092-701">Indica se as senhas de compartilhamento devem ou não ser bloqueadas com o recurso de senhas de soltura de estours iOS 12,0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="1c092-701">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="1c092-702">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="1c092-702">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="1c092-703">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-703">Boolean</span></span>|<span data-ttu-id="1c092-704">Indica se o recurso "definir automaticamente" de data e hora está habilitado e não pode ser desativado pelo usuário (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-704">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="1c092-705">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="1c092-705">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="1c092-706">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-706">Boolean</span></span>|<span data-ttu-id="1c092-707">Indica se os aplicativos gerenciados podem ou não gravar contatos para contas de contatos não gerenciados (iOS 12,0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-707">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="1c092-708">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="1c092-708">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="1c092-709">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-709">Boolean</span></span>|<span data-ttu-id="1c092-710">Indica se os aplicativos não gerenciados podem ler de contas de contatos gerenciados (iOS 12,0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-710">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="1c092-711">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="1c092-711">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="1c092-712">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-712">Boolean</span></span>|<span data-ttu-id="1c092-713">Indica se o usuário será ou não impedido de modificar a configuração de hotspot pessoal (iOS 12,2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-713">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="1c092-714">siriDisableServerLogging</span><span class="sxs-lookup"><span data-stu-id="1c092-714">siriDisableServerLogging</span></span>|<span data-ttu-id="1c092-715">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c092-715">Boolean</span></span>|<span data-ttu-id="1c092-716">Indica se o registro em log do lado do servidor do Siri está desabilitado (iOS 12,2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="1c092-716">Indicates whether or not server-side Siri logging is disabled (iOS 12.2 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="1c092-717">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c092-717">Response</span></span>
<span data-ttu-id="1c092-718">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c092-718">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c092-719">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c092-719">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c092-720">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1c092-720">Request</span></span>
<span data-ttu-id="1c092-721">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c092-721">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10159

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

### <a name="response"></a><span data-ttu-id="1c092-722">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c092-722">Response</span></span>
<span data-ttu-id="1c092-p142">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1c092-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10331

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





