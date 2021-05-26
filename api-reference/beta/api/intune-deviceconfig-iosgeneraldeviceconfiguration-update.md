---
title: Atualizar iosGeneralDeviceConfiguration
description: Atualizar as propriedades de um objeto iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: febd45d2e3682584890a7aacc18e9701bb147b9f
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665389"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="d275d-103">Atualizar iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d275d-103">Update iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="d275d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d275d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d275d-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d275d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d275d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d275d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d275d-107">Atualizar as propriedades de um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d275d-107">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d275d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d275d-108">Prerequisites</span></span>
<span data-ttu-id="d275d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d275d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d275d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d275d-111">Permission type</span></span>|<span data-ttu-id="d275d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d275d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d275d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d275d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d275d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d275d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d275d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d275d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d275d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d275d-116">Not supported.</span></span>|
|<span data-ttu-id="d275d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d275d-117">Application</span></span>|<span data-ttu-id="d275d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d275d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d275d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d275d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d275d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d275d-120">Request headers</span></span>
|<span data-ttu-id="d275d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d275d-121">Header</span></span>|<span data-ttu-id="d275d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d275d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d275d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d275d-123">Authorization</span></span>|<span data-ttu-id="d275d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d275d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d275d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d275d-125">Accept</span></span>|<span data-ttu-id="d275d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d275d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d275d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d275d-127">Request body</span></span>
<span data-ttu-id="d275d-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d275d-128">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="d275d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d275d-129">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="d275d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d275d-130">Property</span></span>|<span data-ttu-id="d275d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d275d-131">Type</span></span>|<span data-ttu-id="d275d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d275d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d275d-133">id</span><span class="sxs-lookup"><span data-stu-id="d275d-133">id</span></span>|<span data-ttu-id="d275d-134">String</span><span class="sxs-lookup"><span data-stu-id="d275d-134">String</span></span>|<span data-ttu-id="d275d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d275d-135">Key of the entity.</span></span> <span data-ttu-id="d275d-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d275d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d275d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d275d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d275d-138">DateTimeOffset</span></span>|<span data-ttu-id="d275d-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d275d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d275d-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d275d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d275d-141">roleScopeTagIds</span></span>|<span data-ttu-id="d275d-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d275d-142">String collection</span></span>|<span data-ttu-id="d275d-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="d275d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d275d-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d275d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d275d-145">supportsScopeTags</span></span>|<span data-ttu-id="d275d-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-146">Boolean</span></span>|<span data-ttu-id="d275d-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d275d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d275d-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d275d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d275d-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d275d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d275d-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d275d-150">This property is read-only.</span></span> <span data-ttu-id="d275d-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d275d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d275d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d275d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d275d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d275d-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d275d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d275d-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d275d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d275d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d275d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d275d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d275d-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d275d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d275d-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d275d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d275d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d275d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d275d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d275d-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="d275d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d275d-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d275d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d275d-164">createdDateTime</span></span>|<span data-ttu-id="d275d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d275d-165">DateTimeOffset</span></span>|<span data-ttu-id="d275d-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d275d-166">DateTime the object was created.</span></span> <span data-ttu-id="d275d-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d275d-168">descrição</span><span class="sxs-lookup"><span data-stu-id="d275d-168">description</span></span>|<span data-ttu-id="d275d-169">String</span><span class="sxs-lookup"><span data-stu-id="d275d-169">String</span></span>|<span data-ttu-id="d275d-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d275d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d275d-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d275d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d275d-172">displayName</span></span>|<span data-ttu-id="d275d-173">String</span><span class="sxs-lookup"><span data-stu-id="d275d-173">String</span></span>|<span data-ttu-id="d275d-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d275d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d275d-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d275d-176">versão</span><span class="sxs-lookup"><span data-stu-id="d275d-176">version</span></span>|<span data-ttu-id="d275d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d275d-177">Int32</span></span>|<span data-ttu-id="d275d-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d275d-178">Version of the device configuration.</span></span> <span data-ttu-id="d275d-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d275d-180">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="d275d-180">accountBlockModification</span></span>|<span data-ttu-id="d275d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-181">Boolean</span></span>|<span data-ttu-id="d275d-182">Indica se a modificação da conta será permitida ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-182">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-183">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="d275d-183">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="d275d-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-184">Boolean</span></span>|<span data-ttu-id="d275d-185">Indica se o bloqueio de ativação será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-185">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="d275d-186">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-186">airDropBlocked</span></span>|<span data-ttu-id="d275d-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-187">Boolean</span></span>|<span data-ttu-id="d275d-188">Indica se o AirDrop será permitido ou não quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-188">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-189">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="d275d-189">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="d275d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-190">Boolean</span></span>|<span data-ttu-id="d275d-191">Indica se o AirDrop deverá ou não ser considerado uma reprodução automática não gerenciada (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-191">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d275d-192">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="d275d-192">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="d275d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-193">Boolean</span></span>|<span data-ttu-id="d275d-194">Indica se todos os dispositivos serão forçados a receber solicitações do AirPlay por este dispositivo para usar uma senha de emparelhamento.</span><span class="sxs-lookup"><span data-stu-id="d275d-194">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="d275d-195">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="d275d-195">appleWatchBlockPairing</span></span>|<span data-ttu-id="d275d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-196">Boolean</span></span>|<span data-ttu-id="d275d-197">Indica se o emparelhamento do Apple Watch será ou não permitido quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-197">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d275d-198">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="d275d-198">appleWatchForceWristDetection</span></span>|<span data-ttu-id="d275d-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-199">Boolean</span></span>|<span data-ttu-id="d275d-200">Indica se um Apple Watch emparelhado será forçado a usar Detecção de Pulso (iOS 8.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-200">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="d275d-201">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-201">appleNewsBlocked</span></span>|<span data-ttu-id="d275d-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-202">Boolean</span></span>|<span data-ttu-id="d275d-203">Indica se o usuário será ou não impedido de usar Notícias quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-203">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d275d-204">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="d275d-204">appsSingleAppModeList</span></span>|<span data-ttu-id="d275d-205">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d275d-206">Obtém ou define a lista de aplicativos iOS que podem entrar de forma autônoma no Modo de Aplicativo Único.</span><span class="sxs-lookup"><span data-stu-id="d275d-206">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="d275d-207">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-207">Supervised only.</span></span> <span data-ttu-id="d275d-208">iOS 7.0 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-208">iOS 7.0 and later.</span></span> <span data-ttu-id="d275d-209">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d275d-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d275d-210">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="d275d-210">appsVisibilityList</span></span>|<span data-ttu-id="d275d-211">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-211">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d275d-212">Lista de aplicativos na lista de visibilidade (lista de aplicativos visíveis/inicializávelis ou lista de aplicativos ocultos/não inicializáveis, controlados por AppsVisibilityListType) (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-212">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="d275d-213">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d275d-213">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d275d-214">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="d275d-214">appsVisibilityListType</span></span>|[<span data-ttu-id="d275d-215">appListType</span><span class="sxs-lookup"><span data-stu-id="d275d-215">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d275d-216">Tipo de lista que está em AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="d275d-216">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="d275d-217">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d275d-217">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d275d-218">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="d275d-218">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="d275d-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-219">Boolean</span></span>|<span data-ttu-id="d275d-220">Indica se será bloqueado ou não o download automático de aplicativos comprados em outros dispositivos quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-220">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d275d-221">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-221">appStoreBlocked</span></span>|<span data-ttu-id="d275d-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-222">Boolean</span></span>|<span data-ttu-id="d275d-223">Indica se o usuário será ou não impedido de usar a App Store.</span><span class="sxs-lookup"><span data-stu-id="d275d-223">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="d275d-224">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-224">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d275d-225">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="d275d-225">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="d275d-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-226">Boolean</span></span>|<span data-ttu-id="d275d-227">Indica se o usuário será ou não impedido de fazer compras no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d275d-227">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="d275d-228">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d275d-228">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="d275d-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-229">Boolean</span></span>|<span data-ttu-id="d275d-230">Indica se o aplicativo da App Store será bloqueado ou não, o que não restringe a instalação por meio de aplicativos do host.</span><span class="sxs-lookup"><span data-stu-id="d275d-230">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="d275d-231">Aplica-se apenas ao modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-231">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d275d-232">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="d275d-232">appStoreRequirePassword</span></span>|<span data-ttu-id="d275d-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-233">Boolean</span></span>|<span data-ttu-id="d275d-234">Indica se uma senha deve ou não ser exigida ao usar a loja de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d275d-234">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="d275d-235">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="d275d-235">autoFillForceAuthentication</span></span>|<span data-ttu-id="d275d-236">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-236">Boolean</span></span>|<span data-ttu-id="d275d-237">Indica se a autenticação do usuário deve ou não forçar o preenchimento automático de senhas e informações de cartão de crédito no Safari e em outros aplicativos em dispositivos supervisionados.</span><span class="sxs-lookup"><span data-stu-id="d275d-237">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="d275d-238">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="d275d-238">bluetoothBlockModification</span></span>|<span data-ttu-id="d275d-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-239">Boolean</span></span>|<span data-ttu-id="d275d-240">Indica se a modificação das configurações do Bluetooth será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 10.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-240">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="d275d-241">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-241">cameraBlocked</span></span>|<span data-ttu-id="d275d-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-242">Boolean</span></span>|<span data-ttu-id="d275d-243">Indica se o usuário será ou não impedido de acessar a câmera do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d275d-243">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="d275d-244">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-244">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d275d-245">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="d275d-245">cellularBlockDataRoaming</span></span>|<span data-ttu-id="d275d-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-246">Boolean</span></span>|<span data-ttu-id="d275d-247">Indica se o roaming de dados deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d275d-247">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="d275d-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="d275d-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="d275d-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-249">Boolean</span></span>|<span data-ttu-id="d275d-250">Indica se a busca global em segundo plano será ou não bloqueada durante roaming.</span><span class="sxs-lookup"><span data-stu-id="d275d-250">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="d275d-251">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="d275d-251">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="d275d-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-252">Boolean</span></span>|<span data-ttu-id="d275d-253">Indica se as alterações em configurações de uso de dados do aplicativo de rede celular serão ou não permitidas quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-253">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-254">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="d275d-254">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="d275d-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-255">Boolean</span></span>|<span data-ttu-id="d275d-256">Indica se o hotspot pessoal deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d275d-256">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="d275d-257">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="d275d-257">cellularBlockPlanModification</span></span>|<span data-ttu-id="d275d-258">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-258">Boolean</span></span>|<span data-ttu-id="d275d-259">Indica se os usuários podem ou não permitir que os usuários alterem as configurações do plano celular em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-259">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="d275d-260">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="d275d-260">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="d275d-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-261">Boolean</span></span>|<span data-ttu-id="d275d-262">Indica se o roaming de voz deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d275d-262">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="d275d-263">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="d275d-263">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="d275d-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-264">Boolean</span></span>|<span data-ttu-id="d275d-265">Indica se os certificados TLS não confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d275d-265">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="d275d-266">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d275d-266">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="d275d-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-267">Boolean</span></span>|<span data-ttu-id="d275d-268">Indica se a observação de tela remota pelo aplicativo Classroom será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-268">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d275d-269">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d275d-269">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="d275d-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-270">Boolean</span></span>|<span data-ttu-id="d275d-271">Indica se o professor de um curso gerenciado no aplicativo Classroom terá ou não permissão automática para visualizar a tela de um aluno sem solicitar quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-271">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-272">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="d275d-272">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="d275d-273">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-273">Boolean</span></span>|<span data-ttu-id="d275d-274">Indica se o usuário deve ou não dar permissão automaticamente às solicitações do professor, sem solicitar ao aluno, quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-274">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-275">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="d275d-275">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="d275d-276">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-276">Boolean</span></span>|<span data-ttu-id="d275d-277">Indica se o professor deve ou não permitir que o professor bloqueie aplicativos ou o dispositivo sem solicitar ao aluno.</span><span class="sxs-lookup"><span data-stu-id="d275d-277">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="d275d-278">Apenas em modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-278">Supervised only.</span></span>|
|<span data-ttu-id="d275d-279">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="d275d-279">compliantAppsList</span></span>|<span data-ttu-id="d275d-280">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-280">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d275d-281">Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="d275d-281">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="d275d-282">Essa coleção pode conter um máximo de 10.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d275d-282">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d275d-283">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="d275d-283">compliantAppListType</span></span>|[<span data-ttu-id="d275d-284">appListType</span><span class="sxs-lookup"><span data-stu-id="d275d-284">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d275d-285">Lista que está em AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="d275d-285">List that is in the AppComplianceList.</span></span> <span data-ttu-id="d275d-286">Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d275d-286">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d275d-287">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="d275d-287">configurationProfileBlockChanges</span></span>|<span data-ttu-id="d275d-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-288">Boolean</span></span>|<span data-ttu-id="d275d-289">Indica se o usuário será ou não impedido de instalar perfis e certificados de configuração de maneira interativa quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-289">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-290">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-290">definitionLookupBlocked</span></span>|<span data-ttu-id="d275d-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-291">Boolean</span></span>|<span data-ttu-id="d275d-292">Indica se a consulta de definição será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-292">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="d275d-293">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="d275d-293">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="d275d-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-294">Boolean</span></span>|<span data-ttu-id="d275d-295">Indica se o usuário poderá ou não habilitar restrições nas configurações do dispositivo quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-295">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-296">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="d275d-296">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="d275d-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-297">Boolean</span></span>|<span data-ttu-id="d275d-298">Indica se será permitido ou não o uso da opção “Apagar todo o conteúdo e as configurações” quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-298">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-299">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="d275d-299">deviceBlockNameModification</span></span>|<span data-ttu-id="d275d-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-300">Boolean</span></span>|<span data-ttu-id="d275d-301">Indica se a modificação do nome do dispositivo será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-301">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d275d-302">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="d275d-302">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="d275d-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-303">Boolean</span></span>|<span data-ttu-id="d275d-304">Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d275d-304">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="d275d-305">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="d275d-305">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="d275d-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-306">Boolean</span></span>|<span data-ttu-id="d275d-307">Indica se a modificação das configurações de envio de diagnóstico será ou não permitida quando o dispositivo estiver no modo supervisionado (iOS 9.3.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-307">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="d275d-308">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="d275d-308">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="d275d-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-309">Boolean</span></span>|<span data-ttu-id="d275d-310">Indica se o usuário será ou não impedido de visualizar documentos gerenciados em aplicativos não gerenciados.</span><span class="sxs-lookup"><span data-stu-id="d275d-310">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="d275d-311">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="d275d-311">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="d275d-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-312">Boolean</span></span>|<span data-ttu-id="d275d-313">Indica se o usuário será ou não impedido de visualizar documentos não gerenciados em aplicativos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="d275d-313">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="d275d-314">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="d275d-314">emailInDomainSuffixes</span></span>|<span data-ttu-id="d275d-315">String collection</span><span class="sxs-lookup"><span data-stu-id="d275d-315">String collection</span></span>|<span data-ttu-id="d275d-316">Um endereço de email sem um sufixo que corresponde a qualquer uma dessas strings será considerado fora do domínio.</span><span class="sxs-lookup"><span data-stu-id="d275d-316">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="d275d-317">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="d275d-317">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="d275d-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-318">Boolean</span></span>|<span data-ttu-id="d275d-319">Indica se o usuário será ou não impedido de confiar em um aplicativo corporativo.</span><span class="sxs-lookup"><span data-stu-id="d275d-319">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="d275d-320">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="d275d-320">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="d275d-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-321">Boolean</span></span>|<span data-ttu-id="d275d-322">\[Preterido Configurar essa configuração e definir o valor como \] "true" não tem efeito no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d275d-322">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="d275d-323">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="d275d-323">esimBlockModification</span></span>|<span data-ttu-id="d275d-324">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-324">Boolean</span></span>|<span data-ttu-id="d275d-325">Indica se é ou não para permitir a adição ou remoção de planos celulares no eSIM de um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-325">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="d275d-326">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-326">faceTimeBlocked</span></span>|<span data-ttu-id="d275d-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-327">Boolean</span></span>|<span data-ttu-id="d275d-328">Indica se o usuário será ou não impedido de usar o FaceTime.</span><span class="sxs-lookup"><span data-stu-id="d275d-328">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="d275d-329">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-329">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d275d-330">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-330">findMyFriendsBlocked</span></span>|<span data-ttu-id="d275d-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-331">Boolean</span></span>|<span data-ttu-id="d275d-332">Indica se deve ou não bloquear as alterações para Encontrar Meus Amigos quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-332">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-333">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="d275d-333">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="d275d-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-334">Boolean</span></span>|<span data-ttu-id="d275d-335">Indica se o usuário será ou não impedido de ter amigos no Game Center.</span><span class="sxs-lookup"><span data-stu-id="d275d-335">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="d275d-336">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-336">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d275d-337">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="d275d-337">gamingBlockMultiplayer</span></span>|<span data-ttu-id="d275d-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-338">Boolean</span></span>|<span data-ttu-id="d275d-339">Indica se o usuário será ou não impedido de usar jogos para vários participantes.</span><span class="sxs-lookup"><span data-stu-id="d275d-339">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="d275d-340">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-340">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d275d-341">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-341">gameCenterBlocked</span></span>|<span data-ttu-id="d275d-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-342">Boolean</span></span>|<span data-ttu-id="d275d-343">Indica se o usuário será ou não impedido de usar o Game Center quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-343">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-344">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-344">hostPairingBlocked</span></span>|<span data-ttu-id="d275d-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-345">Boolean</span></span>|<span data-ttu-id="d275d-346">indica se será permitido ou não o emparelhamento de host para controlar os dispositivos com os quais um dispositivo iOS poderá ser pareado estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-346">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-347">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-347">iBooksStoreBlocked</span></span>|<span data-ttu-id="d275d-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-348">Boolean</span></span>|<span data-ttu-id="d275d-349">Indica se o usuário será ou não impedido de usar a iBooks Store quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-349">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-350">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="d275d-350">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="d275d-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-351">Boolean</span></span>|<span data-ttu-id="d275d-352">Indica se o usuário será ou não impedido de baixar mídia marcada como erótica da iBookstore.</span><span class="sxs-lookup"><span data-stu-id="d275d-352">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="d275d-353">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="d275d-353">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="d275d-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-354">Boolean</span></span>|<span data-ttu-id="d275d-355">Indica se o usuário deve ou não bloquear o trabalho contínuo iniciado no dispositivo iOS para outro dispositivo iOS ou macOS.</span><span class="sxs-lookup"><span data-stu-id="d275d-355">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="d275d-356">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="d275d-356">iCloudBlockBackup</span></span>|<span data-ttu-id="d275d-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-357">Boolean</span></span>|<span data-ttu-id="d275d-358">Indica se o backup do iCloud deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d275d-358">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="d275d-359">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-359">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d275d-360">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="d275d-360">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="d275d-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-361">Boolean</span></span>|<span data-ttu-id="d275d-362">Indica se a sincronização de documentos do iCloud deve ou não ser bloqueado. Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-362">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d275d-363">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="d275d-363">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="d275d-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-364">Boolean</span></span>|<span data-ttu-id="d275d-365">Indica se a Sincronização de nuvem de aplicativos gerenciados deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d275d-365">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="d275d-366">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="d275d-366">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="d275d-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-367">Boolean</span></span>|<span data-ttu-id="d275d-368">Indica se Biblioteca de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d275d-368">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="d275d-369">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="d275d-369">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="d275d-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-370">Boolean</span></span>|<span data-ttu-id="d275d-371">Indica se a sincronização do Fluxo de Fotos do iCloud deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d275d-371">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="d275d-372">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="d275d-372">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="d275d-373">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-373">Boolean</span></span>|<span data-ttu-id="d275d-374">Indica se a sincronização do Fluxo de Fotos Compartilhadas deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d275d-374">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="d275d-375">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="d275d-375">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="d275d-376">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-376">Boolean</span></span>|<span data-ttu-id="d275d-377">Indica se a criptografia de backups no iCloud será exigida ou não.</span><span class="sxs-lookup"><span data-stu-id="d275d-377">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="d275d-378">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="d275d-378">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="d275d-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-379">Boolean</span></span>|<span data-ttu-id="d275d-380">Indica se o usuário será ou não impedido de acessar conteúdo explícito no iTunes e na App Store.</span><span class="sxs-lookup"><span data-stu-id="d275d-380">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="d275d-381">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-381">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d275d-382">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="d275d-382">iTunesBlockMusicService</span></span>|<span data-ttu-id="d275d-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-383">Boolean</span></span>|<span data-ttu-id="d275d-384">Indica se o serviço de música será bloqueado e se o aplicativo Music será revertido ao modo clássico quando o dispositivo estiver no modo supervisionado (iOS 9.3 ou posterior e macOS 10.12 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-384">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="d275d-385">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="d275d-385">iTunesBlockRadio</span></span>|<span data-ttu-id="d275d-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-386">Boolean</span></span>|<span data-ttu-id="d275d-387">Indica se o usuário será ou não impedido de usar o iTunes Radio quando o dispositivo estiver no modo supervisionado (iOS 9.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-387">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d275d-388">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="d275d-388">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="d275d-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-389">Boolean</span></span>|<span data-ttu-id="d275d-390">Indica se a correção automática do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-390">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d275d-391">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="d275d-391">keyboardBlockDictation</span></span>|<span data-ttu-id="d275d-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-392">Boolean</span></span>|<span data-ttu-id="d275d-393">Indica se o usuário será ou não impedido de usar a entrada de ditado quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-393">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-394">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="d275d-394">keyboardBlockPredictive</span></span>|<span data-ttu-id="d275d-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-395">Boolean</span></span>|<span data-ttu-id="d275d-396">Indica se os teclados preditivos serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-396">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d275d-397">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="d275d-397">keyboardBlockShortcuts</span></span>|<span data-ttu-id="d275d-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-398">Boolean</span></span>|<span data-ttu-id="d275d-399">Indica se os atalhos de teclado serão ou não bloqueados quando o dispositivo estiver no modo supervisionado (iOS 9.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-399">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d275d-400">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="d275d-400">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="d275d-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-401">Boolean</span></span>|<span data-ttu-id="d275d-402">Indica se a verificação ortográfica do teclado será ou não bloqueada quando o dispositivo estiver no modo supervisionado (iOS 8.1.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-402">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d275d-403">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="d275d-403">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="d275d-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-404">Boolean</span></span>|<span data-ttu-id="d275d-405">Indica se a fala assistencial será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-405">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-406">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="d275d-406">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="d275d-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-407">Boolean</span></span>|<span data-ttu-id="d275d-408">Indica se o acesso às configurações do Toque assistencial será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-408">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-409">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="d275d-409">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="d275d-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-410">Boolean</span></span>|<span data-ttu-id="d275d-411">Indica se o bloqueio automático do dispositivo será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-411">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="d275d-412">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="d275d-412">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d275d-413">Em vez disso, use KioskModeBlockAutoLock.</span><span class="sxs-lookup"><span data-stu-id="d275d-413">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="d275d-414">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="d275d-414">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="d275d-415">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-415">Boolean</span></span>|<span data-ttu-id="d275d-416">Indica se o bloqueio automático do dispositivo deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-416">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-417">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="d275d-417">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="d275d-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-418">Boolean</span></span>|<span data-ttu-id="d275d-419">Indica se o acesso às configurações de Inversão de cores será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-419">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-420">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="d275d-420">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="d275d-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-421">Boolean</span></span>|<span data-ttu-id="d275d-422">Indica se o uso do botão de toque será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-422">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="d275d-423">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="d275d-423">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d275d-424">Use KioskModeBlockRingerSwitch.</span><span class="sxs-lookup"><span data-stu-id="d275d-424">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="d275d-425">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="d275d-425">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="d275d-426">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-426">Boolean</span></span>|<span data-ttu-id="d275d-427">Indica se o uso do aneler deve ou não ser bloqueado enquanto estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-427">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-428">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="d275d-428">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="d275d-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-429">Boolean</span></span>|<span data-ttu-id="d275d-430">Indica se a rotação de tela será permitida ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-430">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="d275d-431">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="d275d-431">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d275d-432">Use KioskModeBlockScreenRotation em vez disso.</span><span class="sxs-lookup"><span data-stu-id="d275d-432">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="d275d-433">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="d275d-433">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="d275d-434">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-434">Boolean</span></span>|<span data-ttu-id="d275d-435">Indica se a rotação da tela deve ou não ser bloqueado enquanto estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-435">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-436">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="d275d-436">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="d275d-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-437">Boolean</span></span>|<span data-ttu-id="d275d-438">Indica se o uso do botão de suspensão será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-438">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="d275d-439">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="d275d-439">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d275d-440">Use KioskModeBlockSleepButton em vez disso.</span><span class="sxs-lookup"><span data-stu-id="d275d-440">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="d275d-441">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="d275d-441">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="d275d-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-442">Boolean</span></span>|<span data-ttu-id="d275d-443">Indica se o uso do botão de sono deve ou não ser bloqueado enquanto estiver no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-443">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-444">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="d275d-444">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="d275d-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-445">Boolean</span></span>|<span data-ttu-id="d275d-446">Indica se o uso da tela touch será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-446">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="d275d-447">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="d275d-447">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d275d-448">Use KioskModeBlockTouchscreen em vez disso.</span><span class="sxs-lookup"><span data-stu-id="d275d-448">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="d275d-449">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="d275d-449">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="d275d-450">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-450">Boolean</span></span>|<span data-ttu-id="d275d-451">Indica se o uso da tela sensível ao toque deve ou não ser bloqueado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-451">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-452">kioskModeEnableVoiceControl</span><span class="sxs-lookup"><span data-stu-id="d275d-452">kioskModeEnableVoiceControl</span></span>|<span data-ttu-id="d275d-453">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-453">Boolean</span></span>|<span data-ttu-id="d275d-454">Indica se o controle de voz deve ou não ser habilitado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-454">Indicates whether or not to enable voice control in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-455">kioskModeAllowVoiceControlModification</span><span class="sxs-lookup"><span data-stu-id="d275d-455">kioskModeAllowVoiceControlModification</span></span>|<span data-ttu-id="d275d-456">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-456">Boolean</span></span>|<span data-ttu-id="d275d-457">Indica se o usuário pode ou não alternar o controle de voz no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-457">Indicates whether or not to allow the user to toggle voice control in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-458">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="d275d-458">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="d275d-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-459">Boolean</span></span>|<span data-ttu-id="d275d-460">Indica se o acesso às configurações de voice over será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-460">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-461">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="d275d-461">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="d275d-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-462">Boolean</span></span>|<span data-ttu-id="d275d-463">Indica se o uso dos botões de volume será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-463">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="d275d-464">A funcionalidade dessa propriedade é redundante com o padrão do sistema operacional e é preterida.</span><span class="sxs-lookup"><span data-stu-id="d275d-464">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d275d-465">Use KioskModeBlockVolumeButtons.</span><span class="sxs-lookup"><span data-stu-id="d275d-465">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="d275d-466">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="d275d-466">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="d275d-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-467">Boolean</span></span>|<span data-ttu-id="d275d-468">Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-468">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="d275d-469">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="d275d-469">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="d275d-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-470">Boolean</span></span>|<span data-ttu-id="d275d-471">Indica se o acesso às configurações de zoom será permitido ou não no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-471">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-472">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d275d-472">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="d275d-473">String</span><span class="sxs-lookup"><span data-stu-id="d275d-473">String</span></span>|<span data-ttu-id="d275d-474">URL na loja de aplicativos do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-474">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="d275d-475">Use se KioskModeManagedAppId não for conhecido.</span><span class="sxs-lookup"><span data-stu-id="d275d-475">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="d275d-476">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="d275d-476">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="d275d-477">String</span><span class="sxs-lookup"><span data-stu-id="d275d-477">String</span></span>|<span data-ttu-id="d275d-478">ID para aplicativos integrados a usar no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-478">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="d275d-479">Usado quando KioskModeManagedAppId e KioskModeAppStoreUrl não estão definidos.</span><span class="sxs-lookup"><span data-stu-id="d275d-479">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="d275d-480">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="d275d-480">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="d275d-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-481">Boolean</span></span>|<span data-ttu-id="d275d-482">Indica se o toque assistencial deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-482">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-483">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="d275d-483">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="d275d-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-484">Boolean</span></span>|<span data-ttu-id="d275d-485">Indica se a inversão de cores deve ou não ser exigida no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-485">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-486">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="d275d-486">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="d275d-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-487">Boolean</span></span>|<span data-ttu-id="d275d-488">Indica se o áudio mono deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-488">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-489">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="d275d-489">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="d275d-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-490">Boolean</span></span>|<span data-ttu-id="d275d-491">Indica se o voice over deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-491">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-492">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="d275d-492">kioskModeRequireZoom</span></span>|<span data-ttu-id="d275d-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-493">Boolean</span></span>|<span data-ttu-id="d275d-494">Indica se o zoom deve ou não ser exigido no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-494">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="d275d-495">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="d275d-495">kioskModeManagedAppId</span></span>|<span data-ttu-id="d275d-496">String</span><span class="sxs-lookup"><span data-stu-id="d275d-496">String</span></span>|<span data-ttu-id="d275d-497">ID de gerenciamento do aplicativo para uso no modo de quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-497">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="d275d-498">Se KioskModeManagedAppId for especificada, KioskModeAppStoreUrl será ignorada.</span><span class="sxs-lookup"><span data-stu-id="d275d-498">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="d275d-499">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="d275d-499">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="d275d-500">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-500">Boolean</span></span>|<span data-ttu-id="d275d-501">Indica se o usuário será ou não impedido de usar o centro de controle na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="d275d-501">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="d275d-502">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="d275d-502">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="d275d-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-503">Boolean</span></span>|<span data-ttu-id="d275d-504">Indica se o usuário será ou não impedido de usar a exibição de notificações na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="d275d-504">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="d275d-505">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="d275d-505">lockScreenBlockPassbook</span></span>|<span data-ttu-id="d275d-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-506">Boolean</span></span>|<span data-ttu-id="d275d-507">Indica se o usuário será ou não impedido de usar o Passbook quando o dispositivo estiver bloqueado</span><span class="sxs-lookup"><span data-stu-id="d275d-507">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="d275d-508">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="d275d-508">lockScreenBlockTodayView</span></span>|<span data-ttu-id="d275d-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-509">Boolean</span></span>|<span data-ttu-id="d275d-510">Indica se o usuário será ou não impedido de usar a exibição Hoje na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="d275d-510">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="d275d-511">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d275d-511">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="d275d-512">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d275d-512">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="d275d-513">Configurações de classificação de conteúdo de mídia da Austrália</span><span class="sxs-lookup"><span data-stu-id="d275d-513">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="d275d-514">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="d275d-514">mediaContentRatingCanada</span></span>|[<span data-ttu-id="d275d-515">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="d275d-515">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="d275d-516">Configurações de classificação de conteúdo de mídia do Canadá</span><span class="sxs-lookup"><span data-stu-id="d275d-516">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="d275d-517">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d275d-517">mediaContentRatingFrance</span></span>|[<span data-ttu-id="d275d-518">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d275d-518">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="d275d-519">Configurações de classificação de conteúdo de mídia da França</span><span class="sxs-lookup"><span data-stu-id="d275d-519">Media content rating settings for France</span></span>|
|<span data-ttu-id="d275d-520">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d275d-520">mediaContentRatingGermany</span></span>|[<span data-ttu-id="d275d-521">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d275d-521">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="d275d-522">Configurações de classificação de conteúdo de mídia da Alemanha</span><span class="sxs-lookup"><span data-stu-id="d275d-522">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="d275d-523">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="d275d-523">mediaContentRatingIreland</span></span>|[<span data-ttu-id="d275d-524">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="d275d-524">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="d275d-525">Configurações de classificação de conteúdo de mídia da Irlanda</span><span class="sxs-lookup"><span data-stu-id="d275d-525">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="d275d-526">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d275d-526">mediaContentRatingJapan</span></span>|[<span data-ttu-id="d275d-527">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d275d-527">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="d275d-528">Configurações de classificação de conteúdo de mídia do Japão</span><span class="sxs-lookup"><span data-stu-id="d275d-528">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="d275d-529">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d275d-529">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="d275d-530">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d275d-530">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="d275d-531">Configurações de classificação de conteúdo de mídia da Nova Zelândia</span><span class="sxs-lookup"><span data-stu-id="d275d-531">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="d275d-532">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="d275d-532">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="d275d-533">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="d275d-533">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="d275d-534">Configurações de classificação de conteúdo de mídia do Reino Unido</span><span class="sxs-lookup"><span data-stu-id="d275d-534">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="d275d-535">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d275d-535">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="d275d-536">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d275d-536">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="d275d-537">Configurações de classificação de conteúdo de mídia dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="d275d-537">Media content rating settings for United States</span></span>|
|<span data-ttu-id="d275d-538">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="d275d-538">networkUsageRules</span></span>|<span data-ttu-id="d275d-539">Coleção [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="d275d-539">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="d275d-540">Lista de aplicativos gerenciados e regras de rede que se aplicam a eles.</span><span class="sxs-lookup"><span data-stu-id="d275d-540">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="d275d-541">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="d275d-541">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="d275d-542">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="d275d-542">mediaContentRatingApps</span></span>|[<span data-ttu-id="d275d-543">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="d275d-543">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="d275d-544">Configurações de classificação de conteúdo de mídia para Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d275d-544">Media content rating settings for Apps.</span></span> <span data-ttu-id="d275d-545">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="d275d-545">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="d275d-546">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-546">messagesBlocked</span></span>|<span data-ttu-id="d275d-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-547">Boolean</span></span>|<span data-ttu-id="d275d-548">Indica se o usuário será ou não impedido de usar o aplicativo Mensagens no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-548">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="d275d-549">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="d275d-549">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="d275d-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-550">Boolean</span></span>|<span data-ttu-id="d275d-551">Indica se a modificação de configurações de notificações será permitida ou não no dispositivo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-551">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d275d-552">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d275d-552">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="d275d-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-553">Boolean</span></span>|<span data-ttu-id="d275d-554">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d275d-554">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="d275d-555">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="d275d-555">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="d275d-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-556">Boolean</span></span>|<span data-ttu-id="d275d-557">Impedir a modificação de impressões digitais registradas do Touch ID no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-557">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="d275d-558">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="d275d-558">passcodeBlockModification</span></span>|<span data-ttu-id="d275d-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-559">Boolean</span></span>|<span data-ttu-id="d275d-560">Indica se a modificação de senha será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-560">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d275d-561">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d275d-561">passcodeBlockSimple</span></span>|<span data-ttu-id="d275d-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-562">Boolean</span></span>|<span data-ttu-id="d275d-563">Indica se códigos de acesso simples devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d275d-563">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="d275d-564">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d275d-564">passcodeExpirationDays</span></span>|<span data-ttu-id="d275d-565">Int32</span><span class="sxs-lookup"><span data-stu-id="d275d-565">Int32</span></span>|<span data-ttu-id="d275d-566">Número de dias antes da expiração do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="d275d-566">Number of days before the passcode expires.</span></span> <span data-ttu-id="d275d-567">Valores válidos de 1 a 65535</span><span class="sxs-lookup"><span data-stu-id="d275d-567">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="d275d-568">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d275d-568">passcodeMinimumLength</span></span>|<span data-ttu-id="d275d-569">Int32</span><span class="sxs-lookup"><span data-stu-id="d275d-569">Int32</span></span>|<span data-ttu-id="d275d-570">Comprimento mínimo do código de acesso.</span><span class="sxs-lookup"><span data-stu-id="d275d-570">Minimum length of passcode.</span></span> <span data-ttu-id="d275d-571">Valores válidos de 4 a 14</span><span class="sxs-lookup"><span data-stu-id="d275d-571">Valid values 4 to 14</span></span>|
|<span data-ttu-id="d275d-572">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d275d-572">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d275d-573">Int32</span><span class="sxs-lookup"><span data-stu-id="d275d-573">Int32</span></span>|<span data-ttu-id="d275d-574">Minutos de inatividade antes que um código de acesso seja necessário.</span><span class="sxs-lookup"><span data-stu-id="d275d-574">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="d275d-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d275d-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d275d-576">Int32</span><span class="sxs-lookup"><span data-stu-id="d275d-576">Int32</span></span>|<span data-ttu-id="d275d-577">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="d275d-577">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d275d-578">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d275d-578">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="d275d-579">Int32</span><span class="sxs-lookup"><span data-stu-id="d275d-579">Int32</span></span>|<span data-ttu-id="d275d-580">Número de conjuntos de caracteres que uma senha deve conter.</span><span class="sxs-lookup"><span data-stu-id="d275d-580">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="d275d-581">Valores válidos de 0 a 4</span><span class="sxs-lookup"><span data-stu-id="d275d-581">Valid values 0 to 4</span></span>|
|<span data-ttu-id="d275d-582">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="d275d-582">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="d275d-583">Int32</span><span class="sxs-lookup"><span data-stu-id="d275d-583">Int32</span></span>|<span data-ttu-id="d275d-584">Número de códigos de acesso anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="d275d-584">Number of previous passcodes to block.</span></span> <span data-ttu-id="d275d-585">Valores válidos de 1 a 24</span><span class="sxs-lookup"><span data-stu-id="d275d-585">Valid values 1 to 24</span></span>|
|<span data-ttu-id="d275d-586">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="d275d-586">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="d275d-587">Int32</span><span class="sxs-lookup"><span data-stu-id="d275d-587">Int32</span></span>|<span data-ttu-id="d275d-588">Número permitido de falhas de entrada antes da limpeza do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d275d-588">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="d275d-589">Valores válidos de 2 a 11</span><span class="sxs-lookup"><span data-stu-id="d275d-589">Valid values 2 to 11</span></span>|
|<span data-ttu-id="d275d-590">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="d275d-590">passcodeRequiredType</span></span>|[<span data-ttu-id="d275d-591">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d275d-591">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d275d-592">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="d275d-592">Type of passcode that is required.</span></span> <span data-ttu-id="d275d-593">Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d275d-593">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d275d-594">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="d275d-594">passcodeRequired</span></span>|<span data-ttu-id="d275d-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-595">Boolean</span></span>|<span data-ttu-id="d275d-596">Indica se um código de acesso deve ou não ser exigido.</span><span class="sxs-lookup"><span data-stu-id="d275d-596">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="d275d-597">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-597">podcastsBlocked</span></span>|<span data-ttu-id="d275d-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-598">Boolean</span></span>|<span data-ttu-id="d275d-599">Indica se o usuário será ou não impedido de usar podcasts no dispositivo supervisionado (iOS 8.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-599">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="d275d-600">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="d275d-600">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="d275d-601">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-601">Boolean</span></span>|<span data-ttu-id="d275d-602">Indica se o prompt deve ou não habilitar a instalação de dispositivos próximos com um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-602">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="d275d-603">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="d275d-603">safariBlockAutofill</span></span>|<span data-ttu-id="d275d-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-604">Boolean</span></span>|<span data-ttu-id="d275d-605">Indica se o usuário será ou não impedido de usar o preenchimento automático no Safari.</span><span class="sxs-lookup"><span data-stu-id="d275d-605">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="d275d-606">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-606">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d275d-607">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="d275d-607">safariBlockJavaScript</span></span>|<span data-ttu-id="d275d-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-608">Boolean</span></span>|<span data-ttu-id="d275d-609">Indica se o JavaScript deve ou não ser bloqueado no Safari.</span><span class="sxs-lookup"><span data-stu-id="d275d-609">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="d275d-610">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="d275d-610">safariBlockPopups</span></span>|<span data-ttu-id="d275d-611">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-611">Boolean</span></span>|<span data-ttu-id="d275d-612">Indica se os popups devem ou não ser bloqueados no Safari.</span><span class="sxs-lookup"><span data-stu-id="d275d-612">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="d275d-613">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-613">safariBlocked</span></span>|<span data-ttu-id="d275d-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-614">Boolean</span></span>|<span data-ttu-id="d275d-615">Indica se o usuário será ou não impedido de usar o Safari.</span><span class="sxs-lookup"><span data-stu-id="d275d-615">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="d275d-616">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-616">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d275d-617">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d275d-617">safariCookieSettings</span></span>|[<span data-ttu-id="d275d-618">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d275d-618">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="d275d-619">Configurações de cookie do Safari.</span><span class="sxs-lookup"><span data-stu-id="d275d-619">Cookie settings for Safari.</span></span> <span data-ttu-id="d275d-620">Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="d275d-620">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="d275d-621">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="d275d-621">safariManagedDomains</span></span>|<span data-ttu-id="d275d-622">String collection</span><span class="sxs-lookup"><span data-stu-id="d275d-622">String collection</span></span>|<span data-ttu-id="d275d-623">As URLs correspondentes aos padrões indicados aqui serão consideradas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="d275d-623">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="d275d-624">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="d275d-624">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="d275d-625">String collection</span><span class="sxs-lookup"><span data-stu-id="d275d-625">String collection</span></span>|<span data-ttu-id="d275d-626">Os usuários podem salvar senhas no Safari somente de URLs correspondentes aos padrões indicados aqui.</span><span class="sxs-lookup"><span data-stu-id="d275d-626">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="d275d-627">Aplica-se a dispositivos no modo supervisionado (iOS 9.3 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-627">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d275d-628">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="d275d-628">safariRequireFraudWarning</span></span>|<span data-ttu-id="d275d-629">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-629">Boolean</span></span>|<span data-ttu-id="d275d-630">Indica se um aviso de fraude deve ou não ser exigido no Safari.</span><span class="sxs-lookup"><span data-stu-id="d275d-630">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="d275d-631">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-631">screenCaptureBlocked</span></span>|<span data-ttu-id="d275d-632">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-632">Boolean</span></span>|<span data-ttu-id="d275d-633">Indica se o usuário será ou não impedido de fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="d275d-633">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="d275d-634">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-634">siriBlocked</span></span>|<span data-ttu-id="d275d-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-635">Boolean</span></span>|<span data-ttu-id="d275d-636">Indica se o usuário será ou não impedido de usar a Siri.</span><span class="sxs-lookup"><span data-stu-id="d275d-636">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="d275d-637">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="d275d-637">siriBlockedWhenLocked</span></span>|<span data-ttu-id="d275d-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-638">Boolean</span></span>|<span data-ttu-id="d275d-639">Indica se o usuário será ou não impedido de usar a Siri com o dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d275d-639">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="d275d-640">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="d275d-640">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="d275d-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-641">Boolean</span></span>|<span data-ttu-id="d275d-642">Indica se a Siri será ou não impedida de consultar conteúdos gerados pelo usuário quando usada em um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-642">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="d275d-643">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="d275d-643">siriRequireProfanityFilter</span></span>|<span data-ttu-id="d275d-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-644">Boolean</span></span>|<span data-ttu-id="d275d-645">Indica se a Siri deve ou não ser impedida de utilizar linguagem imprópria no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-645">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="d275d-646">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="d275d-646">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="d275d-647">Int32</span><span class="sxs-lookup"><span data-stu-id="d275d-647">Int32</span></span>|<span data-ttu-id="d275d-648">Define quantos dias uma atualização de software será usada para um dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-648">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="d275d-649">Valores válidos de 0 a 90</span><span class="sxs-lookup"><span data-stu-id="d275d-649">Valid values 0 to 90</span></span>|
|<span data-ttu-id="d275d-650">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="d275d-650">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="d275d-651">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-651">Boolean</span></span>|<span data-ttu-id="d275d-652">Indica se o usuário deve ou não atrasar a visibilidade das atualizações de software quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-652">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d275d-653">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="d275d-653">spotlightBlockInternetResults</span></span>|<span data-ttu-id="d275d-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-654">Boolean</span></span>|<span data-ttu-id="d275d-655">Indica se a Pesquisa em Destaque poderá ou não retornar resultados da Internet no dispositivo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-655">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="d275d-656">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-656">voiceDialingBlocked</span></span>|<span data-ttu-id="d275d-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-657">Boolean</span></span>|<span data-ttu-id="d275d-658">Indica se a discagem de voz deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d275d-658">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="d275d-659">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="d275d-659">wallpaperBlockModification</span></span>|<span data-ttu-id="d275d-660">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-660">Boolean</span></span>|<span data-ttu-id="d275d-661">Indica se a modificação de papel de parede será permitida ou não no dispositivo supervisionado (iOS 9.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-661">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="d275d-662">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="d275d-662">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="d275d-663">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-663">Boolean</span></span>|<span data-ttu-id="d275d-664">Indica se o dispositivo será ou não forçado a usar apenas redes Wi-Fi de perfis de configuração quando o dispositivo estiver no modo supervisionado.</span><span class="sxs-lookup"><span data-stu-id="d275d-664">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span> <span data-ttu-id="d275d-665">Disponível para dispositivos que executam versões 14.4 e anteriores do iOS e iPadOS.</span><span class="sxs-lookup"><span data-stu-id="d275d-665">Available for devices running iOS and iPadOS versions 14.4 and earlier.</span></span> <span data-ttu-id="d275d-666">Os dispositivos que executam 14,5+ devem usar a configuração "WiFiConnectToAllowedNetworksOnlyForced.</span><span class="sxs-lookup"><span data-stu-id="d275d-666">Devices running 14.5+ should use the setting, “WiFiConnectToAllowedNetworksOnlyForced.</span></span>|
|<span data-ttu-id="d275d-667">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="d275d-667">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="d275d-668">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-668">Boolean</span></span>|<span data-ttu-id="d275d-669">Indica se um aluno matriculado em um curso não controlado via Classroom solicitará permissão do professor ao tentar sair do curso (iOS 11.3 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-669">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="d275d-670">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="d275d-670">keychainBlockCloudSync</span></span>|<span data-ttu-id="d275d-671">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-671">Boolean</span></span>|<span data-ttu-id="d275d-672">Indica se a sincronização do chaveiro do iCloud está bloqueada ou não.</span><span class="sxs-lookup"><span data-stu-id="d275d-672">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="d275d-673">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-673">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d275d-674">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="d275d-674">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="d275d-675">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-675">Boolean</span></span>|<span data-ttu-id="d275d-676">Indica se as atualizações PKI sobre o ar estão ou não bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="d275d-676">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="d275d-677">Definir essa restrição como false não desabilita as verificações de CRL e OCSP (iOS 7.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-677">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="d275d-678">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="d275d-678">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="d275d-679">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-679">Boolean</span></span>|<span data-ttu-id="d275d-680">Indica se o controle de ad é limitado. (iOS 7.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-680">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="d275d-681">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="d275d-681">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="d275d-682">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-682">Boolean</span></span>|<span data-ttu-id="d275d-683">Indica se o Enterprise de reserva está bloqueado ou não.</span><span class="sxs-lookup"><span data-stu-id="d275d-683">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="d275d-684">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="d275d-684">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="d275d-685">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-685">Boolean</span></span>|<span data-ttu-id="d275d-686">Indica se a sincronização de Enterprise e realçamentos do livro está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d275d-686">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="d275d-687">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-687">airPrintBlocked</span></span>|<span data-ttu-id="d275d-688">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-688">Boolean</span></span>|<span data-ttu-id="d275d-689">Indica se o AirPrint está ou não bloqueado (iOS 11.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-689">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d275d-690">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="d275d-690">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="d275d-691">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-691">Boolean</span></span>|<span data-ttu-id="d275d-692">Indica se o armazenamento de chaves de nome de usuário e senha para Airprint está bloqueado (iOS 11.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-692">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d275d-693">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="d275d-693">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="d275d-694">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-694">Boolean</span></span>|<span data-ttu-id="d275d-695">Indica se certificados confiáveis são necessários para comunicação de impressão TLS (iOS 11.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-695">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d275d-696">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="d275d-696">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="d275d-697">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-697">Boolean</span></span>|<span data-ttu-id="d275d-698">Indica se a descoberta iBeacon ou não de impressoras AirPrint está bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d275d-698">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="d275d-699">Isso impede que os sinalizadores AirPrint Bluetooth phishing para tráfego de rede (iOS 11.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-699">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d275d-700">filesNetworkDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-700">filesNetworkDriveAccessBlocked</span></span>|<span data-ttu-id="d275d-701">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-701">Boolean</span></span>|<span data-ttu-id="d275d-702">Indica se os dispositivos podem acessar arquivos ou outros recursos em um servidor de rede usando o protocolo SMB (Server Message Block).</span><span class="sxs-lookup"><span data-stu-id="d275d-702">Indicates if devices can access files or other resources on a network server using the Server Message Block (SMB) protocol.</span></span> <span data-ttu-id="d275d-703">Disponível para dispositivos que executam iOS e iPadOS, versões 13.0 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="d275d-703">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="d275d-704">filesUsbDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-704">filesUsbDriveAccessBlocked</span></span>|<span data-ttu-id="d275d-705">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-705">Boolean</span></span>|<span data-ttu-id="d275d-706">Indica se os sevices com acesso podem se conectar e abrir arquivos em uma unidade USB.</span><span class="sxs-lookup"><span data-stu-id="d275d-706">Indicates if sevices with access can connect to and open files on a USB drive.</span></span> <span data-ttu-id="d275d-707">Disponível para dispositivos que executam iOS e iPadOS, versões 13.0 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="d275d-707">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="d275d-708">wifiPowerOnForced</span><span class="sxs-lookup"><span data-stu-id="d275d-708">wifiPowerOnForced</span></span>|<span data-ttu-id="d275d-709">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-709">Boolean</span></span>|<span data-ttu-id="d275d-710">Indica se o Wi-Fi permanece ou não, mesmo quando o dispositivo está no modo de avião.</span><span class="sxs-lookup"><span data-stu-id="d275d-710">Indicates whether or not Wi-Fi remains on, even when device is in airplane mode.</span></span> <span data-ttu-id="d275d-711">Disponível para dispositivos que executam iOS e iPadOS, versões 13.0 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="d275d-711">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="d275d-712">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="d275d-712">blockSystemAppRemoval</span></span>|<span data-ttu-id="d275d-713">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-713">Boolean</span></span>|<span data-ttu-id="d275d-714">Indica se a remoção ou não de aplicativos do sistema do dispositivo está bloqueada em um dispositivo supervisionado (iOS 11.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-714">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d275d-715">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="d275d-715">vpnBlockCreation</span></span>|<span data-ttu-id="d275d-716">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-716">Boolean</span></span>|<span data-ttu-id="d275d-717">Indica se a criação de configurações VPN está ou não bloqueada (iOS 11.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-717">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d275d-718">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-718">appRemovalBlocked</span></span>|<span data-ttu-id="d275d-719">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-719">Boolean</span></span>|<span data-ttu-id="d275d-720">Indica se a remoção de aplicativos é permitida.</span><span class="sxs-lookup"><span data-stu-id="d275d-720">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="d275d-721">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-721">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="d275d-722">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-722">Boolean</span></span>|<span data-ttu-id="d275d-723">Indica se a conexão com acessórios USB enquanto o dispositivo está bloqueado é permitida (iOS 11.4.1 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-723">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="d275d-724">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="d275d-724">passwordBlockAutoFill</span></span>|<span data-ttu-id="d275d-725">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-725">Boolean</span></span>|<span data-ttu-id="d275d-726">Indica se o recurso Senhas de Preenchimento Automático é permitido (iOS 12.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-726">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d275d-727">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="d275d-727">passwordBlockProximityRequests</span></span>|<span data-ttu-id="d275d-728">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-728">Boolean</span></span>|<span data-ttu-id="d275d-729">Indica se deve ou não bloquear a solicitação de senhas de dispositivos próximos (iOS 12.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-729">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d275d-730">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="d275d-730">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="d275d-731">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-731">Boolean</span></span>|<span data-ttu-id="d275d-732">Indica se deve ou não bloquear o compartilhamento de senhas com o recurso de senhas do AirDrop iOS 12.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-732">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d275d-733">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="d275d-733">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="d275d-734">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-734">Boolean</span></span>|<span data-ttu-id="d275d-735">Indica se o recurso Data e Hora "Definir Automaticamente" está habilitado e não pode ser desligado pelo usuário (iOS 12.0 e posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-735">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d275d-736">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="d275d-736">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="d275d-737">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-737">Boolean</span></span>|<span data-ttu-id="d275d-738">Indica se os aplicativos gerenciados podem ou não gravar contatos em contas de contatos não gerenciadas (iOS 12.0 e posteriores).</span><span class="sxs-lookup"><span data-stu-id="d275d-738">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d275d-739">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="d275d-739">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="d275d-740">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-740">Boolean</span></span>|<span data-ttu-id="d275d-741">Indica se aplicativos não gerenciados podem ou não ler de contas de contatos gerenciados (iOS 12.0 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-741">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="d275d-742">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="d275d-742">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="d275d-743">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-743">Boolean</span></span>|<span data-ttu-id="d275d-744">Indica se o usuário deve ou não bloquear a modificação da configuração de hotspot pessoal (iOS 12.2 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-744">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="d275d-745">continuousPathKeyboardBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-745">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="d275d-746">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-746">Boolean</span></span>|<span data-ttu-id="d275d-747">Indica se o teclado de caminho contínuo deve ou não ser bloqueado quando o dispositivo é supervisionado (iOS 13 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-747">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="d275d-748">findMyDeviceInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-748">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="d275d-749">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-749">Boolean</span></span>|<span data-ttu-id="d275d-750">Indica se o dispositivo deve ou não ser bloqueado quando o dispositivo é supervisionado (iOS 13 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-750">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="d275d-751">findMyFriendsInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-751">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="d275d-752">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-752">Boolean</span></span>|<span data-ttu-id="d275d-753">Indica se deve ou não bloquear Find My Friends quando o dispositivo é supervisionado (iOS 13 ou posterior).</span><span class="sxs-lookup"><span data-stu-id="d275d-753">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="d275d-754">iTunesBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-754">iTunesBlocked</span></span>|<span data-ttu-id="d275d-755">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-755">Boolean</span></span>|<span data-ttu-id="d275d-756">Indica se o aplicativo iTunes deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="d275d-756">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="d275d-757">Requer um dispositivo supervisionado para iOS 13 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-757">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d275d-758">sharedDeviceBlockTemporarySessions</span><span class="sxs-lookup"><span data-stu-id="d275d-758">sharedDeviceBlockTemporarySessions</span></span>|<span data-ttu-id="d275d-759">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-759">Boolean</span></span>|<span data-ttu-id="d275d-760">Indica se as sessões temporárias de iPads compartilhados (iOS 13.4 ou posteriores) são ou não bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d275d-760">Indicates whether or not to block temporary sessions on Shared iPads (iOS 13.4 or later).</span></span>|
|<span data-ttu-id="d275d-761">appClipsBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-761">appClipsBlocked</span></span>|<span data-ttu-id="d275d-762">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-762">Boolean</span></span>|<span data-ttu-id="d275d-763">Impede que um usuário adicione clipes de aplicativo e remova todos os Clipes de Aplicativo existentes no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d275d-763">Prevents a user from adding any App Clips and removes any existing App Clips on the device.</span></span>|
|<span data-ttu-id="d275d-764">applePersonalizedAdsBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-764">applePersonalizedAdsBlocked</span></span>|<span data-ttu-id="d275d-765">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-765">Boolean</span></span>|<span data-ttu-id="d275d-766">Limita a publicidade personalizada da Apple quando true.</span><span class="sxs-lookup"><span data-stu-id="d275d-766">Limits Apple personalized advertising when true.</span></span> <span data-ttu-id="d275d-767">Disponível no iOS 14 e posterior.</span><span class="sxs-lookup"><span data-stu-id="d275d-767">Available in iOS 14 and later.</span></span>|
|<span data-ttu-id="d275d-768">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-768">nfcBlocked</span></span>|<span data-ttu-id="d275d-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="d275d-769">Boolean</span></span>|<span data-ttu-id="d275d-770">Desabilite a NFC para impedir que dispositivos emparelhem com outros dispositivos habilitados para NFC.</span><span class="sxs-lookup"><span data-stu-id="d275d-770">Disable NFC to prevent devices from pairing with other NFC-enabled devices.</span></span> <span data-ttu-id="d275d-771">Disponível para dispositivos iOS/iPadOS que executam 14.2 e posteriores.</span><span class="sxs-lookup"><span data-stu-id="d275d-771">Available for iOS/iPadOS devices running 14.2 and later.</span></span>|
|<span data-ttu-id="d275d-772">autoUnlockBlocked</span><span class="sxs-lookup"><span data-stu-id="d275d-772">autoUnlockBlocked</span></span>|<span data-ttu-id="d275d-773">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-773">Boolean</span></span>|<span data-ttu-id="d275d-774">Impede que os usuários desbloqueiem seus dispositivos com o Apple Watch.</span><span class="sxs-lookup"><span data-stu-id="d275d-774">Blocks users from unlocking their device with Apple Watch.</span></span> <span data-ttu-id="d275d-775">Disponível para dispositivos que executam versões 14.5 e posteriores do iOS e iPadOS.</span><span class="sxs-lookup"><span data-stu-id="d275d-775">Available for devices running iOS and iPadOS versions 14.5 and later.</span></span>|
|<span data-ttu-id="d275d-776">unpairedExternalBootToRecoveryAllowed</span><span class="sxs-lookup"><span data-stu-id="d275d-776">unpairedExternalBootToRecoveryAllowed</span></span>|<span data-ttu-id="d275d-777">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-777">Boolean</span></span>|<span data-ttu-id="d275d-778">Permitir que os usuários inicialm dispositivos no modo de recuperação com dispositivos não organizados.</span><span class="sxs-lookup"><span data-stu-id="d275d-778">Allow users to boot devices into recovery mode with unpaired devices.</span></span> <span data-ttu-id="d275d-779">Disponível para dispositivos que executam versões 14.5 e posteriores do iOS e iPadOS.</span><span class="sxs-lookup"><span data-stu-id="d275d-779">Available for devices running iOS and iPadOS versions 14.5 and later.</span></span>|
|<span data-ttu-id="d275d-780">onDeviceOnlyDictationForced</span><span class="sxs-lookup"><span data-stu-id="d275d-780">onDeviceOnlyDictationForced</span></span>|<span data-ttu-id="d275d-781">Booleano</span><span class="sxs-lookup"><span data-stu-id="d275d-781">Boolean</span></span>|<span data-ttu-id="d275d-782">Desabilita conexões com servidores Siri para que os usuários não possam usar a Siri para ditar o texto.</span><span class="sxs-lookup"><span data-stu-id="d275d-782">Disables connections to Siri servers so that users can’t use Siri to dictate text.</span></span> <span data-ttu-id="d275d-783">Disponível para dispositivos que executam versões 14.5 e posteriores do iOS e iPadOS.</span><span class="sxs-lookup"><span data-stu-id="d275d-783">Available for devices running iOS and iPadOS versions 14.5 and later.</span></span>|
|<span data-ttu-id="d275d-784">kioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="d275d-784">kioskModeAppType</span></span>|[<span data-ttu-id="d275d-785">iosKioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="d275d-785">iosKioskModeAppType</span></span>](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|<span data-ttu-id="d275d-786">Tipo de aplicativo a ser executado no modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="d275d-786">Type of app to run in kiosk mode.</span></span> <span data-ttu-id="d275d-787">Os valores possíveis são: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span><span class="sxs-lookup"><span data-stu-id="d275d-787">Possible values are: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span></span>|



## <a name="response"></a><span data-ttu-id="d275d-788">Resposta</span><span class="sxs-lookup"><span data-stu-id="d275d-788">Response</span></span>
<span data-ttu-id="d275d-789">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d275d-789">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d275d-790">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d275d-790">Example</span></span>

### <a name="request"></a><span data-ttu-id="d275d-791">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d275d-791">Request</span></span>
<span data-ttu-id="d275d-792">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d275d-792">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 10776

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
  "nfcBlocked": true,
  "autoUnlockBlocked": true,
  "unpairedExternalBootToRecoveryAllowed": true,
  "onDeviceOnlyDictationForced": true,
  "kioskModeAppType": "appStoreApp"
}
```

### <a name="response"></a><span data-ttu-id="d275d-793">Resposta</span><span class="sxs-lookup"><span data-stu-id="d275d-793">Response</span></span>
<span data-ttu-id="d275d-p163">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d275d-p163">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10948

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
  "nfcBlocked": true,
  "autoUnlockBlocked": true,
  "unpairedExternalBootToRecoveryAllowed": true,
  "onDeviceOnlyDictationForced": true,
  "kioskModeAppType": "appStoreApp"
}
```




