---
title: Atualizar macOSDeviceFeaturesConfiguration
description: Atualizar as propriedades de um objeto macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2e5b0c7094bbbf8ca93edd61d05cf8d17b154967
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066100"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="b3fa2-103">Atualizar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3fa2-103">Update macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="b3fa2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3fa2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3fa2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3fa2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3fa2-107">Atualizar as propriedades de um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3fa2-107">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3fa2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b3fa2-108">Prerequisites</span></span>
<span data-ttu-id="b3fa2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3fa2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3fa2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3fa2-111">Permission type</span></span>|<span data-ttu-id="b3fa2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3fa2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3fa2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3fa2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3fa2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3fa2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-116">Not supported.</span></span>|
|<span data-ttu-id="b3fa2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3fa2-117">Application</span></span>|<span data-ttu-id="b3fa2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3fa2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3fa2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3fa2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b3fa2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3fa2-120">Request headers</span></span>
|<span data-ttu-id="b3fa2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b3fa2-121">Header</span></span>|<span data-ttu-id="b3fa2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b3fa2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3fa2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3fa2-123">Authorization</span></span>|<span data-ttu-id="b3fa2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3fa2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b3fa2-125">Accept</span></span>|<span data-ttu-id="b3fa2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3fa2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3fa2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3fa2-127">Request body</span></span>
<span data-ttu-id="b3fa2-128">No corpo da solicitação, forneça uma representação JSON do objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3fa2-128">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="b3fa2-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b3fa2-129">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="b3fa2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3fa2-130">Property</span></span>|<span data-ttu-id="b3fa2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3fa2-131">Type</span></span>|<span data-ttu-id="b3fa2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3fa2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3fa2-133">id</span><span class="sxs-lookup"><span data-stu-id="b3fa2-133">id</span></span>|<span data-ttu-id="b3fa2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3fa2-134">String</span></span>|<span data-ttu-id="b3fa2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-135">Key of the entity.</span></span> <span data-ttu-id="b3fa2-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3fa2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3fa2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b3fa2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3fa2-138">DateTimeOffset</span></span>|<span data-ttu-id="b3fa2-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b3fa2-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3fa2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3fa2-141">roleScopeTagIds</span></span>|<span data-ttu-id="b3fa2-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3fa2-142">String collection</span></span>|<span data-ttu-id="b3fa2-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b3fa2-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3fa2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b3fa2-145">supportsScopeTags</span></span>|<span data-ttu-id="b3fa2-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-146">Boolean</span></span>|<span data-ttu-id="b3fa2-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b3fa2-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b3fa2-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b3fa2-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-150">This property is read-only.</span></span> <span data-ttu-id="b3fa2-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3fa2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b3fa2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b3fa2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b3fa2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b3fa2-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b3fa2-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3fa2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3fa2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b3fa2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b3fa2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b3fa2-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b3fa2-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3fa2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b3fa2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b3fa2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b3fa2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b3fa2-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b3fa2-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3fa2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3fa2-164">createdDateTime</span></span>|<span data-ttu-id="b3fa2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3fa2-165">DateTimeOffset</span></span>|<span data-ttu-id="b3fa2-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-166">DateTime the object was created.</span></span> <span data-ttu-id="b3fa2-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3fa2-168">description</span><span class="sxs-lookup"><span data-stu-id="b3fa2-168">description</span></span>|<span data-ttu-id="b3fa2-169">String</span><span class="sxs-lookup"><span data-stu-id="b3fa2-169">String</span></span>|<span data-ttu-id="b3fa2-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b3fa2-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3fa2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b3fa2-172">displayName</span></span>|<span data-ttu-id="b3fa2-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3fa2-173">String</span></span>|<span data-ttu-id="b3fa2-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b3fa2-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3fa2-176">versão</span><span class="sxs-lookup"><span data-stu-id="b3fa2-176">version</span></span>|<span data-ttu-id="b3fa2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b3fa2-177">Int32</span></span>|<span data-ttu-id="b3fa2-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-178">Version of the device configuration.</span></span> <span data-ttu-id="b3fa2-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3fa2-180">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="b3fa2-180">airPrintDestinations</span></span>|<span data-ttu-id="b3fa2-181">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="b3fa2-182">Uma matriz de impressoras de impressão que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="b3fa2-183">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="b3fa2-184">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="b3fa2-185">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="b3fa2-185">autoLaunchItems</span></span>|<span data-ttu-id="b3fa2-186">coleção [macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="b3fa2-187">Lista de aplicativos, arquivos, pastas e outros itens a serem iniciados quando o usuário fizer logon.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-187">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="b3fa2-188">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-188">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b3fa2-189">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="b3fa2-189">adminShowHostInfo</span></span>|<span data-ttu-id="b3fa2-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-190">Boolean</span></span>|<span data-ttu-id="b3fa2-191">Se deseja mostrar as informações de host de administrador na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-191">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="b3fa2-192">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="b3fa2-192">loginWindowText</span></span>|<span data-ttu-id="b3fa2-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3fa2-193">String</span></span>|<span data-ttu-id="b3fa2-194">Texto personalizado a ser exibido na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-194">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="b3fa2-195">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="b3fa2-195">authorizedUsersListHidden</span></span>|<span data-ttu-id="b3fa2-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-196">Boolean</span></span>|<span data-ttu-id="b3fa2-197">Se deseja mostrar a caixa de diálogo nome e senha ou uma lista de usuários na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-197">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="b3fa2-198">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="b3fa2-198">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="b3fa2-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-199">Boolean</span></span>|<span data-ttu-id="b3fa2-200">Se deseja mostrar somente usuários de rede e de sistema na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-200">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="b3fa2-201">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="b3fa2-201">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="b3fa2-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-202">Boolean</span></span>|<span data-ttu-id="b3fa2-203">Se os usuários móveis serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-203">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="b3fa2-204">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="b3fa2-204">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="b3fa2-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-205">Boolean</span></span>|<span data-ttu-id="b3fa2-206">Se os usuários da rede serão mostrados na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-206">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="b3fa2-207">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="b3fa2-207">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="b3fa2-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-208">Boolean</span></span>|<span data-ttu-id="b3fa2-209">Se os usuários de administrador serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-209">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="b3fa2-210">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="b3fa2-210">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="b3fa2-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-211">Boolean</span></span>|<span data-ttu-id="b3fa2-212">Se deseja mostrar outros usuários na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-212">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="b3fa2-213">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="b3fa2-213">shutDownDisabled</span></span>|<span data-ttu-id="b3fa2-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-214">Boolean</span></span>|<span data-ttu-id="b3fa2-215">Se o item de botão desligar será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-215">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="b3fa2-216">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="b3fa2-216">restartDisabled</span></span>|<span data-ttu-id="b3fa2-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-217">Boolean</span></span>|<span data-ttu-id="b3fa2-218">Se o item de botão de reinicialização será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-218">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="b3fa2-219">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="b3fa2-219">sleepDisabled</span></span>|<span data-ttu-id="b3fa2-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-220">Boolean</span></span>|<span data-ttu-id="b3fa2-221">Se o item de menu de suspensão será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-221">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="b3fa2-222">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="b3fa2-222">consoleAccessDisabled</span></span>|<span data-ttu-id="b3fa2-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-223">Boolean</span></span>|<span data-ttu-id="b3fa2-224">Se o outro usuário desconsiderará o uso do>console> nome de usuário especial.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-224">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="b3fa2-225">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="b3fa2-225">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="b3fa2-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-226">Boolean</span></span>|<span data-ttu-id="b3fa2-227">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-227">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="b3fa2-228">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="b3fa2-228">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="b3fa2-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-229">Boolean</span></span>|<span data-ttu-id="b3fa2-230">Se o item de menu reiniciar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-230">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="b3fa2-231">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="b3fa2-231">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="b3fa2-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-232">Boolean</span></span>|<span data-ttu-id="b3fa2-233">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-233">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="b3fa2-234">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="b3fa2-234">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="b3fa2-235">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-235">Boolean</span></span>|<span data-ttu-id="b3fa2-236">Se o item de menu fazer logout na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-236">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="b3fa2-237">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="b3fa2-237">screenLockDisableImmediate</span></span>|<span data-ttu-id="b3fa2-238">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-238">Boolean</span></span>|<span data-ttu-id="b3fa2-239">Se as funções de bloqueio de tela imediata serão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-239">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="b3fa2-240">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="b3fa2-240">associatedDomains</span></span>|<span data-ttu-id="b3fa2-241">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b3fa2-242">Obtém ou define uma lista que mapeia aplicativos para seus domínios associados.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-242">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="b3fa2-243">A chave deve corresponder à ID do aplicativo, e o valor deve ser uma cadeia de caracteres no formato "Service: domain" onde domínio é um nome de host totalmente qualificado (por exemplo, webcredentials:example. com).</span><span class="sxs-lookup"><span data-stu-id="b3fa2-243">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="b3fa2-244">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-244">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b3fa2-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="b3fa2-245">singleSignOnExtension</span></span>|[<span data-ttu-id="b3fa2-246">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="b3fa2-246">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="b3fa2-247">Obtém ou define um perfil de extensão de logon único.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-247">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="b3fa2-248">Preterido: Use MacOSSingleSignOnExtension em vez disso.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-248">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="b3fa2-249">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="b3fa2-249">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="b3fa2-250">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="b3fa2-250">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="b3fa2-251">Obtém ou define um perfil de extensão de logon único.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-251">Gets or sets a single sign-on extension profile.</span></span>|
|<span data-ttu-id="b3fa2-252">contentCachingEnabled</span><span class="sxs-lookup"><span data-stu-id="b3fa2-252">contentCachingEnabled</span></span>|<span data-ttu-id="b3fa2-253">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-253">Boolean</span></span>|<span data-ttu-id="b3fa2-254">Habilita o cache de conteúdo e impede que ele seja desabilitado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-254">Enables content caching and prevents it from being disabled by the user.</span></span>|
|<span data-ttu-id="b3fa2-255">contentCachingType</span><span class="sxs-lookup"><span data-stu-id="b3fa2-255">contentCachingType</span></span>|[<span data-ttu-id="b3fa2-256">macOSContentCachingType</span><span class="sxs-lookup"><span data-stu-id="b3fa2-256">macOSContentCachingType</span></span>](../resources/intune-deviceconfig-macoscontentcachingtype.md)|<span data-ttu-id="b3fa2-257">Determina o tipo de conteúdo que pode ser armazenado em cache pelo serviço de cache de conteúdo da Apple.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-257">Determines what type of content is allowed to be cached by Apple's content caching service.</span></span> <span data-ttu-id="b3fa2-258">Os valores possíveis são: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-258">Possible values are: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span></span>|
|<span data-ttu-id="b3fa2-259">contentCachingMaxSizeBytes</span><span class="sxs-lookup"><span data-stu-id="b3fa2-259">contentCachingMaxSizeBytes</span></span>|<span data-ttu-id="b3fa2-260">Int32</span><span class="sxs-lookup"><span data-stu-id="b3fa2-260">Int32</span></span>|<span data-ttu-id="b3fa2-261">O número máximo de bytes de espaço em disco que serão usados para o cache de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-261">The maximum number of bytes of disk space that will be used for the content cache.</span></span> <span data-ttu-id="b3fa2-262">Um valor de 0 (padrão) indica espaço em disco ilimitado.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-262">A value of 0 (default) indicates unlimited disk space.</span></span> |
|<span data-ttu-id="b3fa2-263">contentCachingDataPath</span><span class="sxs-lookup"><span data-stu-id="b3fa2-263">contentCachingDataPath</span></span>|<span data-ttu-id="b3fa2-264">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3fa2-264">String</span></span>|<span data-ttu-id="b3fa2-265">O caminho para o diretório usado para armazenar o conteúdo em cache.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-265">The path to the directory used to store cached content.</span></span> <span data-ttu-id="b3fa2-266">O valor deve ser (ou terminar com)/Library/Application Support/Apple/AssetCache/data</span><span class="sxs-lookup"><span data-stu-id="b3fa2-266">The value must be (or end with) /Library/Application Support/Apple/AssetCache/Data</span></span>|
|<span data-ttu-id="b3fa2-267">contentCachingDisableConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="b3fa2-267">contentCachingDisableConnectionSharing</span></span>|<span data-ttu-id="b3fa2-268">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-268">Boolean</span></span>|<span data-ttu-id="b3fa2-269">Desabilita o compartilhamento de conexão com a Internet.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-269">Disables internet connection sharing.</span></span>|
|<span data-ttu-id="b3fa2-270">contentCachingForceConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="b3fa2-270">contentCachingForceConnectionSharing</span></span>|<span data-ttu-id="b3fa2-271">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-271">Boolean</span></span>|<span data-ttu-id="b3fa2-272">Força o compartilhamento de conexão com a Internet.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-272">Forces internet connection sharing.</span></span> <span data-ttu-id="b3fa2-273">contentCachingDisableConnectionSharing substitui essa configuração.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-273">contentCachingDisableConnectionSharing overrides this setting.</span></span>|
|<span data-ttu-id="b3fa2-274">contentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="b3fa2-274">contentCachingClientPolicy</span></span>|[<span data-ttu-id="b3fa2-275">macOSContentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="b3fa2-275">macOSContentCachingClientPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|<span data-ttu-id="b3fa2-276">Determina o método no qual os servidores de cache de conteúdo ouvirão clientes.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-276">Determines the method in which content caching servers will listen for clients.</span></span> <span data-ttu-id="b3fa2-277">Os valores possíveis são: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-277">Possible values are: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span></span>|
|<span data-ttu-id="b3fa2-278">contentCachingClientListenRanges</span><span class="sxs-lookup"><span data-stu-id="b3fa2-278">contentCachingClientListenRanges</span></span>|<span data-ttu-id="b3fa2-279">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-279">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="b3fa2-280">Uma lista de caches de conteúdo de intervalos de IP personalizados que será usada para escutar clientes.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-280">A list of custom IP ranges content caches will use to listen for clients.</span></span> <span data-ttu-id="b3fa2-281">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-281">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b3fa2-282">contentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="b3fa2-282">contentCachingPeerPolicy</span></span>|[<span data-ttu-id="b3fa2-283">macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="b3fa2-283">macOSContentCachingPeerPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|<span data-ttu-id="b3fa2-284">Determina o método no qual o conteúdo armazena em cache ponto com outros caches.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-284">Determines the method in which content caches peer with other caches.</span></span> <span data-ttu-id="b3fa2-285">Os valores possíveis são: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-285">Possible values are: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span></span>|
|<span data-ttu-id="b3fa2-286">contentCachingPeerListenRanges</span><span class="sxs-lookup"><span data-stu-id="b3fa2-286">contentCachingPeerListenRanges</span></span>|<span data-ttu-id="b3fa2-287">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-287">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="b3fa2-288">Uma lista de caches de conteúdo de intervalos de IP personalizados que será usada para escutar em caches de par.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-288">A list of custom IP ranges content caches will use to listen for peer caches.</span></span> <span data-ttu-id="b3fa2-289">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-289">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b3fa2-290">contentCachingPeerFilterRanges</span><span class="sxs-lookup"><span data-stu-id="b3fa2-290">contentCachingPeerFilterRanges</span></span>|<span data-ttu-id="b3fa2-291">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-291">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="b3fa2-292">Uma lista de caches de conteúdo de intervalos de IP personalizados que usará para consultar conteúdo de caches de mesmo nível.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-292">A list of custom IP ranges content caches will use to query for content from peers caches.</span></span> <span data-ttu-id="b3fa2-293">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-293">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b3fa2-294">contentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b3fa2-294">contentCachingParentSelectionPolicy</span></span>|[<span data-ttu-id="b3fa2-295">macOSContentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b3fa2-295">macOSContentCachingParentSelectionPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|<span data-ttu-id="b3fa2-296">Determina o método no qual os servidores de cache de conteúdo selecionarão pais, se houver vários.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-296">Determines the method in which content caching servers will select parents if multiple are present.</span></span> <span data-ttu-id="b3fa2-297">Os possíveis valores são: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-297">Possible values are: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span></span>|
|<span data-ttu-id="b3fa2-298">contentCachingParents</span><span class="sxs-lookup"><span data-stu-id="b3fa2-298">contentCachingParents</span></span>|<span data-ttu-id="b3fa2-299">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3fa2-299">String collection</span></span>|<span data-ttu-id="b3fa2-300">Uma lista de endereços IP que representam caches de conteúdo pai.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-300">A list of IP addresses representing parent content caches.</span></span>|
|<span data-ttu-id="b3fa2-301">contentCachingLogClientIdentities</span><span class="sxs-lookup"><span data-stu-id="b3fa2-301">contentCachingLogClientIdentities</span></span>|<span data-ttu-id="b3fa2-302">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-302">Boolean</span></span>|<span data-ttu-id="b3fa2-303">Permite o registro em log de endereços IP e portas de clientes que solicitam conteúdo em cache.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-303">Enables logging of IP addresses and ports of clients that request cached content.</span></span>|
|<span data-ttu-id="b3fa2-304">contentCachingPublicRanges</span><span class="sxs-lookup"><span data-stu-id="b3fa2-304">contentCachingPublicRanges</span></span>|<span data-ttu-id="b3fa2-305">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="b3fa2-305">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="b3fa2-306">Uma lista de intervalos de IP personalizados que o serviço de cache de conteúdo da Apple deve usar para fazer a correspondência de clientes com caches de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-306">A list of custom IP ranges that Apple's content caching service should use to match clients to content caches.</span></span> <span data-ttu-id="b3fa2-307">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-307">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b3fa2-308">contentCachingBlockDeletion</span><span class="sxs-lookup"><span data-stu-id="b3fa2-308">contentCachingBlockDeletion</span></span>|<span data-ttu-id="b3fa2-309">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-309">Boolean</span></span>|<span data-ttu-id="b3fa2-310">Impede que caches de conteúdo limpem conteúdo para liberar espaço em disco para outros aplicativos.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-310">Prevents content caches from purging content to free up disk space for other apps.</span></span>|
|<span data-ttu-id="b3fa2-311">contentCachingShowAlerts</span><span class="sxs-lookup"><span data-stu-id="b3fa2-311">contentCachingShowAlerts</span></span>|<span data-ttu-id="b3fa2-312">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-312">Boolean</span></span>|<span data-ttu-id="b3fa2-313">Exibir alertas de cache de conteúdo como notificações do sistema.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-313">Display content caching alerts as system notifications.</span></span>|
|<span data-ttu-id="b3fa2-314">contentCachingKeepAwake</span><span class="sxs-lookup"><span data-stu-id="b3fa2-314">contentCachingKeepAwake</span></span>|<span data-ttu-id="b3fa2-315">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3fa2-315">Boolean</span></span>|<span data-ttu-id="b3fa2-316">Impedir que o dispositivo fique dormindo se o cache de conteúdo estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-316">Prevent the device from sleeping if content caching is enabled.</span></span>|
|<span data-ttu-id="b3fa2-317">contentCachingPort</span><span class="sxs-lookup"><span data-stu-id="b3fa2-317">contentCachingPort</span></span>|<span data-ttu-id="b3fa2-318">Int32</span><span class="sxs-lookup"><span data-stu-id="b3fa2-318">Int32</span></span>|<span data-ttu-id="b3fa2-319">Define a porta usada para o cache de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-319">Sets the port used for content caching.</span></span> <span data-ttu-id="b3fa2-320">Se o valor for 0, uma porta aleatória disponível será selecionada.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-320">If the value is 0, a random available port will be selected.</span></span> <span data-ttu-id="b3fa2-321">Valores válidos de 0 a 65535</span><span class="sxs-lookup"><span data-stu-id="b3fa2-321">Valid values 0 to 65535</span></span>|



## <a name="response"></a><span data-ttu-id="b3fa2-322">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3fa2-322">Response</span></span>
<span data-ttu-id="b3fa2-323">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-323">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3fa2-324">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3fa2-324">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3fa2-325">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3fa2-325">Request</span></span>
<span data-ttu-id="b3fa2-326">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-326">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 5388

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

### <a name="response"></a><span data-ttu-id="b3fa2-327">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3fa2-327">Response</span></span>
<span data-ttu-id="b3fa2-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3fa2-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5560

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






