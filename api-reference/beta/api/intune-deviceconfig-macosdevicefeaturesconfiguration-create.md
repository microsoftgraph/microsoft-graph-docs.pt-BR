---
title: Criar macOSDeviceFeaturesConfiguration
description: Criar um novo objeto macOSDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 08a2cb517420c2540e272239c05a1991303d17af
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976873"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="18301-103">Criar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="18301-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="18301-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18301-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18301-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18301-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18301-106">Criar um novo objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="18301-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18301-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="18301-107">Prerequisites</span></span>
<span data-ttu-id="18301-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18301-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18301-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18301-110">Permission type</span></span>|<span data-ttu-id="18301-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="18301-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18301-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18301-112">Delegated (work or school account)</span></span>|<span data-ttu-id="18301-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18301-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="18301-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18301-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18301-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18301-115">Not supported.</span></span>|
|<span data-ttu-id="18301-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18301-116">Application</span></span>|<span data-ttu-id="18301-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18301-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18301-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18301-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="18301-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18301-119">Request headers</span></span>
|<span data-ttu-id="18301-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="18301-120">Header</span></span>|<span data-ttu-id="18301-121">Valor</span><span class="sxs-lookup"><span data-stu-id="18301-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18301-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="18301-122">Authorization</span></span>|<span data-ttu-id="18301-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18301-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18301-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="18301-124">Accept</span></span>|<span data-ttu-id="18301-125">application/json</span><span class="sxs-lookup"><span data-stu-id="18301-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18301-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18301-126">Request body</span></span>
<span data-ttu-id="18301-127">No corpo da solicitação, forneça uma representação JSON do objeto macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="18301-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="18301-128">A tabela a seguir mostra as propriedades que são necessárias ao criar macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="18301-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="18301-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18301-129">Property</span></span>|<span data-ttu-id="18301-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="18301-130">Type</span></span>|<span data-ttu-id="18301-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="18301-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18301-132">id</span><span class="sxs-lookup"><span data-stu-id="18301-132">id</span></span>|<span data-ttu-id="18301-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18301-133">String</span></span>|<span data-ttu-id="18301-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="18301-134">Key of the entity.</span></span> <span data-ttu-id="18301-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18301-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18301-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18301-136">lastModifiedDateTime</span></span>|<span data-ttu-id="18301-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18301-137">DateTimeOffset</span></span>|<span data-ttu-id="18301-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="18301-138">DateTime the object was last modified.</span></span> <span data-ttu-id="18301-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18301-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18301-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18301-140">roleScopeTagIds</span></span>|<span data-ttu-id="18301-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="18301-141">String collection</span></span>|<span data-ttu-id="18301-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="18301-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="18301-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18301-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18301-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="18301-144">supportsScopeTags</span></span>|<span data-ttu-id="18301-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-145">Boolean</span></span>|<span data-ttu-id="18301-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="18301-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="18301-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="18301-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="18301-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="18301-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="18301-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="18301-149">This property is read-only.</span></span> <span data-ttu-id="18301-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18301-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18301-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="18301-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="18301-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="18301-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="18301-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="18301-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="18301-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18301-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18301-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="18301-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="18301-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="18301-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="18301-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="18301-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="18301-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18301-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18301-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="18301-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="18301-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="18301-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="18301-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="18301-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="18301-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18301-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18301-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18301-163">createdDateTime</span></span>|<span data-ttu-id="18301-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18301-164">DateTimeOffset</span></span>|<span data-ttu-id="18301-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="18301-165">DateTime the object was created.</span></span> <span data-ttu-id="18301-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18301-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18301-167">descrição</span><span class="sxs-lookup"><span data-stu-id="18301-167">description</span></span>|<span data-ttu-id="18301-168">String</span><span class="sxs-lookup"><span data-stu-id="18301-168">String</span></span>|<span data-ttu-id="18301-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18301-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="18301-170">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18301-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18301-171">displayName</span><span class="sxs-lookup"><span data-stu-id="18301-171">displayName</span></span>|<span data-ttu-id="18301-172">String</span><span class="sxs-lookup"><span data-stu-id="18301-172">String</span></span>|<span data-ttu-id="18301-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18301-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="18301-174">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18301-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18301-175">versão</span><span class="sxs-lookup"><span data-stu-id="18301-175">version</span></span>|<span data-ttu-id="18301-176">Int32</span><span class="sxs-lookup"><span data-stu-id="18301-176">Int32</span></span>|<span data-ttu-id="18301-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18301-177">Version of the device configuration.</span></span> <span data-ttu-id="18301-178">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="18301-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="18301-179">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="18301-179">airPrintDestinations</span></span>|<span data-ttu-id="18301-180">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="18301-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="18301-181">Uma matriz de impressoras de impressão que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="18301-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="18301-182">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="18301-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="18301-183">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="18301-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="18301-184">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="18301-184">autoLaunchItems</span></span>|<span data-ttu-id="18301-185">coleção [macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="18301-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="18301-186">Lista de aplicativos, arquivos, pastas e outros itens a serem iniciados quando o usuário fizer logon.</span><span class="sxs-lookup"><span data-stu-id="18301-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="18301-187">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="18301-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="18301-188">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="18301-188">adminShowHostInfo</span></span>|<span data-ttu-id="18301-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-189">Boolean</span></span>|<span data-ttu-id="18301-190">Se deseja mostrar as informações de host de administrador na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="18301-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="18301-191">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="18301-191">loginWindowText</span></span>|<span data-ttu-id="18301-192">String</span><span class="sxs-lookup"><span data-stu-id="18301-192">String</span></span>|<span data-ttu-id="18301-193">Texto personalizado a ser exibido na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="18301-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="18301-194">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="18301-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="18301-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-195">Boolean</span></span>|<span data-ttu-id="18301-196">Se deseja mostrar a caixa de diálogo nome e senha ou uma lista de usuários na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="18301-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="18301-197">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="18301-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="18301-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-198">Boolean</span></span>|<span data-ttu-id="18301-199">Se deseja mostrar somente usuários de rede e de sistema na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="18301-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="18301-200">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="18301-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="18301-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-201">Boolean</span></span>|<span data-ttu-id="18301-202">Se os usuários móveis serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="18301-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="18301-203">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="18301-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="18301-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-204">Boolean</span></span>|<span data-ttu-id="18301-205">Se os usuários da rede serão mostrados na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="18301-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="18301-206">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="18301-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="18301-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-207">Boolean</span></span>|<span data-ttu-id="18301-208">Se os usuários de administrador serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="18301-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="18301-209">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="18301-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="18301-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-210">Boolean</span></span>|<span data-ttu-id="18301-211">Se deseja mostrar outros usuários na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="18301-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="18301-212">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="18301-212">shutDownDisabled</span></span>|<span data-ttu-id="18301-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-213">Boolean</span></span>|<span data-ttu-id="18301-214">Se o item de botão desligar será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="18301-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="18301-215">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="18301-215">restartDisabled</span></span>|<span data-ttu-id="18301-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-216">Boolean</span></span>|<span data-ttu-id="18301-217">Se o item de botão de reinicialização será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="18301-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="18301-218">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="18301-218">sleepDisabled</span></span>|<span data-ttu-id="18301-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-219">Boolean</span></span>|<span data-ttu-id="18301-220">Se o item de menu de suspensão será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="18301-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="18301-221">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="18301-221">consoleAccessDisabled</span></span>|<span data-ttu-id="18301-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-222">Boolean</span></span>|<span data-ttu-id="18301-223">Se o outro usuário desconsiderará o uso do>console> nome de usuário especial.</span><span class="sxs-lookup"><span data-stu-id="18301-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="18301-224">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="18301-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="18301-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-225">Boolean</span></span>|<span data-ttu-id="18301-226">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="18301-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="18301-227">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="18301-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="18301-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-228">Boolean</span></span>|<span data-ttu-id="18301-229">Se o item de menu reiniciar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="18301-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="18301-230">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="18301-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="18301-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-231">Boolean</span></span>|<span data-ttu-id="18301-232">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="18301-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="18301-233">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="18301-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="18301-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-234">Boolean</span></span>|<span data-ttu-id="18301-235">Se o item de menu fazer logout na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="18301-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="18301-236">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="18301-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="18301-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="18301-237">Boolean</span></span>|<span data-ttu-id="18301-238">Se as funções de bloqueio de tela imediata serão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="18301-238">Whether to disable the immediate screen lock functions.</span></span>|



## <a name="response"></a><span data-ttu-id="18301-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="18301-239">Response</span></span>
<span data-ttu-id="18301-240">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18301-240">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18301-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18301-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="18301-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18301-242">Request</span></span>
<span data-ttu-id="18301-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="18301-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="18301-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="18301-244">Response</span></span>
<span data-ttu-id="18301-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18301-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





