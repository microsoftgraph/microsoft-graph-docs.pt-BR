---
title: Atualizar macOSDeviceFeaturesConfiguration
description: Atualizar as propriedades de um objeto macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 502f307bb7244cf6bec364aebf6714a6881262e5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733011"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="6ab0b-103">Atualizar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ab0b-103">Update macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="6ab0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ab0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ab0b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ab0b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ab0b-107">Atualizar as propriedades de um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ab0b-107">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ab0b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ab0b-108">Prerequisites</span></span>
<span data-ttu-id="6ab0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ab0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ab0b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ab0b-111">Permission type</span></span>|<span data-ttu-id="6ab0b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ab0b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ab0b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ab0b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ab0b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ab0b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-116">Not supported.</span></span>|
|<span data-ttu-id="6ab0b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ab0b-117">Application</span></span>|<span data-ttu-id="6ab0b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ab0b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ab0b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ab0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6ab0b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ab0b-120">Request headers</span></span>
|<span data-ttu-id="6ab0b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ab0b-121">Header</span></span>|<span data-ttu-id="6ab0b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ab0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ab0b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ab0b-123">Authorization</span></span>|<span data-ttu-id="6ab0b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ab0b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ab0b-125">Accept</span></span>|<span data-ttu-id="6ab0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ab0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ab0b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ab0b-127">Request body</span></span>
<span data-ttu-id="6ab0b-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ab0b-128">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="6ab0b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6ab0b-129">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="6ab0b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ab0b-130">Property</span></span>|<span data-ttu-id="6ab0b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ab0b-131">Type</span></span>|<span data-ttu-id="6ab0b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ab0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ab0b-133">id</span><span class="sxs-lookup"><span data-stu-id="6ab0b-133">id</span></span>|<span data-ttu-id="6ab0b-134">String</span><span class="sxs-lookup"><span data-stu-id="6ab0b-134">String</span></span>|<span data-ttu-id="6ab0b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-135">Key of the entity.</span></span> <span data-ttu-id="6ab0b-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ab0b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ab0b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6ab0b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ab0b-138">DateTimeOffset</span></span>|<span data-ttu-id="6ab0b-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6ab0b-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ab0b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6ab0b-141">roleScopeTagIds</span></span>|<span data-ttu-id="6ab0b-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ab0b-142">String collection</span></span>|<span data-ttu-id="6ab0b-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6ab0b-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ab0b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6ab0b-145">supportsScopeTags</span></span>|<span data-ttu-id="6ab0b-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-146">Boolean</span></span>|<span data-ttu-id="6ab0b-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6ab0b-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6ab0b-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6ab0b-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-150">This property is read-only.</span></span> <span data-ttu-id="6ab0b-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ab0b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6ab0b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6ab0b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6ab0b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6ab0b-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6ab0b-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ab0b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6ab0b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6ab0b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6ab0b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6ab0b-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6ab0b-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ab0b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6ab0b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6ab0b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6ab0b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6ab0b-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6ab0b-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ab0b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ab0b-164">createdDateTime</span></span>|<span data-ttu-id="6ab0b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ab0b-165">DateTimeOffset</span></span>|<span data-ttu-id="6ab0b-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-166">DateTime the object was created.</span></span> <span data-ttu-id="6ab0b-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ab0b-168">description</span><span class="sxs-lookup"><span data-stu-id="6ab0b-168">description</span></span>|<span data-ttu-id="6ab0b-169">String</span><span class="sxs-lookup"><span data-stu-id="6ab0b-169">String</span></span>|<span data-ttu-id="6ab0b-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6ab0b-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ab0b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6ab0b-172">displayName</span></span>|<span data-ttu-id="6ab0b-173">String</span><span class="sxs-lookup"><span data-stu-id="6ab0b-173">String</span></span>|<span data-ttu-id="6ab0b-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6ab0b-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ab0b-176">versão</span><span class="sxs-lookup"><span data-stu-id="6ab0b-176">version</span></span>|<span data-ttu-id="6ab0b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6ab0b-177">Int32</span></span>|<span data-ttu-id="6ab0b-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-178">Version of the device configuration.</span></span> <span data-ttu-id="6ab0b-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6ab0b-180">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="6ab0b-180">airPrintDestinations</span></span>|<span data-ttu-id="6ab0b-181">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="6ab0b-182">Uma matriz de impressoras de impressão que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="6ab0b-183">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6ab0b-184">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="6ab0b-185">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="6ab0b-185">autoLaunchItems</span></span>|<span data-ttu-id="6ab0b-186">coleção [macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="6ab0b-187">Lista de aplicativos, arquivos, pastas e outros itens a serem iniciados quando o usuário fizer logon.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-187">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="6ab0b-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-188">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6ab0b-189">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="6ab0b-189">adminShowHostInfo</span></span>|<span data-ttu-id="6ab0b-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-190">Boolean</span></span>|<span data-ttu-id="6ab0b-191">Se deseja mostrar as informações de host de administrador na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-191">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="6ab0b-192">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="6ab0b-192">loginWindowText</span></span>|<span data-ttu-id="6ab0b-193">String</span><span class="sxs-lookup"><span data-stu-id="6ab0b-193">String</span></span>|<span data-ttu-id="6ab0b-194">Texto personalizado a ser exibido na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-194">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="6ab0b-195">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="6ab0b-195">authorizedUsersListHidden</span></span>|<span data-ttu-id="6ab0b-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-196">Boolean</span></span>|<span data-ttu-id="6ab0b-197">Se deseja mostrar a caixa de diálogo nome e senha ou uma lista de usuários na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-197">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="6ab0b-198">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="6ab0b-198">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="6ab0b-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-199">Boolean</span></span>|<span data-ttu-id="6ab0b-200">Se deseja mostrar somente usuários de rede e de sistema na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-200">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6ab0b-201">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="6ab0b-201">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="6ab0b-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-202">Boolean</span></span>|<span data-ttu-id="6ab0b-203">Se os usuários móveis serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-203">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6ab0b-204">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="6ab0b-204">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="6ab0b-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-205">Boolean</span></span>|<span data-ttu-id="6ab0b-206">Se os usuários da rede serão mostrados na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-206">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6ab0b-207">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="6ab0b-207">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="6ab0b-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-208">Boolean</span></span>|<span data-ttu-id="6ab0b-209">Se os usuários de administrador serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-209">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6ab0b-210">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="6ab0b-210">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="6ab0b-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-211">Boolean</span></span>|<span data-ttu-id="6ab0b-212">Se deseja mostrar outros usuários na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-212">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6ab0b-213">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="6ab0b-213">shutDownDisabled</span></span>|<span data-ttu-id="6ab0b-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-214">Boolean</span></span>|<span data-ttu-id="6ab0b-215">Se o item de botão desligar será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-215">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="6ab0b-216">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="6ab0b-216">restartDisabled</span></span>|<span data-ttu-id="6ab0b-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-217">Boolean</span></span>|<span data-ttu-id="6ab0b-218">Se o item de botão de reinicialização será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-218">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="6ab0b-219">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="6ab0b-219">sleepDisabled</span></span>|<span data-ttu-id="6ab0b-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-220">Boolean</span></span>|<span data-ttu-id="6ab0b-221">Se o item de menu de suspensão será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-221">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="6ab0b-222">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="6ab0b-222">consoleAccessDisabled</span></span>|<span data-ttu-id="6ab0b-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-223">Boolean</span></span>|<span data-ttu-id="6ab0b-224">Se o outro usuário desconsiderará o uso do>console> nome de usuário especial.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-224">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="6ab0b-225">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="6ab0b-225">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="6ab0b-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-226">Boolean</span></span>|<span data-ttu-id="6ab0b-227">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-227">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="6ab0b-228">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="6ab0b-228">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="6ab0b-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-229">Boolean</span></span>|<span data-ttu-id="6ab0b-230">Se o item de menu reiniciar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-230">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="6ab0b-231">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="6ab0b-231">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="6ab0b-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-232">Boolean</span></span>|<span data-ttu-id="6ab0b-233">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-233">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="6ab0b-234">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="6ab0b-234">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="6ab0b-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-235">Boolean</span></span>|<span data-ttu-id="6ab0b-236">Se o item de menu fazer logout na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-236">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="6ab0b-237">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="6ab0b-237">screenLockDisableImmediate</span></span>|<span data-ttu-id="6ab0b-238">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-238">Boolean</span></span>|<span data-ttu-id="6ab0b-239">Se as funções de bloqueio de tela imediata serão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-239">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="6ab0b-240">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="6ab0b-240">associatedDomains</span></span>|<span data-ttu-id="6ab0b-241">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6ab0b-242">Preterido: Use appAssociatedDomains em vez disso.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-242">DEPRECATED: use appAssociatedDomains instead.</span></span> <span data-ttu-id="6ab0b-243">Obtém ou define uma lista que mapeia aplicativos para seus domínios associados.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-243">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="6ab0b-244">A chave deve corresponder à ID do aplicativo, e o valor deve ser uma cadeia de caracteres no formato "Service: domain" onde domínio é um nome de host totalmente qualificado (por exemplo, webcredentials:example. com).</span><span class="sxs-lookup"><span data-stu-id="6ab0b-244">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="6ab0b-245">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-245">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6ab0b-246">appAssociatedDomains</span><span class="sxs-lookup"><span data-stu-id="6ab0b-246">appAssociatedDomains</span></span>|<span data-ttu-id="6ab0b-247">coleção [macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-247">[macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md) collection</span></span>|<span data-ttu-id="6ab0b-248">Obtém ou define uma lista que mapeia aplicativos para seus domínios associados.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-248">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="6ab0b-249">Os identificadores de aplicativo devem ser exclusivos.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-249">Application identifiers must be unique.</span></span> <span data-ttu-id="6ab0b-250">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-250">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6ab0b-251">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="6ab0b-251">singleSignOnExtension</span></span>|[<span data-ttu-id="6ab0b-252">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="6ab0b-252">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="6ab0b-253">Obtém ou define um perfil de extensão de logon único.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-253">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="6ab0b-254">Preterido: Use MacOSSingleSignOnExtension em vez disso.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-254">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="6ab0b-255">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="6ab0b-255">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="6ab0b-256">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="6ab0b-256">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="6ab0b-257">Obtém ou define um perfil de extensão de logon único.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-257">Gets or sets a single sign-on extension profile.</span></span>|
|<span data-ttu-id="6ab0b-258">contentCachingEnabled</span><span class="sxs-lookup"><span data-stu-id="6ab0b-258">contentCachingEnabled</span></span>|<span data-ttu-id="6ab0b-259">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-259">Boolean</span></span>|<span data-ttu-id="6ab0b-260">Habilita o cache de conteúdo e impede que ele seja desabilitado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-260">Enables content caching and prevents it from being disabled by the user.</span></span>|
|<span data-ttu-id="6ab0b-261">contentCachingType</span><span class="sxs-lookup"><span data-stu-id="6ab0b-261">contentCachingType</span></span>|[<span data-ttu-id="6ab0b-262">macOSContentCachingType</span><span class="sxs-lookup"><span data-stu-id="6ab0b-262">macOSContentCachingType</span></span>](../resources/intune-deviceconfig-macoscontentcachingtype.md)|<span data-ttu-id="6ab0b-263">Determina o tipo de conteúdo que pode ser armazenado em cache pelo serviço de cache de conteúdo da Apple.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-263">Determines what type of content is allowed to be cached by Apple's content caching service.</span></span> <span data-ttu-id="6ab0b-264">Os valores possíveis são: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-264">Possible values are: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span></span>|
|<span data-ttu-id="6ab0b-265">contentCachingMaxSizeBytes</span><span class="sxs-lookup"><span data-stu-id="6ab0b-265">contentCachingMaxSizeBytes</span></span>|<span data-ttu-id="6ab0b-266">Int32</span><span class="sxs-lookup"><span data-stu-id="6ab0b-266">Int32</span></span>|<span data-ttu-id="6ab0b-267">O número máximo de bytes de espaço em disco que serão usados para o cache de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-267">The maximum number of bytes of disk space that will be used for the content cache.</span></span> <span data-ttu-id="6ab0b-268">Um valor de 0 (padrão) indica espaço em disco ilimitado.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-268">A value of 0 (default) indicates unlimited disk space.</span></span> |
|<span data-ttu-id="6ab0b-269">contentCachingDataPath</span><span class="sxs-lookup"><span data-stu-id="6ab0b-269">contentCachingDataPath</span></span>|<span data-ttu-id="6ab0b-270">String</span><span class="sxs-lookup"><span data-stu-id="6ab0b-270">String</span></span>|<span data-ttu-id="6ab0b-271">O caminho para o diretório usado para armazenar o conteúdo em cache.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-271">The path to the directory used to store cached content.</span></span> <span data-ttu-id="6ab0b-272">O valor deve ser (ou terminar com)/Library/Application Support/Apple/AssetCache/data</span><span class="sxs-lookup"><span data-stu-id="6ab0b-272">The value must be (or end with) /Library/Application Support/Apple/AssetCache/Data</span></span>|
|<span data-ttu-id="6ab0b-273">contentCachingDisableConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="6ab0b-273">contentCachingDisableConnectionSharing</span></span>|<span data-ttu-id="6ab0b-274">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-274">Boolean</span></span>|<span data-ttu-id="6ab0b-275">Desabilita o compartilhamento de conexão com a Internet.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-275">Disables internet connection sharing.</span></span>|
|<span data-ttu-id="6ab0b-276">contentCachingForceConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="6ab0b-276">contentCachingForceConnectionSharing</span></span>|<span data-ttu-id="6ab0b-277">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-277">Boolean</span></span>|<span data-ttu-id="6ab0b-278">Força o compartilhamento de conexão com a Internet.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-278">Forces internet connection sharing.</span></span> <span data-ttu-id="6ab0b-279">contentCachingDisableConnectionSharing substitui essa configuração.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-279">contentCachingDisableConnectionSharing overrides this setting.</span></span>|
|<span data-ttu-id="6ab0b-280">contentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="6ab0b-280">contentCachingClientPolicy</span></span>|[<span data-ttu-id="6ab0b-281">macOSContentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="6ab0b-281">macOSContentCachingClientPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|<span data-ttu-id="6ab0b-282">Determina o método no qual os servidores de cache de conteúdo ouvirão clientes.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-282">Determines the method in which content caching servers will listen for clients.</span></span> <span data-ttu-id="6ab0b-283">Os valores possíveis são: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-283">Possible values are: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span></span>|
|<span data-ttu-id="6ab0b-284">contentCachingClientListenRanges</span><span class="sxs-lookup"><span data-stu-id="6ab0b-284">contentCachingClientListenRanges</span></span>|<span data-ttu-id="6ab0b-285">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-285">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="6ab0b-286">Uma lista de caches de conteúdo de intervalos de IP personalizados que será usada para escutar clientes.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-286">A list of custom IP ranges content caches will use to listen for clients.</span></span> <span data-ttu-id="6ab0b-287">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-287">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6ab0b-288">contentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="6ab0b-288">contentCachingPeerPolicy</span></span>|[<span data-ttu-id="6ab0b-289">macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="6ab0b-289">macOSContentCachingPeerPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|<span data-ttu-id="6ab0b-290">Determina o método no qual o conteúdo armazena em cache ponto com outros caches.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-290">Determines the method in which content caches peer with other caches.</span></span> <span data-ttu-id="6ab0b-291">Os valores possíveis são: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-291">Possible values are: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span></span>|
|<span data-ttu-id="6ab0b-292">contentCachingPeerListenRanges</span><span class="sxs-lookup"><span data-stu-id="6ab0b-292">contentCachingPeerListenRanges</span></span>|<span data-ttu-id="6ab0b-293">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-293">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="6ab0b-294">Uma lista de caches de conteúdo de intervalos de IP personalizados que será usada para escutar em caches de par.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-294">A list of custom IP ranges content caches will use to listen for peer caches.</span></span> <span data-ttu-id="6ab0b-295">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-295">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6ab0b-296">contentCachingPeerFilterRanges</span><span class="sxs-lookup"><span data-stu-id="6ab0b-296">contentCachingPeerFilterRanges</span></span>|<span data-ttu-id="6ab0b-297">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-297">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="6ab0b-298">Uma lista de caches de conteúdo de intervalos de IP personalizados que usará para consultar conteúdo de caches de mesmo nível.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-298">A list of custom IP ranges content caches will use to query for content from peers caches.</span></span> <span data-ttu-id="6ab0b-299">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-299">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6ab0b-300">contentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="6ab0b-300">contentCachingParentSelectionPolicy</span></span>|[<span data-ttu-id="6ab0b-301">macOSContentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="6ab0b-301">macOSContentCachingParentSelectionPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|<span data-ttu-id="6ab0b-302">Determina o método no qual os servidores de cache de conteúdo selecionarão pais, se houver vários.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-302">Determines the method in which content caching servers will select parents if multiple are present.</span></span> <span data-ttu-id="6ab0b-303">Os possíveis valores são: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-303">Possible values are: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span></span>|
|<span data-ttu-id="6ab0b-304">contentCachingParents</span><span class="sxs-lookup"><span data-stu-id="6ab0b-304">contentCachingParents</span></span>|<span data-ttu-id="6ab0b-305">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ab0b-305">String collection</span></span>|<span data-ttu-id="6ab0b-306">Uma lista de endereços IP que representam caches de conteúdo pai.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-306">A list of IP addresses representing parent content caches.</span></span>|
|<span data-ttu-id="6ab0b-307">contentCachingLogClientIdentities</span><span class="sxs-lookup"><span data-stu-id="6ab0b-307">contentCachingLogClientIdentities</span></span>|<span data-ttu-id="6ab0b-308">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-308">Boolean</span></span>|<span data-ttu-id="6ab0b-309">Permite o registro em log de endereços IP e portas de clientes que solicitam conteúdo em cache.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-309">Enables logging of IP addresses and ports of clients that request cached content.</span></span>|
|<span data-ttu-id="6ab0b-310">contentCachingPublicRanges</span><span class="sxs-lookup"><span data-stu-id="6ab0b-310">contentCachingPublicRanges</span></span>|<span data-ttu-id="6ab0b-311">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="6ab0b-311">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="6ab0b-312">Uma lista de intervalos de IP personalizados que o serviço de cache de conteúdo da Apple deve usar para fazer a correspondência de clientes com caches de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-312">A list of custom IP ranges that Apple's content caching service should use to match clients to content caches.</span></span> <span data-ttu-id="6ab0b-313">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-313">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6ab0b-314">contentCachingBlockDeletion</span><span class="sxs-lookup"><span data-stu-id="6ab0b-314">contentCachingBlockDeletion</span></span>|<span data-ttu-id="6ab0b-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-315">Boolean</span></span>|<span data-ttu-id="6ab0b-316">Impede que caches de conteúdo limpem conteúdo para liberar espaço em disco para outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-316">Prevents content caches from purging content to free up disk space for other apps.</span></span>|
|<span data-ttu-id="6ab0b-317">contentCachingShowAlerts</span><span class="sxs-lookup"><span data-stu-id="6ab0b-317">contentCachingShowAlerts</span></span>|<span data-ttu-id="6ab0b-318">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-318">Boolean</span></span>|<span data-ttu-id="6ab0b-319">Exibir alertas de cache de conteúdo como notificações do sistema.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-319">Display content caching alerts as system notifications.</span></span>|
|<span data-ttu-id="6ab0b-320">contentCachingKeepAwake</span><span class="sxs-lookup"><span data-stu-id="6ab0b-320">contentCachingKeepAwake</span></span>|<span data-ttu-id="6ab0b-321">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ab0b-321">Boolean</span></span>|<span data-ttu-id="6ab0b-322">Impedir que o dispositivo fique dormindo se o cache de conteúdo estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-322">Prevent the device from sleeping if content caching is enabled.</span></span>|
|<span data-ttu-id="6ab0b-323">contentCachingPort</span><span class="sxs-lookup"><span data-stu-id="6ab0b-323">contentCachingPort</span></span>|<span data-ttu-id="6ab0b-324">Int32</span><span class="sxs-lookup"><span data-stu-id="6ab0b-324">Int32</span></span>|<span data-ttu-id="6ab0b-325">Define a porta usada para o cache de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-325">Sets the port used for content caching.</span></span> <span data-ttu-id="6ab0b-326">Se o valor for 0, uma porta aleatória disponível será selecionada.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-326">If the value is 0, a random available port will be selected.</span></span> <span data-ttu-id="6ab0b-327">Valores válidos de 0 a 65535</span><span class="sxs-lookup"><span data-stu-id="6ab0b-327">Valid values 0 to 65535</span></span>|



## <a name="response"></a><span data-ttu-id="6ab0b-328">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ab0b-328">Response</span></span>
<span data-ttu-id="6ab0b-329">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-329">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ab0b-330">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ab0b-330">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ab0b-331">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ab0b-331">Request</span></span>
<span data-ttu-id="6ab0b-332">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-332">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6ab0b-333">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ab0b-333">Response</span></span>
<span data-ttu-id="6ab0b-p130">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ab0b-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





