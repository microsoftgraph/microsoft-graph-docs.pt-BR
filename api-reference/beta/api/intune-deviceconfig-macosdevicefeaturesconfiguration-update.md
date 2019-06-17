---
title: Atualizar macOSDeviceFeaturesConfiguration
description: Atualizar as propriedades de um objeto macOSDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 780a99d3a298caee1e50d8b85699e9f6a4c2a9af
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976803"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="5fbc8-103">Atualizar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5fbc8-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="5fbc8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5fbc8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5fbc8-106">Atualizar as propriedades de um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5fbc8-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5fbc8-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5fbc8-107">Prerequisites</span></span>
<span data-ttu-id="5fbc8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fbc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fbc8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fbc8-110">Permission type</span></span>|<span data-ttu-id="5fbc8-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5fbc8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5fbc8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fbc8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5fbc8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5fbc8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-115">Not supported.</span></span>|
|<span data-ttu-id="5fbc8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fbc8-116">Application</span></span>|<span data-ttu-id="5fbc8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5fbc8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fbc8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5fbc8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fbc8-119">Request headers</span></span>
|<span data-ttu-id="5fbc8-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5fbc8-120">Header</span></span>|<span data-ttu-id="5fbc8-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5fbc8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5fbc8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fbc8-122">Authorization</span></span>|<span data-ttu-id="5fbc8-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5fbc8-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5fbc8-124">Accept</span></span>|<span data-ttu-id="5fbc8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5fbc8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fbc8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fbc8-126">Request body</span></span>
<span data-ttu-id="5fbc8-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5fbc8-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="5fbc8-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5fbc8-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="5fbc8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fbc8-129">Property</span></span>|<span data-ttu-id="5fbc8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fbc8-130">Type</span></span>|<span data-ttu-id="5fbc8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fbc8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fbc8-132">id</span><span class="sxs-lookup"><span data-stu-id="5fbc8-132">id</span></span>|<span data-ttu-id="5fbc8-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fbc8-133">String</span></span>|<span data-ttu-id="5fbc8-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-134">Key of the entity.</span></span> <span data-ttu-id="5fbc8-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fbc8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5fbc8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5fbc8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fbc8-137">DateTimeOffset</span></span>|<span data-ttu-id="5fbc8-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5fbc8-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fbc8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5fbc8-140">roleScopeTagIds</span></span>|<span data-ttu-id="5fbc8-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fbc8-141">String collection</span></span>|<span data-ttu-id="5fbc8-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5fbc8-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fbc8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5fbc8-144">supportsScopeTags</span></span>|<span data-ttu-id="5fbc8-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-145">Boolean</span></span>|<span data-ttu-id="5fbc8-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5fbc8-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5fbc8-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5fbc8-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-149">This property is read-only.</span></span> <span data-ttu-id="5fbc8-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fbc8-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5fbc8-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="5fbc8-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="5fbc8-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="5fbc8-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="5fbc8-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fbc8-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5fbc8-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="5fbc8-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="5fbc8-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="5fbc8-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="5fbc8-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fbc8-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5fbc8-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="5fbc8-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="5fbc8-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="5fbc8-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="5fbc8-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fbc8-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5fbc8-163">createdDateTime</span></span>|<span data-ttu-id="5fbc8-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fbc8-164">DateTimeOffset</span></span>|<span data-ttu-id="5fbc8-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-165">DateTime the object was created.</span></span> <span data-ttu-id="5fbc8-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fbc8-167">descrição</span><span class="sxs-lookup"><span data-stu-id="5fbc8-167">description</span></span>|<span data-ttu-id="5fbc8-168">String</span><span class="sxs-lookup"><span data-stu-id="5fbc8-168">String</span></span>|<span data-ttu-id="5fbc8-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5fbc8-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fbc8-171">displayName</span><span class="sxs-lookup"><span data-stu-id="5fbc8-171">displayName</span></span>|<span data-ttu-id="5fbc8-172">String</span><span class="sxs-lookup"><span data-stu-id="5fbc8-172">String</span></span>|<span data-ttu-id="5fbc8-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5fbc8-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fbc8-175">versão</span><span class="sxs-lookup"><span data-stu-id="5fbc8-175">version</span></span>|<span data-ttu-id="5fbc8-176">Int32</span><span class="sxs-lookup"><span data-stu-id="5fbc8-176">Int32</span></span>|<span data-ttu-id="5fbc8-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-177">Version of the device configuration.</span></span> <span data-ttu-id="5fbc8-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5fbc8-179">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="5fbc8-179">airPrintDestinations</span></span>|<span data-ttu-id="5fbc8-180">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="5fbc8-181">Uma matriz de impressoras de impressão que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="5fbc8-182">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="5fbc8-183">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="5fbc8-184">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="5fbc8-184">autoLaunchItems</span></span>|<span data-ttu-id="5fbc8-185">coleção [macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="5fbc8-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="5fbc8-186">Lista de aplicativos, arquivos, pastas e outros itens a serem iniciados quando o usuário fizer logon.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="5fbc8-187">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5fbc8-188">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="5fbc8-188">adminShowHostInfo</span></span>|<span data-ttu-id="5fbc8-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-189">Boolean</span></span>|<span data-ttu-id="5fbc8-190">Se deseja mostrar as informações de host de administrador na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="5fbc8-191">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="5fbc8-191">loginWindowText</span></span>|<span data-ttu-id="5fbc8-192">String</span><span class="sxs-lookup"><span data-stu-id="5fbc8-192">String</span></span>|<span data-ttu-id="5fbc8-193">Texto personalizado a ser exibido na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="5fbc8-194">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="5fbc8-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="5fbc8-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-195">Boolean</span></span>|<span data-ttu-id="5fbc8-196">Se deseja mostrar a caixa de diálogo nome e senha ou uma lista de usuários na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="5fbc8-197">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="5fbc8-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="5fbc8-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-198">Boolean</span></span>|<span data-ttu-id="5fbc8-199">Se deseja mostrar somente usuários de rede e de sistema na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="5fbc8-200">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="5fbc8-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="5fbc8-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-201">Boolean</span></span>|<span data-ttu-id="5fbc8-202">Se os usuários móveis serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="5fbc8-203">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="5fbc8-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="5fbc8-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-204">Boolean</span></span>|<span data-ttu-id="5fbc8-205">Se os usuários da rede serão mostrados na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="5fbc8-206">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="5fbc8-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="5fbc8-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-207">Boolean</span></span>|<span data-ttu-id="5fbc8-208">Se os usuários de administrador serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="5fbc8-209">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="5fbc8-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="5fbc8-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-210">Boolean</span></span>|<span data-ttu-id="5fbc8-211">Se deseja mostrar outros usuários na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="5fbc8-212">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="5fbc8-212">shutDownDisabled</span></span>|<span data-ttu-id="5fbc8-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-213">Boolean</span></span>|<span data-ttu-id="5fbc8-214">Se o item de botão desligar será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="5fbc8-215">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="5fbc8-215">restartDisabled</span></span>|<span data-ttu-id="5fbc8-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-216">Boolean</span></span>|<span data-ttu-id="5fbc8-217">Se o item de botão de reinicialização será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="5fbc8-218">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="5fbc8-218">sleepDisabled</span></span>|<span data-ttu-id="5fbc8-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-219">Boolean</span></span>|<span data-ttu-id="5fbc8-220">Se o item de menu de suspensão será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="5fbc8-221">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="5fbc8-221">consoleAccessDisabled</span></span>|<span data-ttu-id="5fbc8-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-222">Boolean</span></span>|<span data-ttu-id="5fbc8-223">Se o outro usuário desconsiderará o uso do>console> nome de usuário especial.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="5fbc8-224">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="5fbc8-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="5fbc8-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-225">Boolean</span></span>|<span data-ttu-id="5fbc8-226">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="5fbc8-227">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="5fbc8-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="5fbc8-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-228">Boolean</span></span>|<span data-ttu-id="5fbc8-229">Se o item de menu reiniciar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="5fbc8-230">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="5fbc8-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="5fbc8-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-231">Boolean</span></span>|<span data-ttu-id="5fbc8-232">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="5fbc8-233">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="5fbc8-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="5fbc8-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-234">Boolean</span></span>|<span data-ttu-id="5fbc8-235">Se o item de menu fazer logout na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="5fbc8-236">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="5fbc8-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="5fbc8-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fbc8-237">Boolean</span></span>|<span data-ttu-id="5fbc8-238">Se as funções de bloqueio de tela imediata serão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-238">Whether to disable the immediate screen lock functions.</span></span>|



## <a name="response"></a><span data-ttu-id="5fbc8-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fbc8-239">Response</span></span>
<span data-ttu-id="5fbc8-240">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-240">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fbc8-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5fbc8-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="5fbc8-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fbc8-242">Request</span></span>
<span data-ttu-id="5fbc8-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2107

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
  "screenLockDisableImmediate": true
}
```

### <a name="response"></a><span data-ttu-id="5fbc8-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fbc8-244">Response</span></span>
<span data-ttu-id="5fbc8-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5fbc8-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2279

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
  "screenLockDisableImmediate": true
}
```





