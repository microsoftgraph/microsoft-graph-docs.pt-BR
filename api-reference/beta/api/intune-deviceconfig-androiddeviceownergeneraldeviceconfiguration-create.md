---
title: Criar androidDeviceOwnerGeneralDeviceConfiguration
description: Crie um novo objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7953d9b7e3607c33015106ab13be32ad55b5ae24
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130620"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="703f7-103">Criar androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="703f7-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="703f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="703f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="703f7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="703f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="703f7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="703f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="703f7-107">Crie um novo [objeto androidDeviceOwnerGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="703f7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="703f7-108">Prerequisites</span></span>
<span data-ttu-id="703f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="703f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="703f7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="703f7-111">Permission type</span></span>|<span data-ttu-id="703f7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="703f7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="703f7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="703f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="703f7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="703f7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="703f7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="703f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="703f7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="703f7-116">Not supported.</span></span>|
|<span data-ttu-id="703f7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="703f7-117">Application</span></span>|<span data-ttu-id="703f7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="703f7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="703f7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="703f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="703f7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="703f7-120">Request headers</span></span>
|<span data-ttu-id="703f7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="703f7-121">Header</span></span>|<span data-ttu-id="703f7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="703f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="703f7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="703f7-123">Authorization</span></span>|<span data-ttu-id="703f7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="703f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="703f7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="703f7-125">Accept</span></span>|<span data-ttu-id="703f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="703f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="703f7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="703f7-127">Request body</span></span>
<span data-ttu-id="703f7-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="703f7-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="703f7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="703f7-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="703f7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="703f7-130">Property</span></span>|<span data-ttu-id="703f7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="703f7-131">Type</span></span>|<span data-ttu-id="703f7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="703f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="703f7-133">id</span><span class="sxs-lookup"><span data-stu-id="703f7-133">id</span></span>|<span data-ttu-id="703f7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="703f7-134">String</span></span>|<span data-ttu-id="703f7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="703f7-135">Key of the entity.</span></span> <span data-ttu-id="703f7-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="703f7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="703f7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="703f7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="703f7-138">DateTimeOffset</span></span>|<span data-ttu-id="703f7-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="703f7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="703f7-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="703f7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="703f7-141">roleScopeTagIds</span></span>|<span data-ttu-id="703f7-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="703f7-142">String collection</span></span>|<span data-ttu-id="703f7-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="703f7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="703f7-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="703f7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="703f7-145">supportsScopeTags</span></span>|<span data-ttu-id="703f7-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-146">Boolean</span></span>|<span data-ttu-id="703f7-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="703f7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="703f7-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="703f7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="703f7-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="703f7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="703f7-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="703f7-150">This property is read-only.</span></span> <span data-ttu-id="703f7-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="703f7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="703f7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="703f7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="703f7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="703f7-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="703f7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="703f7-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="703f7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="703f7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="703f7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="703f7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="703f7-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="703f7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="703f7-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="703f7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="703f7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="703f7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="703f7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="703f7-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="703f7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="703f7-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="703f7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="703f7-164">createdDateTime</span></span>|<span data-ttu-id="703f7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="703f7-165">DateTimeOffset</span></span>|<span data-ttu-id="703f7-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="703f7-166">DateTime the object was created.</span></span> <span data-ttu-id="703f7-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="703f7-168">descrição</span><span class="sxs-lookup"><span data-stu-id="703f7-168">description</span></span>|<span data-ttu-id="703f7-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="703f7-169">String</span></span>|<span data-ttu-id="703f7-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="703f7-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="703f7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="703f7-172">displayName</span></span>|<span data-ttu-id="703f7-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="703f7-173">String</span></span>|<span data-ttu-id="703f7-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="703f7-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="703f7-176">versão</span><span class="sxs-lookup"><span data-stu-id="703f7-176">version</span></span>|<span data-ttu-id="703f7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-177">Int32</span></span>|<span data-ttu-id="703f7-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-178">Version of the device configuration.</span></span> <span data-ttu-id="703f7-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="703f7-180">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="703f7-180">accountsBlockModification</span></span>|<span data-ttu-id="703f7-181">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-181">Boolean</span></span>|<span data-ttu-id="703f7-182">Indica se a adição ou remoção de contas está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="703f7-182">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="703f7-183">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="703f7-183">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="703f7-184">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-184">Boolean</span></span>|<span data-ttu-id="703f7-185">Indica se o usuário tem ou não permissão para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="703f7-185">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="703f7-186">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="703f7-186">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="703f7-187">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="703f7-187">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="703f7-188">Indica o valor da política de atualização automática do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="703f7-188">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="703f7-189">Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="703f7-189">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="703f7-190">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="703f7-190">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="703f7-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="703f7-191">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="703f7-192">Indica a política de permissão para solicitações de permissões de tempo de execução se uma não for definida especificamente para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="703f7-192">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="703f7-193">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="703f7-193">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="703f7-194">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="703f7-194">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="703f7-195">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-195">Boolean</span></span>|<span data-ttu-id="703f7-196">Se todos os aplicativos devem ou não ignorar as dicas de uso pela primeira vez que eles possam ter adicionado.</span><span class="sxs-lookup"><span data-stu-id="703f7-196">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="703f7-197">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="703f7-197">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="703f7-198">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-198">Boolean</span></span>|<span data-ttu-id="703f7-199">Indica se um usuário deve ou não bloquear a configuração do bluetooth.</span><span class="sxs-lookup"><span data-stu-id="703f7-199">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="703f7-200">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="703f7-200">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="703f7-201">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-201">Boolean</span></span>|<span data-ttu-id="703f7-202">Indica se um usuário deve ou não bloquear o compartilhamento de contatos via bluetooth.</span><span class="sxs-lookup"><span data-stu-id="703f7-202">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="703f7-203">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-203">cameraBlocked</span></span>|<span data-ttu-id="703f7-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="703f7-204">Boolean</span></span>|<span data-ttu-id="703f7-205">Indica se o uso da câmera deve ou não ser desabilitado.</span><span class="sxs-lookup"><span data-stu-id="703f7-205">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="703f7-206">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="703f7-206">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="703f7-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="703f7-207">Boolean</span></span>|<span data-ttu-id="703f7-208">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="703f7-208">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="703f7-209">certificateCredentialConfigurationDisabled</span><span class="sxs-lookup"><span data-stu-id="703f7-209">certificateCredentialConfigurationDisabled</span></span>|<span data-ttu-id="703f7-210">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-210">Boolean</span></span>|<span data-ttu-id="703f7-211">Indica se os usuários podem ou não bloquear qualquer configuração de credencial de certificado.</span><span class="sxs-lookup"><span data-stu-id="703f7-211">Indicates whether or not to block users from any certificate credential configuration.</span></span>|
|<span data-ttu-id="703f7-212">microsoftLauncherConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="703f7-212">microsoftLauncherConfigurationEnabled</span></span>|<span data-ttu-id="703f7-213">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-213">Boolean</span></span>|<span data-ttu-id="703f7-214">Indica se você deseja ou não configurar o Microsoft Launcher.</span><span class="sxs-lookup"><span data-stu-id="703f7-214">Indicates whether or not to you want configure Microsoft Launcher.</span></span>|
|<span data-ttu-id="703f7-215">microsoftLauncherCustomWallpaperEnabled</span><span class="sxs-lookup"><span data-stu-id="703f7-215">microsoftLauncherCustomWallpaperEnabled</span></span>|<span data-ttu-id="703f7-216">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-216">Boolean</span></span>|<span data-ttu-id="703f7-217">Indica se o papel de parede deve ou não ser configurada nos dispositivos direcionados.</span><span class="sxs-lookup"><span data-stu-id="703f7-217">Indicates whether or not to configure the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="703f7-218">microsoftLauncherCustomWallpaperImageUrl</span><span class="sxs-lookup"><span data-stu-id="703f7-218">microsoftLauncherCustomWallpaperImageUrl</span></span>|<span data-ttu-id="703f7-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="703f7-219">String</span></span>|<span data-ttu-id="703f7-220">Indica a URL do arquivo de imagem a ser usado como papel de parede nos dispositivos direcionados.</span><span class="sxs-lookup"><span data-stu-id="703f7-220">Indicates the URL for the image file to use as the wallpaper on the targeted devices.</span></span>|
|<span data-ttu-id="703f7-221">microsoftLauncherCustomWallpaperAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="703f7-221">microsoftLauncherCustomWallpaperAllowUserModification</span></span>|<span data-ttu-id="703f7-222">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-222">Boolean</span></span>|<span data-ttu-id="703f7-223">Indica se o usuário pode ou não modificar o papel de parede para personalizar seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-223">Indicates whether or not the user can modify the wallpaper to personalize their device.</span></span>|
|<span data-ttu-id="703f7-224">microsoftLauncherFeedEnabled</span><span class="sxs-lookup"><span data-stu-id="703f7-224">microsoftLauncherFeedEnabled</span></span>|<span data-ttu-id="703f7-225">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-225">Boolean</span></span>|<span data-ttu-id="703f7-226">Indica se você deseja ou não habilitar o feed do launcher no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-226">Indicates whether or not you want to enable the launcher feed on the device.</span></span>|
|<span data-ttu-id="703f7-227">microsoftLauncherFeedAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="703f7-227">microsoftLauncherFeedAllowUserModification</span></span>|<span data-ttu-id="703f7-228">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-228">Boolean</span></span>|<span data-ttu-id="703f7-229">Indica se o usuário pode ou não modificar o feed do launcher no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-229">Indicates whether or not the user can modify the launcher feed on the device.</span></span>|
|<span data-ttu-id="703f7-230">microsoftLauncherDockPresenceConfiguration</span><span class="sxs-lookup"><span data-stu-id="703f7-230">microsoftLauncherDockPresenceConfiguration</span></span>|[<span data-ttu-id="703f7-231">microsoftLauncherDockPresence</span><span class="sxs-lookup"><span data-stu-id="703f7-231">microsoftLauncherDockPresence</span></span>](../resources/intune-deviceconfig-microsoftlauncherdockpresence.md)|<span data-ttu-id="703f7-232">Indica se você deseja ou não configurar o encaixe do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-232">Indicates whether or not you want to configure the device dock.</span></span> <span data-ttu-id="703f7-233">Os valores possíveis são: `notConfigured`, `show`, `hide`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="703f7-233">Possible values are: `notConfigured`, `show`, `hide`, `disabled`.</span></span>|
|<span data-ttu-id="703f7-234">microsoftLauncherDockPresenceAllowUserModification</span><span class="sxs-lookup"><span data-stu-id="703f7-234">microsoftLauncherDockPresenceAllowUserModification</span></span>|<span data-ttu-id="703f7-235">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-235">Boolean</span></span>|<span data-ttu-id="703f7-236">Indica se o usuário pode ou não modificar a configuração do encaixe do dispositivo no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-236">Indicates whether or not the user can modify the device dock configuration on the device.</span></span>|
|<span data-ttu-id="703f7-237">microsoftLauncherSearchBarPlacementConfiguration</span><span class="sxs-lookup"><span data-stu-id="703f7-237">microsoftLauncherSearchBarPlacementConfiguration</span></span>|[<span data-ttu-id="703f7-238">microsoftLauncherSearchBarPlacement</span><span class="sxs-lookup"><span data-stu-id="703f7-238">microsoftLauncherSearchBarPlacement</span></span>](../resources/intune-deviceconfig-microsoftlaunchersearchbarplacement.md)|<span data-ttu-id="703f7-239">Indica a configuração de posicionamento da barra de pesquisa no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-239">Indicates the search bar placement configuration on the device.</span></span> <span data-ttu-id="703f7-240">Os valores possíveis são: `notConfigured`, `top`, `bottom`, `hide`.</span><span class="sxs-lookup"><span data-stu-id="703f7-240">Possible values are: `notConfigured`, `top`, `bottom`, `hide`.</span></span>|
|<span data-ttu-id="703f7-241">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="703f7-241">enrollmentProfile</span></span>|[<span data-ttu-id="703f7-242">androidDeviceOwnerEnrollmentProfileType</span><span class="sxs-lookup"><span data-stu-id="703f7-242">androidDeviceOwnerEnrollmentProfileType</span></span>](../resources/intune-deviceconfig-androiddeviceownerenrollmentprofiletype.md)|<span data-ttu-id="703f7-243">Indica qual perfil de registro você deseja configurar.</span><span class="sxs-lookup"><span data-stu-id="703f7-243">Indicates which enrollment profile you want to configure.</span></span> <span data-ttu-id="703f7-244">Os valores possíveis são: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span><span class="sxs-lookup"><span data-stu-id="703f7-244">Possible values are: `notConfigured`, `dedicatedDevice`, `fullyManaged`.</span></span>|
|<span data-ttu-id="703f7-245">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-245">dataRoamingBlocked</span></span>|<span data-ttu-id="703f7-246">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-246">Boolean</span></span>|<span data-ttu-id="703f7-247">Indica se um usuário deve ou não bloquear o roaming de dados.</span><span class="sxs-lookup"><span data-stu-id="703f7-247">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="703f7-248">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-248">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="703f7-249">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-249">Boolean</span></span>|<span data-ttu-id="703f7-250">Indica se o usuário deve ou não bloquear a alteração manual da data ou hora no dispositivo</span><span class="sxs-lookup"><span data-stu-id="703f7-250">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="703f7-251">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="703f7-251">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="703f7-252">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="703f7-252">String collection</span></span>|<span data-ttu-id="703f7-253">Lista de emails de conta do Google que serão necessários para autenticar depois que um dispositivo for redefinido de fábrica antes de poder ser definido.</span><span class="sxs-lookup"><span data-stu-id="703f7-253">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="703f7-254">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-254">factoryResetBlocked</span></span>|<span data-ttu-id="703f7-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="703f7-255">Boolean</span></span>|<span data-ttu-id="703f7-256">Indica se a opção de redefinição de fábrica nas configurações está desabilitada ou não.</span><span class="sxs-lookup"><span data-stu-id="703f7-256">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="703f7-257">globalProxy</span><span class="sxs-lookup"><span data-stu-id="703f7-257">globalProxy</span></span>|[<span data-ttu-id="703f7-258">androidDeviceOwnerGlobalProxy</span><span class="sxs-lookup"><span data-stu-id="703f7-258">androidDeviceOwnerGlobalProxy</span></span>](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)|<span data-ttu-id="703f7-259">O proxy é definido diretamente com host, porta e hosts excluídos.</span><span class="sxs-lookup"><span data-stu-id="703f7-259">Proxy is set up directly with host, port and excluded hosts.</span></span>|
|<span data-ttu-id="703f7-260">googleAccountsBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-260">googleAccountsBlocked</span></span>|<span data-ttu-id="703f7-261">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-261">Boolean</span></span>|<span data-ttu-id="703f7-262">Indica se as contas do Google serão ou não bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="703f7-262">Indicates whether or not google accounts will be blocked.</span></span>|
|<span data-ttu-id="703f7-263">kioskCustomizationDeviceSettingsBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-263">kioskCustomizationDeviceSettingsBlocked</span></span>|<span data-ttu-id="703f7-264">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-264">Boolean</span></span>|<span data-ttu-id="703f7-265">Indica se um usuário pode acessar o aplicativo Configurações do dispositivo enquanto estiver no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-265">Indicates whether a user can access the device's Settings app while in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-266">kioskCustomizationPowerButtonActionsBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-266">kioskCustomizationPowerButtonActionsBlocked</span></span>|<span data-ttu-id="703f7-267">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-267">Boolean</span></span>|<span data-ttu-id="703f7-268">Se o menu de energia é mostrado quando um usuário pressiona por muito tempo o botão Ligar de um dispositivo no Modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-268">Whether the power menu is shown when a user long presses the Power button of a device in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-269">kioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="703f7-269">kioskCustomizationStatusBar</span></span>|[<span data-ttu-id="703f7-270">androidDeviceOwnerKioskCustomizationStatusBar</span><span class="sxs-lookup"><span data-stu-id="703f7-270">androidDeviceOwnerKioskCustomizationStatusBar</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationstatusbar.md)|<span data-ttu-id="703f7-271">Indica se as informações e notificações do sistema estão desabilitadas no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-271">Indicates whether system info and notifications are disabled in Kiosk Mode.</span></span> <span data-ttu-id="703f7-272">Os valores possíveis são: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span><span class="sxs-lookup"><span data-stu-id="703f7-272">Possible values are: `notConfigured`, `notificationsAndSystemInfoEnabled`, `systemInfoOnly`.</span></span>|
|<span data-ttu-id="703f7-273">kioskCustomizationSystemErrorWarnings</span><span class="sxs-lookup"><span data-stu-id="703f7-273">kioskCustomizationSystemErrorWarnings</span></span>|<span data-ttu-id="703f7-274">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-274">Boolean</span></span>|<span data-ttu-id="703f7-275">Indica se as caixas de diálogo de erro do sistema para aplicativos inativos ou não responsivos são mostradas no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-275">Indicates whether system error dialogs for crashed or unresponsive apps are shown in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-276">kioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="703f7-276">kioskCustomizationSystemNavigation</span></span>|[<span data-ttu-id="703f7-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span><span class="sxs-lookup"><span data-stu-id="703f7-277">androidDeviceOwnerKioskCustomizationSystemNavigation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskcustomizationsystemnavigation.md)|<span data-ttu-id="703f7-278">Indica quais recursos de navegação estão habilitados no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-278">Indicates which navigation features are enabled in Kiosk Mode.</span></span> <span data-ttu-id="703f7-279">Os valores possíveis são: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span><span class="sxs-lookup"><span data-stu-id="703f7-279">Possible values are: `notConfigured`, `navigationEnabled`, `homeButtonOnly`.</span></span>|
|<span data-ttu-id="703f7-280">kioskModeScreenSaverConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="703f7-280">kioskModeScreenSaverConfigurationEnabled</span></span>|<span data-ttu-id="703f7-281">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-281">Boolean</span></span>|<span data-ttu-id="703f7-282">Se deve ou não habilitar o modo de economia de tela ou não no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-282">Whether or not to enable screen saver mode or not in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-283">kioskModeScreenSaverImageUrl</span><span class="sxs-lookup"><span data-stu-id="703f7-283">kioskModeScreenSaverImageUrl</span></span>|<span data-ttu-id="703f7-284">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="703f7-284">String</span></span>|<span data-ttu-id="703f7-285">URL de uma imagem que será o protetor de tela do dispositivo no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-285">URL for an image that will be the device's screen saver in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-286">kioskModeScreenSaverDisplayTimeInSeconds</span><span class="sxs-lookup"><span data-stu-id="703f7-286">kioskModeScreenSaverDisplayTimeInSeconds</span></span>|<span data-ttu-id="703f7-287">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-287">Int32</span></span>|<span data-ttu-id="703f7-288">O número de segundos em que o dispositivo exibirá o protetor de tela no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-288">The number of seconds that the device will display the screen saver for in Kiosk Mode.</span></span> <span data-ttu-id="703f7-289">Valores válidos de 0 a 9999999</span><span class="sxs-lookup"><span data-stu-id="703f7-289">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="703f7-290">kioskModeScreenSaverStartDelayInSeconds</span><span class="sxs-lookup"><span data-stu-id="703f7-290">kioskModeScreenSaverStartDelayInSeconds</span></span>|<span data-ttu-id="703f7-291">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-291">Int32</span></span>|<span data-ttu-id="703f7-292">O número de segundos em que o dispositivo precisa estar inativo para antes que a economia de tela seja mostrada no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-292">The number of seconds the device needs to be inactive for before the screen saver is shown in Kiosk Mode.</span></span> <span data-ttu-id="703f7-293">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="703f7-293">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="703f7-294">kioskModeScreenSaverDetectMediaDisabled</span><span class="sxs-lookup"><span data-stu-id="703f7-294">kioskModeScreenSaverDetectMediaDisabled</span></span>|<span data-ttu-id="703f7-295">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-295">Boolean</span></span>|<span data-ttu-id="703f7-296">Se a tela do dispositivo deve ou não mostrar o protetor de tela se o áudio/vídeo estiver sendo exibido no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-296">Whether or not the device screen should show the screen saver if audio/video is playing in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-297">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="703f7-297">kioskModeApps</span></span>|<span data-ttu-id="703f7-298">Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-298">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="703f7-299">Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-299">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="703f7-300">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="703f7-300">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="703f7-301">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="703f7-301">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="703f7-302">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="703f7-302">String</span></span>|<span data-ttu-id="703f7-303">URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-303">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-304">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="703f7-304">kioskModeExitCode</span></span>|<span data-ttu-id="703f7-305">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="703f7-305">String</span></span>|<span data-ttu-id="703f7-306">Código de saída para permitir que um usuário escape do Modo Quiosque quando o dispositivo estiver no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-306">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-307">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="703f7-307">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="703f7-308">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-308">Boolean</span></span>|<span data-ttu-id="703f7-309">Se será exibido ou não um botão home virtual quando o dispositivo estiver no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-309">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-310">kioskModeVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="703f7-310">kioskModeVirtualHomeButtonType</span></span>|[<span data-ttu-id="703f7-311">androidDeviceOwnerVirtualHomeButtonType</span><span class="sxs-lookup"><span data-stu-id="703f7-311">androidDeviceOwnerVirtualHomeButtonType</span></span>](../resources/intune-deviceconfig-androiddeviceownervirtualhomebuttontype.md)|<span data-ttu-id="703f7-312">Indica se o botão home virtual é um botão de passar o dedo para cima ou um botão home flutuante.</span><span class="sxs-lookup"><span data-stu-id="703f7-312">Indicates whether the virtual home button is a swipe up home button or a floating home button.</span></span> <span data-ttu-id="703f7-313">Os valores possíveis são: `notConfigured`, `swipeUp`, `floating`.</span><span class="sxs-lookup"><span data-stu-id="703f7-313">Possible values are: `notConfigured`, `swipeUp`, `floating`.</span></span>|
|<span data-ttu-id="703f7-314">kioskModeBluetoothConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="703f7-314">kioskModeBluetoothConfigurationEnabled</span></span>|<span data-ttu-id="703f7-315">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-315">Boolean</span></span>|<span data-ttu-id="703f7-316">Se um usuário pode ou não configurar Bluetooth configurações no Modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-316">Whether or not to allow a user to configure Bluetooth settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-317">kioskModeWiFiConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="703f7-317">kioskModeWiFiConfigurationEnabled</span></span>|<span data-ttu-id="703f7-318">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-318">Boolean</span></span>|<span data-ttu-id="703f7-319">Se um usuário pode ou não configurar Wi-Fi configurações no Modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-319">Whether or not to allow a user to configure Wi-Fi settings in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-320">kioskModeFlashlightConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="703f7-320">kioskModeFlashlightConfigurationEnabled</span></span>|<span data-ttu-id="703f7-321">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-321">Boolean</span></span>|<span data-ttu-id="703f7-322">Se um usuário pode ou não usar a lanterna no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-322">Whether or not to allow a user to use the flashlight in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-323">kioskModeMediaVolumeConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="703f7-323">kioskModeMediaVolumeConfigurationEnabled</span></span>|<span data-ttu-id="703f7-324">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-324">Boolean</span></span>|<span data-ttu-id="703f7-325">Se um usuário pode ou não alterar o volume de mídia no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-325">Whether or not to allow a user to change the media volume in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-326">kioskModeShowDeviceInfo</span><span class="sxs-lookup"><span data-stu-id="703f7-326">kioskModeShowDeviceInfo</span></span>|<span data-ttu-id="703f7-327">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-327">Boolean</span></span>|<span data-ttu-id="703f7-328">Se um usuário pode ou não acessar informações básicas do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-328">Whether or not to allow a user to access basic device information.</span></span>|
|<span data-ttu-id="703f7-329">kioskModeManagedSettingsEntryDisabled</span><span class="sxs-lookup"><span data-stu-id="703f7-329">kioskModeManagedSettingsEntryDisabled</span></span>|<span data-ttu-id="703f7-330">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-330">Boolean</span></span>|<span data-ttu-id="703f7-331">Se será exibido ou não o ponto de entrada Configurações Gerenciadas na tela inicial gerenciada no Modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-331">Whether or not to display the Managed Settings entry point on the managed home screen in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-332">kioskModeDebugMenuEasyAccessEnabled</span><span class="sxs-lookup"><span data-stu-id="703f7-332">kioskModeDebugMenuEasyAccessEnabled</span></span>|<span data-ttu-id="703f7-333">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-333">Boolean</span></span>|<span data-ttu-id="703f7-334">Se um usuário pode ou não permitir acesso fácil ao menu de depuração no Modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-334">Whether or not to allow a user to easy access to the debug menu in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-335">kioskModeShowAppNotificationBadge</span><span class="sxs-lookup"><span data-stu-id="703f7-335">kioskModeShowAppNotificationBadge</span></span>|<span data-ttu-id="703f7-336">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-336">Boolean</span></span>|<span data-ttu-id="703f7-337">Se os selos de notificação do aplicativo serão exibidos ou não no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-337">Whether or not to display application notification badges in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-338">kioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="703f7-338">kioskModeScreenOrientation</span></span>|[<span data-ttu-id="703f7-339">androidDeviceOwnerKioskModeScreenOrientation</span><span class="sxs-lookup"><span data-stu-id="703f7-339">androidDeviceOwnerKioskModeScreenOrientation</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodescreenorientation.md)|<span data-ttu-id="703f7-340">Configuração de orientação de tela para tela inicial gerenciada no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-340">Screen orientation configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="703f7-341">Os valores possíveis são: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span><span class="sxs-lookup"><span data-stu-id="703f7-341">Possible values are: `notConfigured`, `portrait`, `landscape`, `autoRotate`.</span></span>|
|<span data-ttu-id="703f7-342">kioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="703f7-342">kioskModeIconSize</span></span>|[<span data-ttu-id="703f7-343">androidDeviceOwnerKioskModeIconSize</span><span class="sxs-lookup"><span data-stu-id="703f7-343">androidDeviceOwnerKioskModeIconSize</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodeiconsize.md)|<span data-ttu-id="703f7-344">Configuração do tamanho do ícone para a tela inicial gerenciada no Modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-344">Icon size configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="703f7-345">Os possíveis valores são: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span><span class="sxs-lookup"><span data-stu-id="703f7-345">Possible values are: `notConfigured`, `smallest`, `small`, `regular`, `large`, `largest`.</span></span>|
|<span data-ttu-id="703f7-346">kioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="703f7-346">kioskModeFolderIcon</span></span>|[<span data-ttu-id="703f7-347">androidDeviceOwnerKioskModeFolderIcon</span><span class="sxs-lookup"><span data-stu-id="703f7-347">androidDeviceOwnerKioskModeFolderIcon</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodefoldericon.md)|<span data-ttu-id="703f7-348">Configuração do ícone de pasta para a tela inicial gerenciada no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-348">Folder icon configuration for managed home screen in Kiosk Mode.</span></span> <span data-ttu-id="703f7-349">Os valores possíveis são: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span><span class="sxs-lookup"><span data-stu-id="703f7-349">Possible values are: `notConfigured`, `darkSquare`, `darkCircle`, `lightSquare`, `lightCircle`.</span></span>|
|<span data-ttu-id="703f7-350">kioskModeWifiAllowedSsids</span><span class="sxs-lookup"><span data-stu-id="703f7-350">kioskModeWifiAllowedSsids</span></span>|<span data-ttu-id="703f7-351">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="703f7-351">String collection</span></span>|<span data-ttu-id="703f7-352">O conjunto restrito de SSIDs WIFI disponíveis para o usuário configurar no Modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-352">The restricted set of WIFI SSIDs available for the user to configure in Kiosk Mode.</span></span> <span data-ttu-id="703f7-353">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="703f7-353">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="703f7-354">kioskModeAppOrderEnabled</span><span class="sxs-lookup"><span data-stu-id="703f7-354">kioskModeAppOrderEnabled</span></span>|<span data-ttu-id="703f7-355">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-355">Boolean</span></span>|<span data-ttu-id="703f7-356">Se é ou não para habilitar a ordenação de aplicativos no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-356">Whether or not to enable app ordering in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-357">kioskModeAppsInFolderOrderedByName</span><span class="sxs-lookup"><span data-stu-id="703f7-357">kioskModeAppsInFolderOrderedByName</span></span>|<span data-ttu-id="703f7-358">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-358">Boolean</span></span>|<span data-ttu-id="703f7-359">Se deve ou não alfabéticar aplicativos em uma pasta no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-359">Whether or not to alphabetize applications within a folder in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-360">kioskModeGridHeight</span><span class="sxs-lookup"><span data-stu-id="703f7-360">kioskModeGridHeight</span></span>|<span data-ttu-id="703f7-361">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-361">Int32</span></span>|<span data-ttu-id="703f7-362">Número de linhas para grade da Tela Inicial Gerenciada com a ordenação de aplicativos habilitada no Modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-362">Number of rows for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="703f7-363">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="703f7-363">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="703f7-364">kioskModeGridWidth</span><span class="sxs-lookup"><span data-stu-id="703f7-364">kioskModeGridWidth</span></span>|<span data-ttu-id="703f7-365">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-365">Int32</span></span>|<span data-ttu-id="703f7-366">Número de colunas para grade da Tela Inicial Gerenciada com a ordenação de aplicativos habilitada no Modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-366">Number of columns for Managed Home Screen grid with app ordering enabled in Kiosk Mode.</span></span> <span data-ttu-id="703f7-367">Valores válidos de 1 a 9999999</span><span class="sxs-lookup"><span data-stu-id="703f7-367">Valid values 1 to 9999999</span></span>|
|<span data-ttu-id="703f7-368">kioskModeLockHomeScreen</span><span class="sxs-lookup"><span data-stu-id="703f7-368">kioskModeLockHomeScreen</span></span>|<span data-ttu-id="703f7-369">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-369">Boolean</span></span>|<span data-ttu-id="703f7-370">Se deve ou não bloquear a tela inicial para o usuário final no Modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-370">Whether or not to lock home screen to the end user in Kiosk Mode.</span></span>|
|<span data-ttu-id="703f7-371">kioskModeManagedFolders</span><span class="sxs-lookup"><span data-stu-id="703f7-371">kioskModeManagedFolders</span></span>|<span data-ttu-id="703f7-372">[coleção androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-372">[androidDeviceOwnerKioskModeManagedFolder](../resources/intune-deviceconfig-androiddeviceownerkioskmodemanagedfolder.md) collection</span></span>|<span data-ttu-id="703f7-373">Uma lista de pastas gerenciadas para um dispositivo no modo Quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-373">A list of managed folders for a device in Kiosk Mode.</span></span> <span data-ttu-id="703f7-374">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="703f7-374">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="703f7-375">kioskModeAppPositions</span><span class="sxs-lookup"><span data-stu-id="703f7-375">kioskModeAppPositions</span></span>|<span data-ttu-id="703f7-376">[coleção androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-376">[androidDeviceOwnerKioskModeAppPositionItem](../resources/intune-deviceconfig-androiddeviceownerkioskmodeapppositionitem.md) collection</span></span>|<span data-ttu-id="703f7-377">A ordenação de itens na Tela Inicial Gerenciada do Modo quiosque.</span><span class="sxs-lookup"><span data-stu-id="703f7-377">The ordering of items on Kiosk Mode Managed Home Screen.</span></span> <span data-ttu-id="703f7-378">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="703f7-378">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="703f7-379">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="703f7-379">microphoneForceMute</span></span>|<span data-ttu-id="703f7-380">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-380">Boolean</span></span>|<span data-ttu-id="703f7-381">Indica se o microfone deve ou não ser bloqueado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-381">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="703f7-382">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="703f7-382">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="703f7-383">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-383">Boolean</span></span>|<span data-ttu-id="703f7-384">Indica se o dispositivo permitirá ou não a conexão a uma conexão de rede temporária no momento da inicialização.</span><span class="sxs-lookup"><span data-stu-id="703f7-384">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="703f7-385">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="703f7-385">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="703f7-386">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-386">Boolean</span></span>|<span data-ttu-id="703f7-387">Indica se o raio de saída NFC deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="703f7-387">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="703f7-388">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="703f7-388">passwordBlockKeyguard</span></span>|<span data-ttu-id="703f7-389">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-389">Boolean</span></span>|<span data-ttu-id="703f7-390">Indica se o keyguard está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="703f7-390">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="703f7-391">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="703f7-391">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="703f7-392">[coleção androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-392">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="703f7-393">Lista de recursos de proteção de chave do dispositivo a ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="703f7-393">List of device keyguard features to block.</span></span> <span data-ttu-id="703f7-394">Essa coleção pode conter um máximo de 7 elementos.</span><span class="sxs-lookup"><span data-stu-id="703f7-394">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="703f7-395">Os valores possíveis são: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="703f7-395">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="703f7-396">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="703f7-396">passwordExpirationDays</span></span>|<span data-ttu-id="703f7-397">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-397">Int32</span></span>|<span data-ttu-id="703f7-398">Indica a quantidade de tempo em que uma senha pode ser definida antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="703f7-398">Indicates the amount of time that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="703f7-399">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="703f7-399">Valid values 1 to 365</span></span>|
|<span data-ttu-id="703f7-400">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="703f7-400">passwordMinimumLength</span></span>|<span data-ttu-id="703f7-401">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-401">Int32</span></span>|<span data-ttu-id="703f7-402">Indica o tamanho mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-402">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="703f7-403">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-403">Valid values 4 to 16</span></span>|
|<span data-ttu-id="703f7-404">passwordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="703f7-404">passwordMinimumLetterCharacters</span></span>|<span data-ttu-id="703f7-405">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-405">Int32</span></span>|<span data-ttu-id="703f7-406">Indica o número mínimo de caracteres de letra necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-406">Indicates the minimum number of letter characters required for device password.</span></span> <span data-ttu-id="703f7-407">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-407">Valid values 1 to 16</span></span>|
|<span data-ttu-id="703f7-408">passwordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="703f7-408">passwordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="703f7-409">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-409">Int32</span></span>|<span data-ttu-id="703f7-410">Indica o número mínimo de caracteres de caixa inferiores necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-410">Indicates the minimum number of lower case characters required for device password.</span></span> <span data-ttu-id="703f7-411">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-411">Valid values 1 to 16</span></span>|
|<span data-ttu-id="703f7-412">passwordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="703f7-412">passwordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="703f7-413">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-413">Int32</span></span>|<span data-ttu-id="703f7-414">Indica o número mínimo de caracteres que não são letras necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-414">Indicates the minimum number of non-letter characters required for device password.</span></span> <span data-ttu-id="703f7-415">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-415">Valid values 1 to 16</span></span>|
|<span data-ttu-id="703f7-416">passwordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="703f7-416">passwordMinimumNumericCharacters</span></span>|<span data-ttu-id="703f7-417">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-417">Int32</span></span>|<span data-ttu-id="703f7-418">Indica o número mínimo de caracteres numéricos necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-418">Indicates the minimum number of numeric characters required for device password.</span></span> <span data-ttu-id="703f7-419">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-419">Valid values 1 to 16</span></span>|
|<span data-ttu-id="703f7-420">passwordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="703f7-420">passwordMinimumSymbolCharacters</span></span>|<span data-ttu-id="703f7-421">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-421">Int32</span></span>|<span data-ttu-id="703f7-422">Indica o número mínimo de caracteres de símbolo necessário para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-422">Indicates the minimum number of symbol characters required for device password.</span></span> <span data-ttu-id="703f7-423">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-423">Valid values 1 to 16</span></span>|
|<span data-ttu-id="703f7-424">passwordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="703f7-424">passwordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="703f7-425">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-425">Int32</span></span>|<span data-ttu-id="703f7-426">Indica o número mínimo de caracteres de letras maiúsculas de maiúsculas e médios necessários para a senha do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-426">Indicates the minimum number of upper case letter characters required for device password.</span></span> <span data-ttu-id="703f7-427">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-427">Valid values 1 to 16</span></span>|
|<span data-ttu-id="703f7-428">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="703f7-428">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="703f7-429">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-429">Int32</span></span>|<span data-ttu-id="703f7-430">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="703f7-430">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="703f7-431">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="703f7-431">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="703f7-432">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-432">Int32</span></span>|<span data-ttu-id="703f7-433">Indica o tamanho do histórico de senhas, em que o usuário não poderá inserir uma nova senha que seja a mesma de qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="703f7-433">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="703f7-434">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="703f7-434">Valid values 0 to 24</span></span>|
|<span data-ttu-id="703f7-435">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="703f7-435">passwordRequiredType</span></span>|[<span data-ttu-id="703f7-436">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="703f7-436">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="703f7-437">Indica a qualidade mínima de senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-437">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="703f7-438">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="703f7-438">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="703f7-439">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="703f7-439">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="703f7-440">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-440">Int32</span></span>|<span data-ttu-id="703f7-441">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="703f7-441">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="703f7-442">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="703f7-442">Valid values 4 to 11</span></span>|
|<span data-ttu-id="703f7-443">playStoreMode</span><span class="sxs-lookup"><span data-stu-id="703f7-443">playStoreMode</span></span>|[<span data-ttu-id="703f7-444">androidDeviceOwnerPlayStoreMode</span><span class="sxs-lookup"><span data-stu-id="703f7-444">androidDeviceOwnerPlayStoreMode</span></span>](../resources/intune-deviceconfig-androiddeviceownerplaystoremode.md)|<span data-ttu-id="703f7-445">Indica o modo Play Store do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-445">Indicates the Play Store mode of the device.</span></span> <span data-ttu-id="703f7-446">Os valores possíveis são: `notConfigured`, `allowList`, `blockList`.</span><span class="sxs-lookup"><span data-stu-id="703f7-446">Possible values are: `notConfigured`, `allowList`, `blockList`.</span></span>|
|<span data-ttu-id="703f7-447">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-447">safeBootBlocked</span></span>|<span data-ttu-id="703f7-448">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-448">Boolean</span></span>|<span data-ttu-id="703f7-449">Indica se a reinicialização ou não do dispositivo na inicialização segura está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="703f7-449">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="703f7-450">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-450">screenCaptureBlocked</span></span>|<span data-ttu-id="703f7-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="703f7-451">Boolean</span></span>|<span data-ttu-id="703f7-452">Indica se o recurso deve ou não ser desabilitado para fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="703f7-452">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="703f7-453">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="703f7-453">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="703f7-454">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-454">Boolean</span></span>|<span data-ttu-id="703f7-455">Indica se o usuário deve ou não bloquear a habilitação de recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-455">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="703f7-456">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="703f7-456">securityRequireVerifyApps</span></span>|<span data-ttu-id="703f7-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="703f7-457">Boolean</span></span>|<span data-ttu-id="703f7-458">Indica se os aplicativos são ou não necessários.</span><span class="sxs-lookup"><span data-stu-id="703f7-458">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="703f7-459">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-459">statusBarBlocked</span></span>|<span data-ttu-id="703f7-460">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-460">Boolean</span></span>|<span data-ttu-id="703f7-461">Indica se ou a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.</span><span class="sxs-lookup"><span data-stu-id="703f7-461">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="703f7-462">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="703f7-462">stayOnModes</span></span>|<span data-ttu-id="703f7-463">[coleção androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)</span><span class="sxs-lookup"><span data-stu-id="703f7-463">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="703f7-464">Lista de modos em que a exibição do dispositivo permanecerá acionada.</span><span class="sxs-lookup"><span data-stu-id="703f7-464">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="703f7-465">Essa coleção pode conter no máximo quatro elementos.</span><span class="sxs-lookup"><span data-stu-id="703f7-465">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="703f7-466">Os valores possíveis são: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="703f7-466">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="703f7-467">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="703f7-467">storageAllowUsb</span></span>|<span data-ttu-id="703f7-468">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-468">Boolean</span></span>|<span data-ttu-id="703f7-469">Indica se é ou não para permitir o armazenamento em massa USB.</span><span class="sxs-lookup"><span data-stu-id="703f7-469">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="703f7-470">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="703f7-470">storageBlockExternalMedia</span></span>|<span data-ttu-id="703f7-471">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-471">Boolean</span></span>|<span data-ttu-id="703f7-472">Indica se a mídia externa deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="703f7-472">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="703f7-473">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="703f7-473">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="703f7-474">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-474">Boolean</span></span>|<span data-ttu-id="703f7-475">Indica se a transferência de arquivo USB deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="703f7-475">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="703f7-476">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="703f7-476">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="703f7-477">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-477">Int32</span></span>|<span data-ttu-id="703f7-478">Indica o número de minutos após a meia-noite em que a janela de atualização do sistema é iniciada.</span><span class="sxs-lookup"><span data-stu-id="703f7-478">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="703f7-479">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="703f7-479">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="703f7-480">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="703f7-480">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="703f7-481">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-481">Int32</span></span>|<span data-ttu-id="703f7-482">Indica o número de minutos após a meia-noite em que a janela de atualização do sistema termina.</span><span class="sxs-lookup"><span data-stu-id="703f7-482">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="703f7-483">Valores válidos de 0 a 1440</span><span class="sxs-lookup"><span data-stu-id="703f7-483">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="703f7-484">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="703f7-484">systemUpdateInstallType</span></span>|[<span data-ttu-id="703f7-485">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="703f7-485">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="703f7-486">O tipo de configuração de atualização do sistema.</span><span class="sxs-lookup"><span data-stu-id="703f7-486">The type of system update configuration.</span></span> <span data-ttu-id="703f7-487">Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="703f7-487">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="703f7-488">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-488">systemWindowsBlocked</span></span>|<span data-ttu-id="703f7-489">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-489">Boolean</span></span>|<span data-ttu-id="703f7-490">Se deve ou não bloquear janelas de prompt do sistema Android, como notualizações, atividades telefônicas e alertas do sistema.</span><span class="sxs-lookup"><span data-stu-id="703f7-490">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="703f7-491">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="703f7-491">usersBlockAdd</span></span>|<span data-ttu-id="703f7-492">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-492">Boolean</span></span>|<span data-ttu-id="703f7-493">Indica se a adição ou não de usuários e perfis está desabilitada.</span><span class="sxs-lookup"><span data-stu-id="703f7-493">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="703f7-494">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="703f7-494">usersBlockRemove</span></span>|<span data-ttu-id="703f7-495">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-495">Boolean</span></span>|<span data-ttu-id="703f7-496">Indica se deve ou não desabilitar a remoção de outros usuários do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="703f7-496">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="703f7-497">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="703f7-497">volumeBlockAdjustment</span></span>|<span data-ttu-id="703f7-498">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-498">Boolean</span></span>|<span data-ttu-id="703f7-499">Indica se o ajuste do volume mestre está desabilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="703f7-499">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="703f7-500">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="703f7-500">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="703f7-501">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-501">Boolean</span></span>|<span data-ttu-id="703f7-502">Se um nome de pacote VPN sempre estiver especificado, se o tráfego de rede será ou não travado quando essa VPN estiver desconectada.</span><span class="sxs-lookup"><span data-stu-id="703f7-502">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="703f7-503">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="703f7-503">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="703f7-504">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="703f7-504">String</span></span>|<span data-ttu-id="703f7-505">Nome do pacote do aplicativo Android para aplicativo que lidará com uma conexão VPN sempre on.</span><span class="sxs-lookup"><span data-stu-id="703f7-505">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="703f7-506">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="703f7-506">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="703f7-507">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-507">Boolean</span></span>|<span data-ttu-id="703f7-508">Indica se o usuário deve ou não bloquear a edição das configurações de conexão wifi.</span><span class="sxs-lookup"><span data-stu-id="703f7-508">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="703f7-509">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="703f7-509">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="703f7-510">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-510">Boolean</span></span>|<span data-ttu-id="703f7-511">Indica se o usuário deve ou não bloquear a edição apenas das redes definidas pela política.</span><span class="sxs-lookup"><span data-stu-id="703f7-511">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|
|<span data-ttu-id="703f7-512">personalProfileAppsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="703f7-512">personalProfileAppsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="703f7-513">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-513">Boolean</span></span>|<span data-ttu-id="703f7-514">Indica se o usuário pode instalar aplicativos de fontes desconhecidas no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="703f7-514">Indicates whether the user can install apps from unknown sources on the personal profile.</span></span>|
|<span data-ttu-id="703f7-515">personalProfileCameraBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-515">personalProfileCameraBlocked</span></span>|<span data-ttu-id="703f7-516">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-516">Boolean</span></span>|<span data-ttu-id="703f7-517">Indica se o uso da câmera deve ser desabilitado no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="703f7-517">Indicates whether to disable the use of the camera on the personal profile.</span></span>|
|<span data-ttu-id="703f7-518">personalProfileScreenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="703f7-518">personalProfileScreenCaptureBlocked</span></span>|<span data-ttu-id="703f7-519">Booleano</span><span class="sxs-lookup"><span data-stu-id="703f7-519">Boolean</span></span>|<span data-ttu-id="703f7-520">Indica se a funcionalidade deve ser desabilitada para fazer capturas de tela no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="703f7-520">Indicates whether to disable the capability to take screenshots on the personal profile.</span></span>|
|<span data-ttu-id="703f7-521">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="703f7-521">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="703f7-522">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-522">Int32</span></span>|<span data-ttu-id="703f7-523">Indica o número de dias em que uma senha de perfil de trabalho pode ser definida antes de expirar e uma nova senha será necessária.</span><span class="sxs-lookup"><span data-stu-id="703f7-523">Indicates the number of days that a work profile password can be set before it expires and a new password will be required.</span></span> <span data-ttu-id="703f7-524">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="703f7-524">Valid values 1 to 365</span></span>|
|<span data-ttu-id="703f7-525">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="703f7-525">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="703f7-526">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-526">Int32</span></span>|<span data-ttu-id="703f7-527">Indica o tamanho mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="703f7-527">Indicates the minimum length of the work profile password.</span></span> <span data-ttu-id="703f7-528">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-528">Valid values 4 to 16</span></span>|
|<span data-ttu-id="703f7-529">workProfilePasswordMinimumNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="703f7-529">workProfilePasswordMinimumNumericCharacters</span></span>|<span data-ttu-id="703f7-530">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-530">Int32</span></span>|<span data-ttu-id="703f7-531">Indica o número mínimo de caracteres numéricos necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="703f7-531">Indicates the minimum number of numeric characters required for the work profile password.</span></span> <span data-ttu-id="703f7-532">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-532">Valid values 1 to 16</span></span>|
|<span data-ttu-id="703f7-533">workProfilePasswordMinimumNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="703f7-533">workProfilePasswordMinimumNonLetterCharacters</span></span>|<span data-ttu-id="703f7-534">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-534">Int32</span></span>|<span data-ttu-id="703f7-535">Indica o número mínimo de caracteres que não são letras necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="703f7-535">Indicates the minimum number of non-letter characters required for the work profile password.</span></span> <span data-ttu-id="703f7-536">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-536">Valid values 1 to 16</span></span>|
|<span data-ttu-id="703f7-537">workProfilePasswordMinimumLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="703f7-537">workProfilePasswordMinimumLetterCharacters</span></span>|<span data-ttu-id="703f7-538">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-538">Int32</span></span>|<span data-ttu-id="703f7-539">Indica o número mínimo de caracteres de letra necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="703f7-539">Indicates the minimum number of letter characters required for the work profile password.</span></span> <span data-ttu-id="703f7-540">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-540">Valid values 1 to 16</span></span>|
|<span data-ttu-id="703f7-541">workProfilePasswordMinimumLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="703f7-541">workProfilePasswordMinimumLowerCaseCharacters</span></span>|<span data-ttu-id="703f7-542">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-542">Int32</span></span>|<span data-ttu-id="703f7-543">Indica o número mínimo de caracteres de caso inferior necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="703f7-543">Indicates the minimum number of lower-case characters required for the work profile password.</span></span> <span data-ttu-id="703f7-544">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-544">Valid values 1 to 16</span></span>|
|<span data-ttu-id="703f7-545">workProfilePasswordMinimumUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="703f7-545">workProfilePasswordMinimumUpperCaseCharacters</span></span>|<span data-ttu-id="703f7-546">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-546">Int32</span></span>|<span data-ttu-id="703f7-547">Indica o número mínimo de caracteres de letra de maiúsculas e altas necessários para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="703f7-547">Indicates the minimum number of upper-case letter characters required for the work profile password.</span></span> <span data-ttu-id="703f7-548">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-548">Valid values 1 to 16</span></span>|
|<span data-ttu-id="703f7-549">workProfilePasswordMinimumSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="703f7-549">workProfilePasswordMinimumSymbolCharacters</span></span>|<span data-ttu-id="703f7-550">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-550">Int32</span></span>|<span data-ttu-id="703f7-551">Indica o número mínimo de caracteres de símbolo necessário para a senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="703f7-551">Indicates the minimum number of symbol characters required for the work profile password.</span></span> <span data-ttu-id="703f7-552">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="703f7-552">Valid values 1 to 16</span></span>|
|<span data-ttu-id="703f7-553">workProfilePasswordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="703f7-553">workProfilePasswordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="703f7-554">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-554">Int32</span></span>|<span data-ttu-id="703f7-555">Indica o tamanho do histórico de senhas do perfil de trabalho, onde o usuário não poderá inserir uma nova senha que seja a mesma de qualquer senha no histórico.</span><span class="sxs-lookup"><span data-stu-id="703f7-555">Indicates the length of the work profile password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="703f7-556">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="703f7-556">Valid values 0 to 24</span></span>|
|<span data-ttu-id="703f7-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="703f7-557">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="703f7-558">Int32</span><span class="sxs-lookup"><span data-stu-id="703f7-558">Int32</span></span>|<span data-ttu-id="703f7-559">Indica o número de vezes que um usuário pode inserir uma senha de perfil de trabalho incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="703f7-559">Indicates the number of times a user can enter an incorrect work profile password before the device is wiped.</span></span> <span data-ttu-id="703f7-560">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="703f7-560">Valid values 4 to 11</span></span>|
|<span data-ttu-id="703f7-561">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="703f7-561">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="703f7-562">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="703f7-562">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="703f7-563">Indica a qualidade mínima de senha necessária na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="703f7-563">Indicates the minimum password quality required on the work profile password.</span></span> <span data-ttu-id="703f7-564">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="703f7-564">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="703f7-565">Resposta</span><span class="sxs-lookup"><span data-stu-id="703f7-565">Response</span></span>
<span data-ttu-id="703f7-566">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="703f7-566">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="703f7-567">Exemplo</span><span class="sxs-lookup"><span data-stu-id="703f7-567">Example</span></span>

### <a name="request"></a><span data-ttu-id="703f7-568">Solicitação</span><span class="sxs-lookup"><span data-stu-id="703f7-568">Request</span></span>
<span data-ttu-id="703f7-569">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="703f7-569">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 7313

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
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
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required"
}
```

### <a name="response"></a><span data-ttu-id="703f7-570">Resposta</span><span class="sxs-lookup"><span data-stu-id="703f7-570">Response</span></span>
<span data-ttu-id="703f7-p160">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="703f7-p160">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7485

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
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
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "certificateCredentialConfigurationDisabled": true,
  "microsoftLauncherConfigurationEnabled": true,
  "microsoftLauncherCustomWallpaperEnabled": true,
  "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
  "microsoftLauncherCustomWallpaperAllowUserModification": true,
  "microsoftLauncherFeedEnabled": true,
  "microsoftLauncherFeedAllowUserModification": true,
  "microsoftLauncherDockPresenceConfiguration": "show",
  "microsoftLauncherDockPresenceAllowUserModification": true,
  "microsoftLauncherSearchBarPlacementConfiguration": "top",
  "enrollmentProfile": "dedicatedDevice",
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "globalProxy": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
    "proxyAutoConfigURL": "Proxy Auto Config URL value"
  },
  "googleAccountsBlocked": true,
  "kioskCustomizationDeviceSettingsBlocked": true,
  "kioskCustomizationPowerButtonActionsBlocked": true,
  "kioskCustomizationStatusBar": "notificationsAndSystemInfoEnabled",
  "kioskCustomizationSystemErrorWarnings": true,
  "kioskCustomizationSystemNavigation": "navigationEnabled",
  "kioskModeScreenSaverConfigurationEnabled": true,
  "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
  "kioskModeScreenSaverDisplayTimeInSeconds": 8,
  "kioskModeScreenSaverStartDelayInSeconds": 7,
  "kioskModeScreenSaverDetectMediaDisabled": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "kioskModeVirtualHomeButtonType": "swipeUp",
  "kioskModeBluetoothConfigurationEnabled": true,
  "kioskModeWiFiConfigurationEnabled": true,
  "kioskModeFlashlightConfigurationEnabled": true,
  "kioskModeMediaVolumeConfigurationEnabled": true,
  "kioskModeShowDeviceInfo": true,
  "kioskModeManagedSettingsEntryDisabled": true,
  "kioskModeDebugMenuEasyAccessEnabled": true,
  "kioskModeShowAppNotificationBadge": true,
  "kioskModeScreenOrientation": "portrait",
  "kioskModeIconSize": "smallest",
  "kioskModeFolderIcon": "darkSquare",
  "kioskModeWifiAllowedSsids": [
    "Kiosk Mode Wifi Allowed Ssids value"
  ],
  "kioskModeAppOrderEnabled": true,
  "kioskModeAppsInFolderOrderedByName": true,
  "kioskModeGridHeight": 3,
  "kioskModeGridWidth": 2,
  "kioskModeLockHomeScreen": true,
  "kioskModeManagedFolders": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder",
      "folderName": "Folder Name value",
      "folderIdentifier": "Folder Identifier value",
      "items": [
        {
          "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
          "label": "Label value",
          "link": "Link value"
        }
      ]
    }
  ],
  "kioskModeAppPositions": [
    {
      "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
      "position": 8,
      "item": {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
        "label": "Label value",
        "link": "Link value"
      }
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "playStoreMode": "allowList",
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnLockdownMode": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true,
  "personalProfileAppsAllowInstallFromUnknownSources": true,
  "personalProfileCameraBlocked": true,
  "personalProfileScreenCaptureBlocked": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinimumNumericCharacters": 11,
  "workProfilePasswordMinimumNonLetterCharacters": 13,
  "workProfilePasswordMinimumLetterCharacters": 10,
  "workProfilePasswordMinimumLowerCaseCharacters": 13,
  "workProfilePasswordMinimumUpperCaseCharacters": 13,
  "workProfilePasswordMinimumSymbolCharacters": 10,
  "workProfilePasswordPreviousPasswordCountToBlock": 15,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "required"
}
```




