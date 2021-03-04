---
title: Criar aospDeviceOwnerDeviceConfiguration
description: Crie um novo objeto aospDeviceOwnerDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0613bfc61e34b66f2eab4b7e6e12b08efde6a52e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445715"
---
# <a name="create-aospdeviceownerdeviceconfiguration"></a><span data-ttu-id="9a0e7-103">Criar aospDeviceOwnerDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a0e7-103">Create aospDeviceOwnerDeviceConfiguration</span></span>

<span data-ttu-id="9a0e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a0e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a0e7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a0e7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a0e7-107">Crie um novo [objeto aospDeviceOwnerDeviceConfiguration.](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-107">Create a new [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a0e7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9a0e7-108">Prerequisites</span></span>
<span data-ttu-id="9a0e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a0e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a0e7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a0e7-111">Permission type</span></span>|<span data-ttu-id="9a0e7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a0e7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a0e7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a0e7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a0e7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a0e7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-116">Not supported.</span></span>|
|<span data-ttu-id="9a0e7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a0e7-117">Application</span></span>|<span data-ttu-id="9a0e7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a0e7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a0e7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a0e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9a0e7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0e7-120">Request headers</span></span>
|<span data-ttu-id="9a0e7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a0e7-121">Header</span></span>|<span data-ttu-id="9a0e7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9a0e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a0e7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a0e7-123">Authorization</span></span>|<span data-ttu-id="9a0e7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a0e7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9a0e7-125">Accept</span></span>|<span data-ttu-id="9a0e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a0e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a0e7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0e7-127">Request body</span></span>
<span data-ttu-id="9a0e7-128">No corpo da solicitação, fornece uma representação JSON para o objeto aospDeviceOwnerDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-128">In the request body, supply a JSON representation for the aospDeviceOwnerDeviceConfiguration object.</span></span>

<span data-ttu-id="9a0e7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o aospDeviceOwnerDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-129">The following table shows the properties that are required when you create the aospDeviceOwnerDeviceConfiguration.</span></span>

|<span data-ttu-id="9a0e7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a0e7-130">Property</span></span>|<span data-ttu-id="9a0e7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a0e7-131">Type</span></span>|<span data-ttu-id="9a0e7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a0e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a0e7-133">id</span><span class="sxs-lookup"><span data-stu-id="9a0e7-133">id</span></span>|<span data-ttu-id="9a0e7-134">String</span><span class="sxs-lookup"><span data-stu-id="9a0e7-134">String</span></span>|<span data-ttu-id="9a0e7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-135">Key of the entity.</span></span> <span data-ttu-id="9a0e7-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a0e7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a0e7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9a0e7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a0e7-138">DateTimeOffset</span></span>|<span data-ttu-id="9a0e7-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9a0e7-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a0e7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9a0e7-141">roleScopeTagIds</span></span>|<span data-ttu-id="9a0e7-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a0e7-142">String collection</span></span>|<span data-ttu-id="9a0e7-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9a0e7-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a0e7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9a0e7-145">supportsScopeTags</span></span>|<span data-ttu-id="9a0e7-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e7-146">Boolean</span></span>|<span data-ttu-id="9a0e7-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9a0e7-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9a0e7-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9a0e7-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-150">This property is read-only.</span></span> <span data-ttu-id="9a0e7-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a0e7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9a0e7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9a0e7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9a0e7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9a0e7-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9a0e7-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a0e7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9a0e7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9a0e7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9a0e7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9a0e7-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9a0e7-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a0e7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9a0e7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9a0e7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9a0e7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9a0e7-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9a0e7-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a0e7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a0e7-164">createdDateTime</span></span>|<span data-ttu-id="9a0e7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a0e7-165">DateTimeOffset</span></span>|<span data-ttu-id="9a0e7-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-166">DateTime the object was created.</span></span> <span data-ttu-id="9a0e7-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a0e7-168">descrição</span><span class="sxs-lookup"><span data-stu-id="9a0e7-168">description</span></span>|<span data-ttu-id="9a0e7-169">String</span><span class="sxs-lookup"><span data-stu-id="9a0e7-169">String</span></span>|<span data-ttu-id="9a0e7-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9a0e7-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a0e7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9a0e7-172">displayName</span></span>|<span data-ttu-id="9a0e7-173">String</span><span class="sxs-lookup"><span data-stu-id="9a0e7-173">String</span></span>|<span data-ttu-id="9a0e7-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9a0e7-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a0e7-176">versão</span><span class="sxs-lookup"><span data-stu-id="9a0e7-176">version</span></span>|<span data-ttu-id="9a0e7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9a0e7-177">Int32</span></span>|<span data-ttu-id="9a0e7-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-178">Version of the device configuration.</span></span> <span data-ttu-id="9a0e7-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9a0e7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9a0e7-180">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="9a0e7-180">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="9a0e7-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e7-181">Boolean</span></span>|<span data-ttu-id="9a0e7-182">Indica se o usuário tem ou não permissão para habilitar a configuração de fontes desconhecidas.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-182">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="9a0e7-183">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="9a0e7-183">bluetoothBlocked</span></span>|<span data-ttu-id="9a0e7-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a0e7-184">Boolean</span></span>|<span data-ttu-id="9a0e7-185">Indica se o uso do bluetooth deve ou não ser desabilitado.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-185">Indicates whether or not to disable the use of bluetooth.</span></span> <span data-ttu-id="9a0e7-186">Quando definido como true, o bluetooth não pode ser habilitado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-186">When set to true, bluetooth cannot be enabled on the device.</span></span>|
|<span data-ttu-id="9a0e7-187">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a0e7-187">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="9a0e7-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e7-188">Boolean</span></span>|<span data-ttu-id="9a0e7-189">Indica se um usuário deve ou não bloquear a configuração do bluetooth.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-189">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="9a0e7-190">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="9a0e7-190">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="9a0e7-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e7-191">Boolean</span></span>|<span data-ttu-id="9a0e7-192">Indica se um usuário deve ou não bloquear o compartilhamento de contatos via bluetooth.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-192">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="9a0e7-193">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="9a0e7-193">cameraBlocked</span></span>|<span data-ttu-id="9a0e7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a0e7-194">Boolean</span></span>|<span data-ttu-id="9a0e7-195">Indica se o uso da câmera deve ou não ser desabilitado.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-195">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="9a0e7-196">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="9a0e7-196">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="9a0e7-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a0e7-197">Boolean</span></span>|<span data-ttu-id="9a0e7-198">Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-198">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="9a0e7-199">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="9a0e7-199">factoryResetBlocked</span></span>|<span data-ttu-id="9a0e7-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a0e7-200">Boolean</span></span>|<span data-ttu-id="9a0e7-201">Indica se a opção de redefinição de fábrica nas configurações está desabilitada ou não.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-201">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="9a0e7-202">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9a0e7-202">passwordMinimumLength</span></span>|<span data-ttu-id="9a0e7-203">Int32</span><span class="sxs-lookup"><span data-stu-id="9a0e7-203">Int32</span></span>|<span data-ttu-id="9a0e7-204">Indica o tamanho mínimo da senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-204">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="9a0e7-205">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="9a0e7-205">Valid values 4 to 16</span></span>|
|<span data-ttu-id="9a0e7-206">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9a0e7-206">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9a0e7-207">Int32</span><span class="sxs-lookup"><span data-stu-id="9a0e7-207">Int32</span></span>|<span data-ttu-id="9a0e7-208">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-208">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="9a0e7-209">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9a0e7-209">passwordRequiredType</span></span>|[<span data-ttu-id="9a0e7-210">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9a0e7-210">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="9a0e7-211">Indica a qualidade mínima de senha necessária no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-211">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="9a0e7-212">Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-212">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.</span></span>|
|<span data-ttu-id="9a0e7-213">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9a0e7-213">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9a0e7-214">Int32</span><span class="sxs-lookup"><span data-stu-id="9a0e7-214">Int32</span></span>|<span data-ttu-id="9a0e7-215">Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-215">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="9a0e7-216">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="9a0e7-216">Valid values 4 to 11</span></span>|
|<span data-ttu-id="9a0e7-217">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="9a0e7-217">screenCaptureBlocked</span></span>|<span data-ttu-id="9a0e7-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a0e7-218">Boolean</span></span>|<span data-ttu-id="9a0e7-219">Indica se o recurso deve ou não ser desabilitado para fazer capturas de tela.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-219">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="9a0e7-220">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="9a0e7-220">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="9a0e7-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e7-221">Boolean</span></span>|<span data-ttu-id="9a0e7-222">Indica se o usuário deve ou não bloquear a habilitação de recursos de depuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-222">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="9a0e7-223">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="9a0e7-223">storageAllowUsb</span></span>|<span data-ttu-id="9a0e7-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e7-224">Boolean</span></span>|<span data-ttu-id="9a0e7-225">Indica se o armazenamento USB deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-225">Indicates whether or not to block USB storage.</span></span>|
|<span data-ttu-id="9a0e7-226">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="9a0e7-226">storageBlockExternalMedia</span></span>|<span data-ttu-id="9a0e7-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e7-227">Boolean</span></span>|<span data-ttu-id="9a0e7-228">Indica se a mídia externa deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-228">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="9a0e7-229">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="9a0e7-229">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="9a0e7-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e7-230">Boolean</span></span>|<span data-ttu-id="9a0e7-231">Indica se a transferência de arquivo USB deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-231">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="9a0e7-232">backupBlocked</span><span class="sxs-lookup"><span data-stu-id="9a0e7-232">backupBlocked</span></span>|<span data-ttu-id="9a0e7-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e7-233">Boolean</span></span>|<span data-ttu-id="9a0e7-234">Indica se o serviço de backup deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-234">Indicates whether or not to block backup service.</span></span>|
|<span data-ttu-id="9a0e7-235">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="9a0e7-235">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="9a0e7-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a0e7-236">Boolean</span></span>|<span data-ttu-id="9a0e7-237">Indica se o usuário deve ou não bloquear a edição das configurações de conexão wifi.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-237">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|



## <a name="response"></a><span data-ttu-id="9a0e7-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a0e7-238">Response</span></span>
<span data-ttu-id="9a0e7-239">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-239">If successful, this method returns a `201 Created` response code and a [aospDeviceOwnerDeviceConfiguration](../resources/intune-deviceconfig-aospdeviceownerdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a0e7-240">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a0e7-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a0e7-241">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0e7-241">Request</span></span>
<span data-ttu-id="9a0e7-242">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1721

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerDeviceConfiguration",
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
  "appsAllowInstallFromUnknownSources": true,
  "bluetoothBlocked": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "factoryResetBlocked": true,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "backupBlocked": true,
  "wifiBlockEditConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="9a0e7-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a0e7-243">Response</span></span>
<span data-ttu-id="9a0e7-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a0e7-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1893

{
  "@odata.type": "#microsoft.graph.aospDeviceOwnerDeviceConfiguration",
  "id": "c9e83a69-3a69-c9e8-693a-e8c9693ae8c9",
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
  "appsAllowInstallFromUnknownSources": true,
  "bluetoothBlocked": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "factoryResetBlocked": true,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "backupBlocked": true,
  "wifiBlockEditConfigurations": true
}
```




