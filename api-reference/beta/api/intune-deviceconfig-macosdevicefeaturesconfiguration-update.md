---
title: Atualizar macOSDeviceFeaturesConfiguration
description: Atualizar as propriedades de um objeto macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ddab518e5ab2e2aa4b61c71d45166419e0869631
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177902"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="83f52-103">Atualizar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="83f52-103">Update macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="83f52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83f52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83f52-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83f52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83f52-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83f52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83f52-107">Atualizar as propriedades de um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83f52-107">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83f52-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83f52-108">Prerequisites</span></span>
<span data-ttu-id="83f52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83f52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83f52-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="83f52-111">Permission type</span></span>|<span data-ttu-id="83f52-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="83f52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83f52-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="83f52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83f52-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83f52-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83f52-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="83f52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83f52-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="83f52-116">Not supported.</span></span>|
|<span data-ttu-id="83f52-117">Application</span><span class="sxs-lookup"><span data-stu-id="83f52-117">Application</span></span>|<span data-ttu-id="83f52-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83f52-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83f52-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83f52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="83f52-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83f52-120">Request headers</span></span>
|<span data-ttu-id="83f52-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83f52-121">Header</span></span>|<span data-ttu-id="83f52-122">Valor</span><span class="sxs-lookup"><span data-stu-id="83f52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83f52-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="83f52-123">Authorization</span></span>|<span data-ttu-id="83f52-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83f52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83f52-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="83f52-125">Accept</span></span>|<span data-ttu-id="83f52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83f52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83f52-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83f52-127">Request body</span></span>
<span data-ttu-id="83f52-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83f52-128">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="83f52-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83f52-129">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="83f52-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83f52-130">Property</span></span>|<span data-ttu-id="83f52-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="83f52-131">Type</span></span>|<span data-ttu-id="83f52-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="83f52-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83f52-133">id</span><span class="sxs-lookup"><span data-stu-id="83f52-133">id</span></span>|<span data-ttu-id="83f52-134">String</span><span class="sxs-lookup"><span data-stu-id="83f52-134">String</span></span>|<span data-ttu-id="83f52-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="83f52-135">Key of the entity.</span></span> <span data-ttu-id="83f52-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83f52-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83f52-137">lastModifiedDateTime</span></span>|<span data-ttu-id="83f52-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83f52-138">DateTimeOffset</span></span>|<span data-ttu-id="83f52-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="83f52-139">DateTime the object was last modified.</span></span> <span data-ttu-id="83f52-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83f52-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83f52-141">roleScopeTagIds</span></span>|<span data-ttu-id="83f52-142">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="83f52-142">String collection</span></span>|<span data-ttu-id="83f52-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="83f52-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83f52-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83f52-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="83f52-145">supportsScopeTags</span></span>|<span data-ttu-id="83f52-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-146">Boolean</span></span>|<span data-ttu-id="83f52-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="83f52-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="83f52-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="83f52-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="83f52-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="83f52-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="83f52-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83f52-150">This property is read-only.</span></span> <span data-ttu-id="83f52-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83f52-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83f52-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="83f52-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83f52-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="83f52-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="83f52-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="83f52-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83f52-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83f52-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="83f52-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83f52-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="83f52-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="83f52-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="83f52-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83f52-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="83f52-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="83f52-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="83f52-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="83f52-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="83f52-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="83f52-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83f52-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83f52-164">createdDateTime</span></span>|<span data-ttu-id="83f52-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83f52-165">DateTimeOffset</span></span>|<span data-ttu-id="83f52-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="83f52-166">DateTime the object was created.</span></span> <span data-ttu-id="83f52-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83f52-168">description</span><span class="sxs-lookup"><span data-stu-id="83f52-168">description</span></span>|<span data-ttu-id="83f52-169">String</span><span class="sxs-lookup"><span data-stu-id="83f52-169">String</span></span>|<span data-ttu-id="83f52-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83f52-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83f52-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83f52-172">displayName</span><span class="sxs-lookup"><span data-stu-id="83f52-172">displayName</span></span>|<span data-ttu-id="83f52-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83f52-173">String</span></span>|<span data-ttu-id="83f52-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83f52-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83f52-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83f52-176">versão</span><span class="sxs-lookup"><span data-stu-id="83f52-176">version</span></span>|<span data-ttu-id="83f52-177">Int32</span><span class="sxs-lookup"><span data-stu-id="83f52-177">Int32</span></span>|<span data-ttu-id="83f52-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="83f52-178">Version of the device configuration.</span></span> <span data-ttu-id="83f52-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83f52-180">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="83f52-180">airPrintDestinations</span></span>|<span data-ttu-id="83f52-181">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="83f52-182">Uma matriz de impressoras de impressão que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="83f52-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="83f52-183">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="83f52-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="83f52-184">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="83f52-185">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="83f52-185">autoLaunchItems</span></span>|<span data-ttu-id="83f52-186">coleção [macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="83f52-187">Lista de aplicativos, arquivos, pastas e outros itens a serem iniciados quando o usuário fizer logon.</span><span class="sxs-lookup"><span data-stu-id="83f52-187">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="83f52-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="83f52-188">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="83f52-189">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="83f52-189">adminShowHostInfo</span></span>|<span data-ttu-id="83f52-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-190">Boolean</span></span>|<span data-ttu-id="83f52-191">Se deseja mostrar as informações de host de administrador na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="83f52-191">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="83f52-192">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="83f52-192">loginWindowText</span></span>|<span data-ttu-id="83f52-193">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="83f52-193">String</span></span>|<span data-ttu-id="83f52-194">Texto personalizado a ser exibido na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="83f52-194">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="83f52-195">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="83f52-195">authorizedUsersListHidden</span></span>|<span data-ttu-id="83f52-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-196">Boolean</span></span>|<span data-ttu-id="83f52-197">Se deseja mostrar a caixa de diálogo nome e senha ou uma lista de usuários na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="83f52-197">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="83f52-198">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="83f52-198">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="83f52-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-199">Boolean</span></span>|<span data-ttu-id="83f52-200">Se deseja mostrar somente usuários de rede e de sistema na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="83f52-200">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="83f52-201">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="83f52-201">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="83f52-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-202">Boolean</span></span>|<span data-ttu-id="83f52-203">Se os usuários móveis serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="83f52-203">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="83f52-204">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="83f52-204">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="83f52-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-205">Boolean</span></span>|<span data-ttu-id="83f52-206">Se os usuários da rede serão mostrados na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="83f52-206">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="83f52-207">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="83f52-207">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="83f52-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-208">Boolean</span></span>|<span data-ttu-id="83f52-209">Se os usuários de administrador serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="83f52-209">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="83f52-210">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="83f52-210">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="83f52-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-211">Boolean</span></span>|<span data-ttu-id="83f52-212">Se deseja mostrar outros usuários na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="83f52-212">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="83f52-213">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="83f52-213">shutDownDisabled</span></span>|<span data-ttu-id="83f52-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-214">Boolean</span></span>|<span data-ttu-id="83f52-215">Se o item de botão desligar será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="83f52-215">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="83f52-216">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="83f52-216">restartDisabled</span></span>|<span data-ttu-id="83f52-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-217">Boolean</span></span>|<span data-ttu-id="83f52-218">Se o item de botão de reinicialização será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="83f52-218">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="83f52-219">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="83f52-219">sleepDisabled</span></span>|<span data-ttu-id="83f52-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-220">Boolean</span></span>|<span data-ttu-id="83f52-221">Se o item de menu de suspensão será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="83f52-221">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="83f52-222">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="83f52-222">consoleAccessDisabled</span></span>|<span data-ttu-id="83f52-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-223">Boolean</span></span>|<span data-ttu-id="83f52-224">Se o outro usuário desconsiderará o uso do>console> nome de usuário especial.</span><span class="sxs-lookup"><span data-stu-id="83f52-224">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="83f52-225">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="83f52-225">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="83f52-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-226">Boolean</span></span>|<span data-ttu-id="83f52-227">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="83f52-227">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="83f52-228">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="83f52-228">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="83f52-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-229">Boolean</span></span>|<span data-ttu-id="83f52-230">Se o item de menu reiniciar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="83f52-230">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="83f52-231">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="83f52-231">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="83f52-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-232">Boolean</span></span>|<span data-ttu-id="83f52-233">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="83f52-233">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="83f52-234">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="83f52-234">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="83f52-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-235">Boolean</span></span>|<span data-ttu-id="83f52-236">Se o item de menu fazer logout na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="83f52-236">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="83f52-237">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="83f52-237">screenLockDisableImmediate</span></span>|<span data-ttu-id="83f52-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="83f52-238">Boolean</span></span>|<span data-ttu-id="83f52-239">Se as funções de bloqueio de tela imediata serão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="83f52-239">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="83f52-240">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="83f52-240">associatedDomains</span></span>|<span data-ttu-id="83f52-241">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="83f52-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="83f52-242">Obtém ou define uma lista que mapeia aplicativos para seus domínios associados.</span><span class="sxs-lookup"><span data-stu-id="83f52-242">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="83f52-243">A chave deve corresponder à ID do aplicativo, e o valor deve ser uma cadeia de caracteres no formato "Service: domain" onde domínio é um nome de host totalmente qualificado (por exemplo, webcredentials:example. com).</span><span class="sxs-lookup"><span data-stu-id="83f52-243">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="83f52-244">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="83f52-244">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="83f52-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="83f52-245">singleSignOnExtension</span></span>|[<span data-ttu-id="83f52-246">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="83f52-246">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="83f52-247">Obtém ou define um perfil de extensão de logon único.</span><span class="sxs-lookup"><span data-stu-id="83f52-247">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="83f52-248">Preterido: Use MacOSSingleSignOnExtension em vez disso.</span><span class="sxs-lookup"><span data-stu-id="83f52-248">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="83f52-249">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="83f52-249">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="83f52-250">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="83f52-250">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="83f52-251">Obtém ou define um perfil de extensão de logon único.</span><span class="sxs-lookup"><span data-stu-id="83f52-251">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="83f52-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="83f52-252">Response</span></span>
<span data-ttu-id="83f52-253">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83f52-253">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83f52-254">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83f52-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="83f52-255">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83f52-255">Request</span></span>
<span data-ttu-id="83f52-256">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83f52-256">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3879

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
  }
}
```

### <a name="response"></a><span data-ttu-id="83f52-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="83f52-257">Response</span></span>
<span data-ttu-id="83f52-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83f52-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4051

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
  }
}
```



