---
title: Atualizar macOSDeviceFeaturesConfiguration
description: Atualizar as propriedades de um objeto macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4ca8d2f36cebda6210f39a3b23aa6d098632e375
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131369"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="e07dc-103">Atualizar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="e07dc-103">Update macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="e07dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e07dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e07dc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e07dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e07dc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e07dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e07dc-107">Atualizar as propriedades de um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e07dc-107">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e07dc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e07dc-108">Prerequisites</span></span>
<span data-ttu-id="e07dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e07dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e07dc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e07dc-111">Permission type</span></span>|<span data-ttu-id="e07dc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e07dc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e07dc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e07dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e07dc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e07dc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e07dc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e07dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e07dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e07dc-116">Not supported.</span></span>|
|<span data-ttu-id="e07dc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e07dc-117">Application</span></span>|<span data-ttu-id="e07dc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e07dc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e07dc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e07dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e07dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e07dc-120">Request headers</span></span>
|<span data-ttu-id="e07dc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e07dc-121">Header</span></span>|<span data-ttu-id="e07dc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e07dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e07dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e07dc-123">Authorization</span></span>|<span data-ttu-id="e07dc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e07dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e07dc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e07dc-125">Accept</span></span>|<span data-ttu-id="e07dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e07dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e07dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e07dc-127">Request body</span></span>
<span data-ttu-id="e07dc-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e07dc-128">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="e07dc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e07dc-129">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="e07dc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e07dc-130">Property</span></span>|<span data-ttu-id="e07dc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e07dc-131">Type</span></span>|<span data-ttu-id="e07dc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e07dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e07dc-133">id</span><span class="sxs-lookup"><span data-stu-id="e07dc-133">id</span></span>|<span data-ttu-id="e07dc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07dc-134">String</span></span>|<span data-ttu-id="e07dc-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e07dc-135">Key of the entity.</span></span> <span data-ttu-id="e07dc-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e07dc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e07dc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e07dc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e07dc-138">DateTimeOffset</span></span>|<span data-ttu-id="e07dc-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e07dc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e07dc-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e07dc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e07dc-141">roleScopeTagIds</span></span>|<span data-ttu-id="e07dc-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07dc-142">String collection</span></span>|<span data-ttu-id="e07dc-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="e07dc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e07dc-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e07dc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e07dc-145">supportsScopeTags</span></span>|<span data-ttu-id="e07dc-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-146">Boolean</span></span>|<span data-ttu-id="e07dc-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e07dc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e07dc-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e07dc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e07dc-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="e07dc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e07dc-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e07dc-150">This property is read-only.</span></span> <span data-ttu-id="e07dc-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e07dc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e07dc-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e07dc-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e07dc-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e07dc-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="e07dc-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e07dc-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e07dc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e07dc-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e07dc-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e07dc-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e07dc-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="e07dc-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e07dc-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e07dc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e07dc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e07dc-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e07dc-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e07dc-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="e07dc-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e07dc-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e07dc-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e07dc-164">createdDateTime</span></span>|<span data-ttu-id="e07dc-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e07dc-165">DateTimeOffset</span></span>|<span data-ttu-id="e07dc-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e07dc-166">DateTime the object was created.</span></span> <span data-ttu-id="e07dc-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e07dc-168">descrição</span><span class="sxs-lookup"><span data-stu-id="e07dc-168">description</span></span>|<span data-ttu-id="e07dc-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07dc-169">String</span></span>|<span data-ttu-id="e07dc-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e07dc-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e07dc-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e07dc-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e07dc-172">displayName</span></span>|<span data-ttu-id="e07dc-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07dc-173">String</span></span>|<span data-ttu-id="e07dc-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e07dc-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e07dc-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e07dc-176">versão</span><span class="sxs-lookup"><span data-stu-id="e07dc-176">version</span></span>|<span data-ttu-id="e07dc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e07dc-177">Int32</span></span>|<span data-ttu-id="e07dc-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e07dc-178">Version of the device configuration.</span></span> <span data-ttu-id="e07dc-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e07dc-180">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="e07dc-180">airPrintDestinations</span></span>|<span data-ttu-id="e07dc-181">[Coleção airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="e07dc-182">Uma matriz de impressoras AirPrint que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="e07dc-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="e07dc-183">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e07dc-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e07dc-184">Herdado [do appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="e07dc-185">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="e07dc-185">autoLaunchItems</span></span>|<span data-ttu-id="e07dc-186">[Coleção macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="e07dc-187">Lista de aplicativos, arquivos, pastas e outros itens a iniciar quando o usuário faz login.</span><span class="sxs-lookup"><span data-stu-id="e07dc-187">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="e07dc-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e07dc-188">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e07dc-189">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="e07dc-189">adminShowHostInfo</span></span>|<span data-ttu-id="e07dc-190">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-190">Boolean</span></span>|<span data-ttu-id="e07dc-191">Se deve mostrar informações do host do administrador na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="e07dc-191">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="e07dc-192">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="e07dc-192">loginWindowText</span></span>|<span data-ttu-id="e07dc-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07dc-193">String</span></span>|<span data-ttu-id="e07dc-194">Texto personalizado a ser exibido na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="e07dc-194">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="e07dc-195">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="e07dc-195">authorizedUsersListHidden</span></span>|<span data-ttu-id="e07dc-196">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-196">Boolean</span></span>|<span data-ttu-id="e07dc-197">Se será exibida a caixa de diálogo nome e senha ou uma lista de usuários na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="e07dc-197">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="e07dc-198">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="e07dc-198">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="e07dc-199">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-199">Boolean</span></span>|<span data-ttu-id="e07dc-200">Se apenas os usuários da rede e do sistema na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="e07dc-200">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="e07dc-201">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="e07dc-201">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="e07dc-202">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-202">Boolean</span></span>|<span data-ttu-id="e07dc-203">Se deve ocultar usuários móveis na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="e07dc-203">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="e07dc-204">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="e07dc-204">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="e07dc-205">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-205">Boolean</span></span>|<span data-ttu-id="e07dc-206">Se deve mostrar usuários de rede na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="e07dc-206">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="e07dc-207">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="e07dc-207">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="e07dc-208">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-208">Boolean</span></span>|<span data-ttu-id="e07dc-209">Se deve ocultar usuários de administrador na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="e07dc-209">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="e07dc-210">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="e07dc-210">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="e07dc-211">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-211">Boolean</span></span>|<span data-ttu-id="e07dc-212">Se deve mostrar outros usuários na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="e07dc-212">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="e07dc-213">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="e07dc-213">shutDownDisabled</span></span>|<span data-ttu-id="e07dc-214">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-214">Boolean</span></span>|<span data-ttu-id="e07dc-215">Se deve ocultar o item do botão Desligar na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="e07dc-215">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="e07dc-216">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="e07dc-216">restartDisabled</span></span>|<span data-ttu-id="e07dc-217">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-217">Boolean</span></span>|<span data-ttu-id="e07dc-218">Se deve ocultar o item do botão Reiniciar na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="e07dc-218">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="e07dc-219">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="e07dc-219">sleepDisabled</span></span>|<span data-ttu-id="e07dc-220">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-220">Boolean</span></span>|<span data-ttu-id="e07dc-221">Se deve ocultar o item de menu Ental na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="e07dc-221">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="e07dc-222">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="e07dc-222">consoleAccessDisabled</span></span>|<span data-ttu-id="e07dc-223">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-223">Boolean</span></span>|<span data-ttu-id="e07dc-224">Se o outro usuário ignorará o uso do ' console>> nome de usuário especial.</span><span class="sxs-lookup"><span data-stu-id="e07dc-224">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="e07dc-225">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="e07dc-225">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="e07dc-226">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-226">Boolean</span></span>|<span data-ttu-id="e07dc-227">Se o item de menu Desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="e07dc-227">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="e07dc-228">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="e07dc-228">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="e07dc-229">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-229">Boolean</span></span>|<span data-ttu-id="e07dc-230">Se o item de menu Reiniciar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="e07dc-230">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="e07dc-231">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="e07dc-231">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="e07dc-232">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-232">Boolean</span></span>|<span data-ttu-id="e07dc-233">Se o item de menu Desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="e07dc-233">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="e07dc-234">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="e07dc-234">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="e07dc-235">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-235">Boolean</span></span>|<span data-ttu-id="e07dc-236">Se o item de menu Sair na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="e07dc-236">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="e07dc-237">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="e07dc-237">screenLockDisableImmediate</span></span>|<span data-ttu-id="e07dc-238">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-238">Boolean</span></span>|<span data-ttu-id="e07dc-239">Se desabilitar as funções imediatas de bloqueio de tela.</span><span class="sxs-lookup"><span data-stu-id="e07dc-239">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="e07dc-240">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="e07dc-240">associatedDomains</span></span>|<span data-ttu-id="e07dc-241">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e07dc-242">PRETERIDO: use appAssociatedDomains.</span><span class="sxs-lookup"><span data-stu-id="e07dc-242">DEPRECATED: use appAssociatedDomains instead.</span></span> <span data-ttu-id="e07dc-243">Obtém ou define uma lista que mapeia aplicativos para seus domínios associados.</span><span class="sxs-lookup"><span data-stu-id="e07dc-243">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="e07dc-244">A chave deve corresponder à ID do aplicativo e o valor deve ser uma cadeia de caracteres na forma de "service:domain" em que o domínio é um nome de host totalmente qualificado (por exemplo, webcredentials:example.com).</span><span class="sxs-lookup"><span data-stu-id="e07dc-244">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="e07dc-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e07dc-245">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e07dc-246">appAssociatedDomains</span><span class="sxs-lookup"><span data-stu-id="e07dc-246">appAssociatedDomains</span></span>|<span data-ttu-id="e07dc-247">[Coleção macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-247">[macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md) collection</span></span>|<span data-ttu-id="e07dc-248">Obtém ou define uma lista que mapeia aplicativos para seus domínios associados.</span><span class="sxs-lookup"><span data-stu-id="e07dc-248">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="e07dc-249">Os identificadores de aplicativo devem ser exclusivos.</span><span class="sxs-lookup"><span data-stu-id="e07dc-249">Application identifiers must be unique.</span></span> <span data-ttu-id="e07dc-250">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e07dc-250">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e07dc-251">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="e07dc-251">singleSignOnExtension</span></span>|[<span data-ttu-id="e07dc-252">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="e07dc-252">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="e07dc-253">Obtém ou define um único perfil de extensão de entrada.</span><span class="sxs-lookup"><span data-stu-id="e07dc-253">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="e07dc-254">Preterido: use MacOSSingleSignOnExtension.</span><span class="sxs-lookup"><span data-stu-id="e07dc-254">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="e07dc-255">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="e07dc-255">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="e07dc-256">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="e07dc-256">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="e07dc-257">Obtém ou define um único perfil de extensão de entrada.</span><span class="sxs-lookup"><span data-stu-id="e07dc-257">Gets or sets a single sign-on extension profile.</span></span>|
|<span data-ttu-id="e07dc-258">contentCachingEnabled</span><span class="sxs-lookup"><span data-stu-id="e07dc-258">contentCachingEnabled</span></span>|<span data-ttu-id="e07dc-259">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-259">Boolean</span></span>|<span data-ttu-id="e07dc-260">Habilita o cache de conteúdo e impede que ele seja desabilitado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="e07dc-260">Enables content caching and prevents it from being disabled by the user.</span></span>|
|<span data-ttu-id="e07dc-261">contentCachingType</span><span class="sxs-lookup"><span data-stu-id="e07dc-261">contentCachingType</span></span>|[<span data-ttu-id="e07dc-262">macOSContentCachingType</span><span class="sxs-lookup"><span data-stu-id="e07dc-262">macOSContentCachingType</span></span>](../resources/intune-deviceconfig-macoscontentcachingtype.md)|<span data-ttu-id="e07dc-263">Determina que tipo de conteúdo pode ser armazenado em cache pelo serviço de cache de conteúdo da Apple.</span><span class="sxs-lookup"><span data-stu-id="e07dc-263">Determines what type of content is allowed to be cached by Apple's content caching service.</span></span> <span data-ttu-id="e07dc-264">Os valores possíveis são: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span><span class="sxs-lookup"><span data-stu-id="e07dc-264">Possible values are: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span></span>|
|<span data-ttu-id="e07dc-265">contentCachingMaxSizeBytes</span><span class="sxs-lookup"><span data-stu-id="e07dc-265">contentCachingMaxSizeBytes</span></span>|<span data-ttu-id="e07dc-266">Int32</span><span class="sxs-lookup"><span data-stu-id="e07dc-266">Int32</span></span>|<span data-ttu-id="e07dc-267">O número máximo de bytes de espaço em disco que será usado para o cache de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e07dc-267">The maximum number of bytes of disk space that will be used for the content cache.</span></span> <span data-ttu-id="e07dc-268">Um valor 0 (padrão) indica espaço em disco ilimitado.</span><span class="sxs-lookup"><span data-stu-id="e07dc-268">A value of 0 (default) indicates unlimited disk space.</span></span> |
|<span data-ttu-id="e07dc-269">contentCachingDataPath</span><span class="sxs-lookup"><span data-stu-id="e07dc-269">contentCachingDataPath</span></span>|<span data-ttu-id="e07dc-270">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07dc-270">String</span></span>|<span data-ttu-id="e07dc-271">O caminho para o diretório usado para armazenar conteúdo armazenado em cache.</span><span class="sxs-lookup"><span data-stu-id="e07dc-271">The path to the directory used to store cached content.</span></span> <span data-ttu-id="e07dc-272">O valor deve ser (ou terminar com) /Library/Application Support/Apple/AssetCache/Data</span><span class="sxs-lookup"><span data-stu-id="e07dc-272">The value must be (or end with) /Library/Application Support/Apple/AssetCache/Data</span></span>|
|<span data-ttu-id="e07dc-273">contentCachingDisableConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="e07dc-273">contentCachingDisableConnectionSharing</span></span>|<span data-ttu-id="e07dc-274">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-274">Boolean</span></span>|<span data-ttu-id="e07dc-275">Desabilita o compartilhamento de conexões com a Internet.</span><span class="sxs-lookup"><span data-stu-id="e07dc-275">Disables internet connection sharing.</span></span>|
|<span data-ttu-id="e07dc-276">contentCachingForceConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="e07dc-276">contentCachingForceConnectionSharing</span></span>|<span data-ttu-id="e07dc-277">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-277">Boolean</span></span>|<span data-ttu-id="e07dc-278">Força o compartilhamento de conexão com a Internet.</span><span class="sxs-lookup"><span data-stu-id="e07dc-278">Forces internet connection sharing.</span></span> <span data-ttu-id="e07dc-279">contentCachingDisableConnectionSharing substitui essa configuração.</span><span class="sxs-lookup"><span data-stu-id="e07dc-279">contentCachingDisableConnectionSharing overrides this setting.</span></span>|
|<span data-ttu-id="e07dc-280">contentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="e07dc-280">contentCachingClientPolicy</span></span>|[<span data-ttu-id="e07dc-281">macOSContentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="e07dc-281">macOSContentCachingClientPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|<span data-ttu-id="e07dc-282">Determina o método no qual os servidores de cache de conteúdo escutarão clientes.</span><span class="sxs-lookup"><span data-stu-id="e07dc-282">Determines the method in which content caching servers will listen for clients.</span></span> <span data-ttu-id="e07dc-283">Os valores possíveis são: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span><span class="sxs-lookup"><span data-stu-id="e07dc-283">Possible values are: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span></span>|
|<span data-ttu-id="e07dc-284">contentCachingClientListenRanges</span><span class="sxs-lookup"><span data-stu-id="e07dc-284">contentCachingClientListenRanges</span></span>|<span data-ttu-id="e07dc-285">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-285">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="e07dc-286">Uma lista de caches de conteúdo de intervalos IP personalizados será usada para escutar clientes.</span><span class="sxs-lookup"><span data-stu-id="e07dc-286">A list of custom IP ranges content caches will use to listen for clients.</span></span> <span data-ttu-id="e07dc-287">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e07dc-287">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e07dc-288">contentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="e07dc-288">contentCachingPeerPolicy</span></span>|[<span data-ttu-id="e07dc-289">macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="e07dc-289">macOSContentCachingPeerPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|<span data-ttu-id="e07dc-290">Determina o método no qual o conteúdo armazena o par de caches com outros caches.</span><span class="sxs-lookup"><span data-stu-id="e07dc-290">Determines the method in which content caches peer with other caches.</span></span> <span data-ttu-id="e07dc-291">Os valores possíveis são: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span><span class="sxs-lookup"><span data-stu-id="e07dc-291">Possible values are: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span></span>|
|<span data-ttu-id="e07dc-292">contentCachingPeerListenRanges</span><span class="sxs-lookup"><span data-stu-id="e07dc-292">contentCachingPeerListenRanges</span></span>|<span data-ttu-id="e07dc-293">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-293">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="e07dc-294">Uma lista de caches de conteúdo de intervalos IP personalizados será usada para escutar caches de pares.</span><span class="sxs-lookup"><span data-stu-id="e07dc-294">A list of custom IP ranges content caches will use to listen for peer caches.</span></span> <span data-ttu-id="e07dc-295">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e07dc-295">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e07dc-296">contentCachingPeerFilterRanges</span><span class="sxs-lookup"><span data-stu-id="e07dc-296">contentCachingPeerFilterRanges</span></span>|<span data-ttu-id="e07dc-297">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-297">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="e07dc-298">Uma lista de caches de conteúdo de intervalos IP personalizados será usada para consultar conteúdo de caches de pares.</span><span class="sxs-lookup"><span data-stu-id="e07dc-298">A list of custom IP ranges content caches will use to query for content from peers caches.</span></span> <span data-ttu-id="e07dc-299">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e07dc-299">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e07dc-300">contentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e07dc-300">contentCachingParentSelectionPolicy</span></span>|[<span data-ttu-id="e07dc-301">macOSContentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e07dc-301">macOSContentCachingParentSelectionPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|<span data-ttu-id="e07dc-302">Determina o método no qual os servidores de cache de conteúdo selecionarão pais se vários estão presentes.</span><span class="sxs-lookup"><span data-stu-id="e07dc-302">Determines the method in which content caching servers will select parents if multiple are present.</span></span> <span data-ttu-id="e07dc-303">Os possíveis valores são: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span><span class="sxs-lookup"><span data-stu-id="e07dc-303">Possible values are: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span></span>|
|<span data-ttu-id="e07dc-304">contentCachingParents</span><span class="sxs-lookup"><span data-stu-id="e07dc-304">contentCachingParents</span></span>|<span data-ttu-id="e07dc-305">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07dc-305">String collection</span></span>|<span data-ttu-id="e07dc-306">Uma lista de endereços IP que representam caches de conteúdo pai.</span><span class="sxs-lookup"><span data-stu-id="e07dc-306">A list of IP addresses representing parent content caches.</span></span>|
|<span data-ttu-id="e07dc-307">contentCachingLogClientIdentities</span><span class="sxs-lookup"><span data-stu-id="e07dc-307">contentCachingLogClientIdentities</span></span>|<span data-ttu-id="e07dc-308">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-308">Boolean</span></span>|<span data-ttu-id="e07dc-309">Habilita o registro em log de endereços IP e portas de clientes que solicitam conteúdo armazenado em cache.</span><span class="sxs-lookup"><span data-stu-id="e07dc-309">Enables logging of IP addresses and ports of clients that request cached content.</span></span>|
|<span data-ttu-id="e07dc-310">contentCachingPublicRanges</span><span class="sxs-lookup"><span data-stu-id="e07dc-310">contentCachingPublicRanges</span></span>|<span data-ttu-id="e07dc-311">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e07dc-311">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="e07dc-312">Uma lista de intervalos IP personalizados que o serviço de cache de conteúdo da Apple deve usar para corresponder clientes a caches de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e07dc-312">A list of custom IP ranges that Apple's content caching service should use to match clients to content caches.</span></span> <span data-ttu-id="e07dc-313">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="e07dc-313">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e07dc-314">contentCachingBlockDeletion</span><span class="sxs-lookup"><span data-stu-id="e07dc-314">contentCachingBlockDeletion</span></span>|<span data-ttu-id="e07dc-315">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-315">Boolean</span></span>|<span data-ttu-id="e07dc-316">Impede que os caches de conteúdo puriem conteúdo para liberar espaço em disco para outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e07dc-316">Prevents content caches from purging content to free up disk space for other apps.</span></span>|
|<span data-ttu-id="e07dc-317">contentCachingShowAlerts</span><span class="sxs-lookup"><span data-stu-id="e07dc-317">contentCachingShowAlerts</span></span>|<span data-ttu-id="e07dc-318">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-318">Boolean</span></span>|<span data-ttu-id="e07dc-319">Exibir alertas de cache de conteúdo como notificações do sistema.</span><span class="sxs-lookup"><span data-stu-id="e07dc-319">Display content caching alerts as system notifications.</span></span>|
|<span data-ttu-id="e07dc-320">contentCachingKeepAwake</span><span class="sxs-lookup"><span data-stu-id="e07dc-320">contentCachingKeepAwake</span></span>|<span data-ttu-id="e07dc-321">Booleano</span><span class="sxs-lookup"><span data-stu-id="e07dc-321">Boolean</span></span>|<span data-ttu-id="e07dc-322">Impedir que o dispositivo adormeça se o cache de conteúdo estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="e07dc-322">Prevent the device from sleeping if content caching is enabled.</span></span>|
|<span data-ttu-id="e07dc-323">contentCachingPort</span><span class="sxs-lookup"><span data-stu-id="e07dc-323">contentCachingPort</span></span>|<span data-ttu-id="e07dc-324">Int32</span><span class="sxs-lookup"><span data-stu-id="e07dc-324">Int32</span></span>|<span data-ttu-id="e07dc-325">Define a porta usada para o cache de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e07dc-325">Sets the port used for content caching.</span></span> <span data-ttu-id="e07dc-326">Se o valor for 0, uma porta disponível aleatória será selecionada.</span><span class="sxs-lookup"><span data-stu-id="e07dc-326">If the value is 0, a random available port will be selected.</span></span> <span data-ttu-id="e07dc-327">Valores válidos de 0 a 65535</span><span class="sxs-lookup"><span data-stu-id="e07dc-327">Valid values 0 to 65535</span></span>|



## <a name="response"></a><span data-ttu-id="e07dc-328">Resposta</span><span class="sxs-lookup"><span data-stu-id="e07dc-328">Response</span></span>
<span data-ttu-id="e07dc-329">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e07dc-329">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e07dc-330">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e07dc-330">Example</span></span>

### <a name="request"></a><span data-ttu-id="e07dc-331">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e07dc-331">Request</span></span>
<span data-ttu-id="e07dc-332">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e07dc-332">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5662

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "Path value",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "Login Window Text value",
  "authorizedUsersListHidden": true,
  "authorizedUsersListHideLocalUsers": true,
  "authorizedUsersListHideMobileAccounts": true,
  "authorizedUsersListIncludeNetworkUsers": true,
  "authorizedUsersListHideAdminUsers": true,
  "authorizedUsersListShowOtherManagedUsers": true,
  "shutDownDisabled": true,
  "restartDisabled": true,
  "sleepDisabled": true,
  "consoleAccessDisabled": true,
  "shutDownDisabledWhileLoggedIn": true,
  "restartDisabledWhileLoggedIn": true,
  "powerOffDisabledWhileLoggedIn": true,
  "logOutDisabledWhileLoggedIn": true,
  "screenLockDisableImmediate": true,
  "associatedDomains": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "appAssociatedDomains": [
    {
      "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
      "applicationIdentifier": "Application Identifier value",
      "domains": [
        "Domains value"
      ],
      "directDownloadsEnabled": true
    }
  ],
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
    "extensionIdentifier": "Extension Identifier value",
    "teamIdentifier": "Team Identifier value",
    "domains": [
      "Domains value"
    ],
    "realm": "Realm value",
    "configurations": [
      {
        "@odata.type": "microsoft.graph.keyStringValuePair",
        "key": "Key value",
        "value": "Value value"
      }
    ]
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  },
  "contentCachingEnabled": true,
  "contentCachingType": "userContentOnly",
  "contentCachingMaxSizeBytes": 10,
  "contentCachingDataPath": "Content Caching Data Path value",
  "contentCachingDisableConnectionSharing": true,
  "contentCachingForceConnectionSharing": true,
  "contentCachingClientPolicy": "clientsInLocalNetwork",
  "contentCachingClientListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerPolicy": "peersInLocalNetwork",
  "contentCachingPeerListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerFilterRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingParentSelectionPolicy": "roundRobin",
  "contentCachingParents": [
    "Content Caching Parents value"
  ],
  "contentCachingLogClientIdentities": true,
  "contentCachingPublicRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingBlockDeletion": true,
  "contentCachingShowAlerts": true,
  "contentCachingKeepAwake": true,
  "contentCachingPort": 2
}
```

### <a name="response"></a><span data-ttu-id="e07dc-333">Resposta</span><span class="sxs-lookup"><span data-stu-id="e07dc-333">Response</span></span>
<span data-ttu-id="e07dc-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e07dc-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5834

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "Path value",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "Login Window Text value",
  "authorizedUsersListHidden": true,
  "authorizedUsersListHideLocalUsers": true,
  "authorizedUsersListHideMobileAccounts": true,
  "authorizedUsersListIncludeNetworkUsers": true,
  "authorizedUsersListHideAdminUsers": true,
  "authorizedUsersListShowOtherManagedUsers": true,
  "shutDownDisabled": true,
  "restartDisabled": true,
  "sleepDisabled": true,
  "consoleAccessDisabled": true,
  "shutDownDisabledWhileLoggedIn": true,
  "restartDisabledWhileLoggedIn": true,
  "powerOffDisabledWhileLoggedIn": true,
  "logOutDisabledWhileLoggedIn": true,
  "screenLockDisableImmediate": true,
  "associatedDomains": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "appAssociatedDomains": [
    {
      "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
      "applicationIdentifier": "Application Identifier value",
      "domains": [
        "Domains value"
      ],
      "directDownloadsEnabled": true
    }
  ],
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
    "extensionIdentifier": "Extension Identifier value",
    "teamIdentifier": "Team Identifier value",
    "domains": [
      "Domains value"
    ],
    "realm": "Realm value",
    "configurations": [
      {
        "@odata.type": "microsoft.graph.keyStringValuePair",
        "key": "Key value",
        "value": "Value value"
      }
    ]
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  },
  "contentCachingEnabled": true,
  "contentCachingType": "userContentOnly",
  "contentCachingMaxSizeBytes": 10,
  "contentCachingDataPath": "Content Caching Data Path value",
  "contentCachingDisableConnectionSharing": true,
  "contentCachingForceConnectionSharing": true,
  "contentCachingClientPolicy": "clientsInLocalNetwork",
  "contentCachingClientListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerPolicy": "peersInLocalNetwork",
  "contentCachingPeerListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerFilterRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingParentSelectionPolicy": "roundRobin",
  "contentCachingParents": [
    "Content Caching Parents value"
  ],
  "contentCachingLogClientIdentities": true,
  "contentCachingPublicRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingBlockDeletion": true,
  "contentCachingShowAlerts": true,
  "contentCachingKeepAwake": true,
  "contentCachingPort": 2
}
```




