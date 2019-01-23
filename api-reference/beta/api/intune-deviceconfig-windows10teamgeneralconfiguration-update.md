---
title: Atualizar windows10TeamGeneralConfiguration
description: Atualizar as propriedades de um objeto windows10TeamGeneralConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8d2faf01d6184201ebe444712d6b16c4b03cc35b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408849"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="15525-103">Atualizar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="15525-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="15525-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="15525-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15525-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="15525-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15525-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="15525-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15525-107">Atualizar as propriedades de um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15525-107">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15525-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="15525-108">Prerequisites</span></span>
<span data-ttu-id="15525-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="15525-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="15525-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15525-111">Permission type</span></span>|<span data-ttu-id="15525-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="15525-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15525-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15525-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15525-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15525-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="15525-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15525-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15525-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15525-116">Not supported.</span></span>|
|<span data-ttu-id="15525-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15525-117">Application</span></span>|<span data-ttu-id="15525-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15525-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15525-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15525-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="15525-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15525-120">Request headers</span></span>
|<span data-ttu-id="15525-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="15525-121">Header</span></span>|<span data-ttu-id="15525-122">Valor</span><span class="sxs-lookup"><span data-stu-id="15525-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15525-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="15525-123">Authorization</span></span>|<span data-ttu-id="15525-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15525-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15525-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="15525-125">Accept</span></span>|<span data-ttu-id="15525-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15525-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15525-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15525-127">Request body</span></span>
<span data-ttu-id="15525-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15525-128">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="15525-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="15525-129">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="15525-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15525-130">Property</span></span>|<span data-ttu-id="15525-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="15525-131">Type</span></span>|<span data-ttu-id="15525-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="15525-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15525-133">id</span><span class="sxs-lookup"><span data-stu-id="15525-133">id</span></span>|<span data-ttu-id="15525-134">String</span><span class="sxs-lookup"><span data-stu-id="15525-134">String</span></span>|<span data-ttu-id="15525-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="15525-135">Key of the entity.</span></span> <span data-ttu-id="15525-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15525-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15525-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15525-137">lastModifiedDateTime</span></span>|<span data-ttu-id="15525-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15525-138">DateTimeOffset</span></span>|<span data-ttu-id="15525-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="15525-139">DateTime the object was last modified.</span></span> <span data-ttu-id="15525-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15525-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15525-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="15525-141">roleScopeTagIds</span></span>|<span data-ttu-id="15525-142">String collection</span><span class="sxs-lookup"><span data-stu-id="15525-142">String collection</span></span>|<span data-ttu-id="15525-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="15525-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="15525-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15525-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15525-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="15525-145">supportsScopeTags</span></span>|<span data-ttu-id="15525-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="15525-146">Boolean</span></span>|<span data-ttu-id="15525-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="15525-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="15525-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="15525-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="15525-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="15525-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="15525-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="15525-150">This property is read-only.</span></span> <span data-ttu-id="15525-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15525-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15525-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15525-152">createdDateTime</span></span>|<span data-ttu-id="15525-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15525-153">DateTimeOffset</span></span>|<span data-ttu-id="15525-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="15525-154">DateTime the object was created.</span></span> <span data-ttu-id="15525-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15525-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15525-156">description</span><span class="sxs-lookup"><span data-stu-id="15525-156">description</span></span>|<span data-ttu-id="15525-157">String</span><span class="sxs-lookup"><span data-stu-id="15525-157">String</span></span>|<span data-ttu-id="15525-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15525-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="15525-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15525-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15525-160">displayName</span><span class="sxs-lookup"><span data-stu-id="15525-160">displayName</span></span>|<span data-ttu-id="15525-161">String</span><span class="sxs-lookup"><span data-stu-id="15525-161">String</span></span>|<span data-ttu-id="15525-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15525-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="15525-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15525-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15525-164">version</span><span class="sxs-lookup"><span data-stu-id="15525-164">version</span></span>|<span data-ttu-id="15525-165">Int32</span><span class="sxs-lookup"><span data-stu-id="15525-165">Int32</span></span>|<span data-ttu-id="15525-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15525-166">Version of the device configuration.</span></span> <span data-ttu-id="15525-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="15525-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="15525-168">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="15525-168">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="15525-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="15525-169">Boolean</span></span>|<span data-ttu-id="15525-170">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="15525-170">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="15525-171">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="15525-171">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="15525-172">String</span><span class="sxs-lookup"><span data-stu-id="15525-172">String</span></span>|<span data-ttu-id="15525-173">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="15525-173">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="15525-174">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="15525-174">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="15525-175">String</span><span class="sxs-lookup"><span data-stu-id="15525-175">String</span></span>|<span data-ttu-id="15525-176">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="15525-176">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="15525-177">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="15525-177">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="15525-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="15525-178">Boolean</span></span>|<span data-ttu-id="15525-179">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="15525-179">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="15525-180">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="15525-180">maintenanceWindowBlocked</span></span>|<span data-ttu-id="15525-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="15525-181">Boolean</span></span>|<span data-ttu-id="15525-182">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="15525-182">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="15525-183">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="15525-183">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="15525-184">Int32</span><span class="sxs-lookup"><span data-stu-id="15525-184">Int32</span></span>|<span data-ttu-id="15525-185">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15525-185">Maintenance window duration for device updates.</span></span> <span data-ttu-id="15525-186">Valores válidos: 0 a 5</span><span class="sxs-lookup"><span data-stu-id="15525-186">Valid values 0 to 5</span></span>|
|<span data-ttu-id="15525-187">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="15525-187">maintenanceWindowStartTime</span></span>|<span data-ttu-id="15525-188">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="15525-188">TimeOfDay</span></span>|<span data-ttu-id="15525-189">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15525-189">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="15525-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="15525-190">miracastChannel</span></span>|[<span data-ttu-id="15525-191">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="15525-191">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="15525-192">O canal.</span><span class="sxs-lookup"><span data-stu-id="15525-192">The channel.</span></span> <span data-ttu-id="15525-193">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="15525-193">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="15525-194">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="15525-194">miracastBlocked</span></span>|<span data-ttu-id="15525-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="15525-195">Boolean</span></span>|<span data-ttu-id="15525-196">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="15525-196">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="15525-197">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="15525-197">miracastRequirePin</span></span>|<span data-ttu-id="15525-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="15525-198">Boolean</span></span>|<span data-ttu-id="15525-199">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="15525-199">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="15525-200">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="15525-200">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="15525-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="15525-201">Boolean</span></span>|<span data-ttu-id="15525-202">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="15525-202">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="15525-203">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="15525-203">settingsBlockSessionResume</span></span>|<span data-ttu-id="15525-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="15525-204">Boolean</span></span>|<span data-ttu-id="15525-205">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="15525-205">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="15525-206">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="15525-206">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="15525-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="15525-207">Boolean</span></span>|<span data-ttu-id="15525-208">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="15525-208">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="15525-209">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="15525-209">settingsDefaultVolume</span></span>|<span data-ttu-id="15525-210">Int32</span><span class="sxs-lookup"><span data-stu-id="15525-210">Int32</span></span>|<span data-ttu-id="15525-211">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="15525-211">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="15525-212">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="15525-212">Permitted values are 0-100.</span></span> <span data-ttu-id="15525-213">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="15525-213">The default is 45.</span></span> <span data-ttu-id="15525-214">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="15525-214">Valid values 0 to 100</span></span>|
|<span data-ttu-id="15525-215">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="15525-215">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="15525-216">Int32</span><span class="sxs-lookup"><span data-stu-id="15525-216">Int32</span></span>|<span data-ttu-id="15525-217">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="15525-217">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="15525-218">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="15525-218">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="15525-219">Int32</span><span class="sxs-lookup"><span data-stu-id="15525-219">Int32</span></span>|<span data-ttu-id="15525-220">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="15525-220">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="15525-221">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="15525-221">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="15525-222">Int32</span><span class="sxs-lookup"><span data-stu-id="15525-222">Int32</span></span>|<span data-ttu-id="15525-223">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="15525-223">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="15525-224">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="15525-224">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="15525-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="15525-225">Boolean</span></span>|<span data-ttu-id="15525-226">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="15525-226">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="15525-227">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="15525-227">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="15525-228">String</span><span class="sxs-lookup"><span data-stu-id="15525-228">String</span></span>|<span data-ttu-id="15525-229">The welcome screen background image URL.</span><span class="sxs-lookup"><span data-stu-id="15525-229">The welcome screen background image URL.</span></span> <span data-ttu-id="15525-230">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="15525-230">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="15525-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="15525-231">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="15525-232">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="15525-232">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="15525-233">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="15525-233">The welcome screen meeting information shown.</span></span> <span data-ttu-id="15525-234">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="15525-234">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="15525-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="15525-235">Response</span></span>
<span data-ttu-id="15525-236">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15525-236">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15525-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15525-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="15525-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15525-238">Request</span></span>
<span data-ttu-id="15525-239">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15525-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1242

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```

### <a name="response"></a><span data-ttu-id="15525-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="15525-240">Response</span></span>
<span data-ttu-id="15525-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15525-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1414

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```




