---
title: Criar macOSDeviceFeaturesConfiguration
description: Criar um novo objeto macOSDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e6c56d3a2c5291deb298f6f7d4082e571a5b114f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37178750"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="f5042-103">Criar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="f5042-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="f5042-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f5042-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5042-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5042-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5042-106">Criar um novo objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f5042-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5042-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f5042-107">Prerequisites</span></span>
<span data-ttu-id="f5042-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5042-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5042-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5042-110">Permission type</span></span>|<span data-ttu-id="f5042-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f5042-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5042-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5042-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5042-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5042-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5042-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5042-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5042-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5042-115">Not supported.</span></span>|
|<span data-ttu-id="f5042-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5042-116">Application</span></span>|<span data-ttu-id="f5042-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5042-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5042-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5042-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f5042-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5042-119">Request headers</span></span>
|<span data-ttu-id="f5042-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5042-120">Header</span></span>|<span data-ttu-id="f5042-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f5042-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5042-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5042-122">Authorization</span></span>|<span data-ttu-id="f5042-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5042-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5042-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f5042-124">Accept</span></span>|<span data-ttu-id="f5042-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f5042-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5042-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5042-126">Request body</span></span>
<span data-ttu-id="f5042-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f5042-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="f5042-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f5042-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="f5042-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5042-129">Property</span></span>|<span data-ttu-id="f5042-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5042-130">Type</span></span>|<span data-ttu-id="f5042-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5042-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5042-132">id</span><span class="sxs-lookup"><span data-stu-id="f5042-132">id</span></span>|<span data-ttu-id="f5042-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5042-133">String</span></span>|<span data-ttu-id="f5042-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f5042-134">Key of the entity.</span></span> <span data-ttu-id="f5042-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5042-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5042-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f5042-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5042-137">DateTimeOffset</span></span>|<span data-ttu-id="f5042-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f5042-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f5042-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5042-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f5042-140">roleScopeTagIds</span></span>|<span data-ttu-id="f5042-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5042-141">String collection</span></span>|<span data-ttu-id="f5042-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="f5042-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f5042-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5042-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f5042-144">supportsScopeTags</span></span>|<span data-ttu-id="f5042-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-145">Boolean</span></span>|<span data-ttu-id="f5042-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f5042-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f5042-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f5042-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f5042-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="f5042-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f5042-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f5042-149">This property is read-only.</span></span> <span data-ttu-id="f5042-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5042-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f5042-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f5042-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f5042-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f5042-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="f5042-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f5042-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5042-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f5042-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f5042-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f5042-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f5042-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="f5042-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f5042-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5042-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f5042-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f5042-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f5042-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f5042-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="f5042-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f5042-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5042-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5042-163">createdDateTime</span></span>|<span data-ttu-id="f5042-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5042-164">DateTimeOffset</span></span>|<span data-ttu-id="f5042-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f5042-165">DateTime the object was created.</span></span> <span data-ttu-id="f5042-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5042-167">descrição</span><span class="sxs-lookup"><span data-stu-id="f5042-167">description</span></span>|<span data-ttu-id="f5042-168">String</span><span class="sxs-lookup"><span data-stu-id="f5042-168">String</span></span>|<span data-ttu-id="f5042-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f5042-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f5042-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5042-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f5042-171">displayName</span></span>|<span data-ttu-id="f5042-172">String</span><span class="sxs-lookup"><span data-stu-id="f5042-172">String</span></span>|<span data-ttu-id="f5042-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f5042-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f5042-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5042-175">versão</span><span class="sxs-lookup"><span data-stu-id="f5042-175">version</span></span>|<span data-ttu-id="f5042-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f5042-176">Int32</span></span>|<span data-ttu-id="f5042-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f5042-177">Version of the device configuration.</span></span> <span data-ttu-id="f5042-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5042-179">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="f5042-179">airPrintDestinations</span></span>|<span data-ttu-id="f5042-180">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="f5042-181">Uma matriz de impressoras de impressão que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="f5042-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="f5042-182">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f5042-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="f5042-183">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="f5042-184">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="f5042-184">autoLaunchItems</span></span>|<span data-ttu-id="f5042-185">coleção [macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="f5042-186">Lista de aplicativos, arquivos, pastas e outros itens a serem iniciados quando o usuário fizer logon.</span><span class="sxs-lookup"><span data-stu-id="f5042-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="f5042-187">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f5042-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f5042-188">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="f5042-188">adminShowHostInfo</span></span>|<span data-ttu-id="f5042-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-189">Boolean</span></span>|<span data-ttu-id="f5042-190">Se deseja mostrar as informações de host de administrador na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="f5042-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="f5042-191">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="f5042-191">loginWindowText</span></span>|<span data-ttu-id="f5042-192">String</span><span class="sxs-lookup"><span data-stu-id="f5042-192">String</span></span>|<span data-ttu-id="f5042-193">Texto personalizado a ser exibido na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="f5042-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="f5042-194">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="f5042-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="f5042-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-195">Boolean</span></span>|<span data-ttu-id="f5042-196">Se deseja mostrar a caixa de diálogo nome e senha ou uma lista de usuários na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="f5042-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="f5042-197">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="f5042-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="f5042-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-198">Boolean</span></span>|<span data-ttu-id="f5042-199">Se deseja mostrar somente usuários de rede e de sistema na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="f5042-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="f5042-200">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="f5042-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="f5042-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-201">Boolean</span></span>|<span data-ttu-id="f5042-202">Se os usuários móveis serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="f5042-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="f5042-203">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="f5042-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="f5042-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-204">Boolean</span></span>|<span data-ttu-id="f5042-205">Se os usuários da rede serão mostrados na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="f5042-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="f5042-206">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="f5042-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="f5042-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-207">Boolean</span></span>|<span data-ttu-id="f5042-208">Se os usuários de administrador serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="f5042-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="f5042-209">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="f5042-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="f5042-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-210">Boolean</span></span>|<span data-ttu-id="f5042-211">Se deseja mostrar outros usuários na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="f5042-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="f5042-212">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="f5042-212">shutDownDisabled</span></span>|<span data-ttu-id="f5042-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-213">Boolean</span></span>|<span data-ttu-id="f5042-214">Se o item de botão desligar será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="f5042-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="f5042-215">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="f5042-215">restartDisabled</span></span>|<span data-ttu-id="f5042-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-216">Boolean</span></span>|<span data-ttu-id="f5042-217">Se o item de botão de reinicialização será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="f5042-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="f5042-218">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="f5042-218">sleepDisabled</span></span>|<span data-ttu-id="f5042-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-219">Boolean</span></span>|<span data-ttu-id="f5042-220">Se o item de menu de suspensão será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="f5042-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="f5042-221">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="f5042-221">consoleAccessDisabled</span></span>|<span data-ttu-id="f5042-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-222">Boolean</span></span>|<span data-ttu-id="f5042-223">Se o outro usuário desconsiderará o uso do>console> nome de usuário especial.</span><span class="sxs-lookup"><span data-stu-id="f5042-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="f5042-224">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="f5042-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="f5042-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-225">Boolean</span></span>|<span data-ttu-id="f5042-226">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="f5042-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="f5042-227">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="f5042-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="f5042-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-228">Boolean</span></span>|<span data-ttu-id="f5042-229">Se o item de menu reiniciar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="f5042-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="f5042-230">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="f5042-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="f5042-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-231">Boolean</span></span>|<span data-ttu-id="f5042-232">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="f5042-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="f5042-233">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="f5042-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="f5042-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-234">Boolean</span></span>|<span data-ttu-id="f5042-235">Se o item de menu fazer logout na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="f5042-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="f5042-236">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="f5042-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="f5042-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5042-237">Boolean</span></span>|<span data-ttu-id="f5042-238">Se as funções de bloqueio de tela imediata serão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="f5042-238">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="f5042-239">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="f5042-239">associatedDomains</span></span>|<span data-ttu-id="f5042-240">Coleção [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f5042-240">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="f5042-241">Obtém ou define uma lista que mapeia aplicativos para seus domínios associados.</span><span class="sxs-lookup"><span data-stu-id="f5042-241">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="f5042-242">A chave deve corresponder à ID do aplicativo, e o valor deve ser uma cadeia de caracteres no formato "Service: domain" onde domínio é um nome de host totalmente qualificado (por exemplo, webcredentials:example. com).</span><span class="sxs-lookup"><span data-stu-id="f5042-242">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="f5042-243">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="f5042-243">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f5042-244">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="f5042-244">singleSignOnExtension</span></span>|[<span data-ttu-id="f5042-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="f5042-245">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="f5042-246">Obtém ou define um perfil de extensão de logon único.</span><span class="sxs-lookup"><span data-stu-id="f5042-246">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="f5042-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5042-247">Response</span></span>
<span data-ttu-id="f5042-248">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5042-248">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5042-249">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5042-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5042-250">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5042-250">Request</span></span>
<span data-ttu-id="f5042-251">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5042-251">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2362

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
  }
}
```

### <a name="response"></a><span data-ttu-id="f5042-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5042-252">Response</span></span>
<span data-ttu-id="f5042-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5042-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2534

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
  }
}
```




