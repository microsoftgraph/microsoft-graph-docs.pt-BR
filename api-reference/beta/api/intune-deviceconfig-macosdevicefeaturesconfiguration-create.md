---
title: Criar macOSDeviceFeaturesConfiguration
description: Criar um novo objeto macOSDeviceFeaturesConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 509487d54dfa2d7f5041214bd79ca1d144a8bc28
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42747022"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="7420e-103">Criar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="7420e-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="7420e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7420e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7420e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7420e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7420e-106">Criar um novo objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7420e-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7420e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7420e-107">Prerequisites</span></span>
<span data-ttu-id="7420e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7420e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7420e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7420e-110">Permission type</span></span>|<span data-ttu-id="7420e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7420e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7420e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7420e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7420e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7420e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7420e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7420e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7420e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7420e-115">Not supported.</span></span>|
|<span data-ttu-id="7420e-116">Application</span><span class="sxs-lookup"><span data-stu-id="7420e-116">Application</span></span>|<span data-ttu-id="7420e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7420e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7420e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7420e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7420e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7420e-119">Request headers</span></span>
|<span data-ttu-id="7420e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7420e-120">Header</span></span>|<span data-ttu-id="7420e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7420e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7420e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7420e-122">Authorization</span></span>|<span data-ttu-id="7420e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7420e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7420e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7420e-124">Accept</span></span>|<span data-ttu-id="7420e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7420e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7420e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7420e-126">Request body</span></span>
<span data-ttu-id="7420e-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7420e-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="7420e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="7420e-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="7420e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7420e-129">Property</span></span>|<span data-ttu-id="7420e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7420e-130">Type</span></span>|<span data-ttu-id="7420e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7420e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7420e-132">id</span><span class="sxs-lookup"><span data-stu-id="7420e-132">id</span></span>|<span data-ttu-id="7420e-133">String</span><span class="sxs-lookup"><span data-stu-id="7420e-133">String</span></span>|<span data-ttu-id="7420e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7420e-134">Key of the entity.</span></span> <span data-ttu-id="7420e-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7420e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7420e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7420e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7420e-137">DateTimeOffset</span></span>|<span data-ttu-id="7420e-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7420e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7420e-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7420e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7420e-140">roleScopeTagIds</span></span>|<span data-ttu-id="7420e-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7420e-141">String collection</span></span>|<span data-ttu-id="7420e-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="7420e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7420e-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7420e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7420e-144">supportsScopeTags</span></span>|<span data-ttu-id="7420e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-145">Boolean</span></span>|<span data-ttu-id="7420e-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="7420e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7420e-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="7420e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7420e-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7420e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7420e-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7420e-149">This property is read-only.</span></span> <span data-ttu-id="7420e-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7420e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7420e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7420e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7420e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7420e-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="7420e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7420e-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7420e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7420e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7420e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7420e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7420e-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="7420e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7420e-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7420e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7420e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7420e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7420e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7420e-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="7420e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7420e-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7420e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7420e-163">createdDateTime</span></span>|<span data-ttu-id="7420e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7420e-164">DateTimeOffset</span></span>|<span data-ttu-id="7420e-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7420e-165">DateTime the object was created.</span></span> <span data-ttu-id="7420e-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7420e-167">description</span><span class="sxs-lookup"><span data-stu-id="7420e-167">description</span></span>|<span data-ttu-id="7420e-168">String</span><span class="sxs-lookup"><span data-stu-id="7420e-168">String</span></span>|<span data-ttu-id="7420e-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7420e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7420e-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7420e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="7420e-171">displayName</span></span>|<span data-ttu-id="7420e-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7420e-172">String</span></span>|<span data-ttu-id="7420e-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7420e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7420e-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7420e-175">versão</span><span class="sxs-lookup"><span data-stu-id="7420e-175">version</span></span>|<span data-ttu-id="7420e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7420e-176">Int32</span></span>|<span data-ttu-id="7420e-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7420e-177">Version of the device configuration.</span></span> <span data-ttu-id="7420e-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7420e-179">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="7420e-179">airPrintDestinations</span></span>|<span data-ttu-id="7420e-180">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="7420e-181">Uma matriz de impressoras de impressão que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="7420e-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="7420e-182">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="7420e-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="7420e-183">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="7420e-184">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="7420e-184">autoLaunchItems</span></span>|<span data-ttu-id="7420e-185">coleção [macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="7420e-186">Lista de aplicativos, arquivos, pastas e outros itens a serem iniciados quando o usuário fizer logon.</span><span class="sxs-lookup"><span data-stu-id="7420e-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="7420e-187">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="7420e-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7420e-188">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="7420e-188">adminShowHostInfo</span></span>|<span data-ttu-id="7420e-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-189">Boolean</span></span>|<span data-ttu-id="7420e-190">Se deseja mostrar as informações de host de administrador na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="7420e-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="7420e-191">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="7420e-191">loginWindowText</span></span>|<span data-ttu-id="7420e-192">String</span><span class="sxs-lookup"><span data-stu-id="7420e-192">String</span></span>|<span data-ttu-id="7420e-193">Texto personalizado a ser exibido na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="7420e-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="7420e-194">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="7420e-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="7420e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-195">Boolean</span></span>|<span data-ttu-id="7420e-196">Se deseja mostrar a caixa de diálogo nome e senha ou uma lista de usuários na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="7420e-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="7420e-197">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="7420e-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="7420e-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-198">Boolean</span></span>|<span data-ttu-id="7420e-199">Se deseja mostrar somente usuários de rede e de sistema na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="7420e-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="7420e-200">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="7420e-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="7420e-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-201">Boolean</span></span>|<span data-ttu-id="7420e-202">Se os usuários móveis serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="7420e-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="7420e-203">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="7420e-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="7420e-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-204">Boolean</span></span>|<span data-ttu-id="7420e-205">Se os usuários da rede serão mostrados na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="7420e-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="7420e-206">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="7420e-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="7420e-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-207">Boolean</span></span>|<span data-ttu-id="7420e-208">Se os usuários de administrador serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="7420e-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="7420e-209">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="7420e-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="7420e-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-210">Boolean</span></span>|<span data-ttu-id="7420e-211">Se deseja mostrar outros usuários na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="7420e-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="7420e-212">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="7420e-212">shutDownDisabled</span></span>|<span data-ttu-id="7420e-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-213">Boolean</span></span>|<span data-ttu-id="7420e-214">Se o item de botão desligar será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="7420e-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="7420e-215">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="7420e-215">restartDisabled</span></span>|<span data-ttu-id="7420e-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-216">Boolean</span></span>|<span data-ttu-id="7420e-217">Se o item de botão de reinicialização será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="7420e-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="7420e-218">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="7420e-218">sleepDisabled</span></span>|<span data-ttu-id="7420e-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-219">Boolean</span></span>|<span data-ttu-id="7420e-220">Se o item de menu de suspensão será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="7420e-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="7420e-221">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="7420e-221">consoleAccessDisabled</span></span>|<span data-ttu-id="7420e-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-222">Boolean</span></span>|<span data-ttu-id="7420e-223">Se o outro usuário desconsiderará o uso do>console> nome de usuário especial.</span><span class="sxs-lookup"><span data-stu-id="7420e-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="7420e-224">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="7420e-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="7420e-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-225">Boolean</span></span>|<span data-ttu-id="7420e-226">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="7420e-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="7420e-227">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="7420e-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="7420e-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-228">Boolean</span></span>|<span data-ttu-id="7420e-229">Se o item de menu reiniciar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="7420e-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="7420e-230">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="7420e-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="7420e-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-231">Boolean</span></span>|<span data-ttu-id="7420e-232">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="7420e-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="7420e-233">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="7420e-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="7420e-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-234">Boolean</span></span>|<span data-ttu-id="7420e-235">Se o item de menu fazer logout na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="7420e-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="7420e-236">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="7420e-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="7420e-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="7420e-237">Boolean</span></span>|<span data-ttu-id="7420e-238">Se as funções de bloqueio de tela imediata serão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="7420e-238">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="7420e-239">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="7420e-239">associatedDomains</span></span>|<span data-ttu-id="7420e-240">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="7420e-240">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="7420e-241">Obtém ou define uma lista que mapeia aplicativos para seus domínios associados.</span><span class="sxs-lookup"><span data-stu-id="7420e-241">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="7420e-242">A chave deve corresponder à ID do aplicativo, e o valor deve ser uma cadeia de caracteres no formato "Service: domain" onde domínio é um nome de host totalmente qualificado (por exemplo, webcredentials:example. com).</span><span class="sxs-lookup"><span data-stu-id="7420e-242">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="7420e-243">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="7420e-243">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7420e-244">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="7420e-244">singleSignOnExtension</span></span>|[<span data-ttu-id="7420e-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="7420e-245">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="7420e-246">Obtém ou define um perfil de extensão de logon único.</span><span class="sxs-lookup"><span data-stu-id="7420e-246">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="7420e-247">Preterido: Use MacOSSingleSignOnExtension em vez disso.</span><span class="sxs-lookup"><span data-stu-id="7420e-247">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="7420e-248">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="7420e-248">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="7420e-249">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="7420e-249">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="7420e-250">Obtém ou define um perfil de extensão de logon único.</span><span class="sxs-lookup"><span data-stu-id="7420e-250">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="7420e-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="7420e-251">Response</span></span>
<span data-ttu-id="7420e-252">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7420e-252">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7420e-253">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7420e-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="7420e-254">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7420e-254">Request</span></span>
<span data-ttu-id="7420e-255">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7420e-255">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2468

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
    "@odata.type": "microsoft.graph.singleSignOnExtension"
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSSingleSignOnExtension"
  }
}
```

### <a name="response"></a><span data-ttu-id="7420e-256">Resposta</span><span class="sxs-lookup"><span data-stu-id="7420e-256">Response</span></span>
<span data-ttu-id="7420e-p117">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7420e-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2640

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
    "@odata.type": "microsoft.graph.singleSignOnExtension"
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSSingleSignOnExtension"
  }
}
```




