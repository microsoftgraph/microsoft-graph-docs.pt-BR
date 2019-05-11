---
title: Atualizar macOSDeviceFeaturesConfiguration
description: Atualizar as propriedades de um objeto macOSDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64588b45886d8abfbc6f7598d626c3bb47dfcdc9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922821"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="4dfe4-103">Atualizar macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="4dfe4-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="4dfe4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dfe4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dfe4-106">Atualizar as propriedades de um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dfe4-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4dfe4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4dfe4-107">Prerequisites</span></span>
<span data-ttu-id="4dfe4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4dfe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dfe4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4dfe4-110">Permission type</span></span>|<span data-ttu-id="4dfe4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4dfe4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4dfe4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4dfe4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4dfe4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4dfe4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-115">Not supported.</span></span>|
|<span data-ttu-id="4dfe4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4dfe4-116">Application</span></span>|<span data-ttu-id="4dfe4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4dfe4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4dfe4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4dfe4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4dfe4-119">Request headers</span></span>
|<span data-ttu-id="4dfe4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4dfe4-120">Header</span></span>|<span data-ttu-id="4dfe4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4dfe4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4dfe4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4dfe4-122">Authorization</span></span>|<span data-ttu-id="4dfe4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4dfe4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4dfe4-124">Accept</span></span>|<span data-ttu-id="4dfe4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4dfe4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dfe4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4dfe4-126">Request body</span></span>
<span data-ttu-id="4dfe4-127">No corpo da solicitação, forneça uma representação JSON do objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dfe4-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="4dfe4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4dfe4-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="4dfe4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dfe4-129">Property</span></span>|<span data-ttu-id="4dfe4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dfe4-130">Type</span></span>|<span data-ttu-id="4dfe4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dfe4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dfe4-132">id</span><span class="sxs-lookup"><span data-stu-id="4dfe4-132">id</span></span>|<span data-ttu-id="4dfe4-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4dfe4-133">String</span></span>|<span data-ttu-id="4dfe4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-134">Key of the entity.</span></span> <span data-ttu-id="4dfe4-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dfe4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4dfe4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4dfe4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dfe4-137">DateTimeOffset</span></span>|<span data-ttu-id="4dfe4-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4dfe4-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dfe4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4dfe4-140">roleScopeTagIds</span></span>|<span data-ttu-id="4dfe4-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4dfe4-141">String collection</span></span>|<span data-ttu-id="4dfe4-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4dfe4-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dfe4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4dfe4-144">supportsScopeTags</span></span>|<span data-ttu-id="4dfe4-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-145">Boolean</span></span>|<span data-ttu-id="4dfe4-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4dfe4-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4dfe4-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4dfe4-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-149">This property is read-only.</span></span> <span data-ttu-id="4dfe4-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dfe4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4dfe4-151">createdDateTime</span></span>|<span data-ttu-id="4dfe4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dfe4-152">DateTimeOffset</span></span>|<span data-ttu-id="4dfe4-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-153">DateTime the object was created.</span></span> <span data-ttu-id="4dfe4-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dfe4-155">description</span><span class="sxs-lookup"><span data-stu-id="4dfe4-155">description</span></span>|<span data-ttu-id="4dfe4-156">String</span><span class="sxs-lookup"><span data-stu-id="4dfe4-156">String</span></span>|<span data-ttu-id="4dfe4-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4dfe4-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dfe4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4dfe4-159">displayName</span></span>|<span data-ttu-id="4dfe4-160">String</span><span class="sxs-lookup"><span data-stu-id="4dfe4-160">String</span></span>|<span data-ttu-id="4dfe4-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4dfe4-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dfe4-163">versão</span><span class="sxs-lookup"><span data-stu-id="4dfe4-163">version</span></span>|<span data-ttu-id="4dfe4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4dfe4-164">Int32</span></span>|<span data-ttu-id="4dfe4-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-165">Version of the device configuration.</span></span> <span data-ttu-id="4dfe4-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4dfe4-167">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="4dfe4-167">airPrintDestinations</span></span>|<span data-ttu-id="4dfe4-168">coleção [airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="4dfe4-169">Uma matriz de impressoras de impressão que sempre devem ser mostradas.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="4dfe4-170">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="4dfe4-171">Herdado de [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="4dfe4-172">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="4dfe4-172">autoLaunchItems</span></span>|<span data-ttu-id="4dfe4-173">coleção [macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="4dfe4-173">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="4dfe4-174">Lista de aplicativos, arquivos, pastas e outros itens a serem iniciados quando o usuário fizer logon.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-174">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="4dfe4-175">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-175">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4dfe4-176">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="4dfe4-176">adminShowHostInfo</span></span>|<span data-ttu-id="4dfe4-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-177">Boolean</span></span>|<span data-ttu-id="4dfe4-178">Se deseja mostrar as informações de host de administrador na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-178">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="4dfe4-179">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="4dfe4-179">loginWindowText</span></span>|<span data-ttu-id="4dfe4-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4dfe4-180">String</span></span>|<span data-ttu-id="4dfe4-181">Texto personalizado a ser exibido na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-181">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="4dfe4-182">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="4dfe4-182">authorizedUsersListHidden</span></span>|<span data-ttu-id="4dfe4-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-183">Boolean</span></span>|<span data-ttu-id="4dfe4-184">Se deseja mostrar a caixa de diálogo nome e senha ou uma lista de usuários na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-184">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="4dfe4-185">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="4dfe4-185">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="4dfe4-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-186">Boolean</span></span>|<span data-ttu-id="4dfe4-187">Se deseja mostrar somente usuários de rede e de sistema na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-187">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="4dfe4-188">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="4dfe4-188">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="4dfe4-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-189">Boolean</span></span>|<span data-ttu-id="4dfe4-190">Se os usuários móveis serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-190">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="4dfe4-191">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="4dfe4-191">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="4dfe4-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-192">Boolean</span></span>|<span data-ttu-id="4dfe4-193">Se os usuários da rede serão mostrados na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-193">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="4dfe4-194">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="4dfe4-194">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="4dfe4-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-195">Boolean</span></span>|<span data-ttu-id="4dfe4-196">Se os usuários de administrador serão ocultos na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-196">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="4dfe4-197">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="4dfe4-197">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="4dfe4-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-198">Boolean</span></span>|<span data-ttu-id="4dfe4-199">Se deseja mostrar outros usuários na lista de usuários autorizados na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-199">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="4dfe4-200">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="4dfe4-200">shutDownDisabled</span></span>|<span data-ttu-id="4dfe4-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-201">Boolean</span></span>|<span data-ttu-id="4dfe4-202">Se o item de botão desligar será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-202">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="4dfe4-203">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="4dfe4-203">restartDisabled</span></span>|<span data-ttu-id="4dfe4-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-204">Boolean</span></span>|<span data-ttu-id="4dfe4-205">Se o item de botão de reinicialização será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-205">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="4dfe4-206">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="4dfe4-206">sleepDisabled</span></span>|<span data-ttu-id="4dfe4-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-207">Boolean</span></span>|<span data-ttu-id="4dfe4-208">Se o item de menu de suspensão será ocultado na janela de logon.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-208">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="4dfe4-209">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="4dfe4-209">consoleAccessDisabled</span></span>|<span data-ttu-id="4dfe4-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-210">Boolean</span></span>|<span data-ttu-id="4dfe4-211">Se o outro usuário desconsiderará o uso do nome de usuário especial do >console>.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-211">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="4dfe4-212">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="4dfe4-212">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="4dfe4-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-213">Boolean</span></span>|<span data-ttu-id="4dfe4-214">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-214">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="4dfe4-215">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="4dfe4-215">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="4dfe4-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-216">Boolean</span></span>|<span data-ttu-id="4dfe4-217">Se o item de menu reiniciar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-217">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="4dfe4-218">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="4dfe4-218">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="4dfe4-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-219">Boolean</span></span>|<span data-ttu-id="4dfe4-220">Se o item de menu desligar na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-220">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="4dfe4-221">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="4dfe4-221">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="4dfe4-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-222">Boolean</span></span>|<span data-ttu-id="4dfe4-223">Se o item de menu fazer logout na janela de logon será desabilitado enquanto o usuário estiver conectado.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-223">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="4dfe4-224">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="4dfe4-224">screenLockDisableImmediate</span></span>|<span data-ttu-id="4dfe4-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dfe4-225">Boolean</span></span>|<span data-ttu-id="4dfe4-226">Se as funções de bloqueio de tela imediata serão desabilitadas.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-226">Whether to disable the immediate screen lock functions.</span></span>|



## <a name="response"></a><span data-ttu-id="4dfe4-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dfe4-227">Response</span></span>
<span data-ttu-id="4dfe4-228">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-228">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dfe4-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4dfe4-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="4dfe4-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4dfe4-230">Request</span></span>
<span data-ttu-id="4dfe4-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1334

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="4dfe4-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="4dfe4-232">Response</span></span>
<span data-ttu-id="4dfe4-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4dfe4-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1506

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




