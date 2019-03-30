---
title: Atualizar windows10TeamGeneralConfiguration
description: Atualizar as propriedades de um objeto windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea49d65b395b8f3804f0cd9b42c33852832caa5f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988711"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="6d04a-103">Atualizar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="6d04a-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="6d04a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6d04a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d04a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6d04a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d04a-106">Atualizar as propriedades de um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d04a-106">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d04a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6d04a-107">Prerequisites</span></span>
<span data-ttu-id="6d04a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d04a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d04a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d04a-110">Permission type</span></span>|<span data-ttu-id="6d04a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6d04a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d04a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d04a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d04a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d04a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d04a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d04a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d04a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d04a-115">Not supported.</span></span>|
|<span data-ttu-id="6d04a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d04a-116">Application</span></span>|<span data-ttu-id="6d04a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d04a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d04a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d04a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6d04a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d04a-119">Request headers</span></span>
|<span data-ttu-id="6d04a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6d04a-120">Header</span></span>|<span data-ttu-id="6d04a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6d04a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d04a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d04a-122">Authorization</span></span>|<span data-ttu-id="6d04a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d04a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d04a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6d04a-124">Accept</span></span>|<span data-ttu-id="6d04a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6d04a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d04a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d04a-126">Request body</span></span>
<span data-ttu-id="6d04a-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d04a-127">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="6d04a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d04a-128">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="6d04a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d04a-129">Property</span></span>|<span data-ttu-id="6d04a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d04a-130">Type</span></span>|<span data-ttu-id="6d04a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d04a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d04a-132">id</span><span class="sxs-lookup"><span data-stu-id="6d04a-132">id</span></span>|<span data-ttu-id="6d04a-133">String</span><span class="sxs-lookup"><span data-stu-id="6d04a-133">String</span></span>|<span data-ttu-id="6d04a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6d04a-134">Key of the entity.</span></span> <span data-ttu-id="6d04a-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d04a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d04a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d04a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6d04a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d04a-137">DateTimeOffset</span></span>|<span data-ttu-id="6d04a-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6d04a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6d04a-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d04a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d04a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6d04a-140">roleScopeTagIds</span></span>|<span data-ttu-id="6d04a-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="6d04a-141">String collection</span></span>|<span data-ttu-id="6d04a-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6d04a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6d04a-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d04a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d04a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6d04a-144">supportsScopeTags</span></span>|<span data-ttu-id="6d04a-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d04a-145">Boolean</span></span>|<span data-ttu-id="6d04a-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6d04a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6d04a-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6d04a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6d04a-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6d04a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6d04a-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d04a-149">This property is read-only.</span></span> <span data-ttu-id="6d04a-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d04a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d04a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d04a-151">createdDateTime</span></span>|<span data-ttu-id="6d04a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d04a-152">DateTimeOffset</span></span>|<span data-ttu-id="6d04a-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6d04a-153">DateTime the object was created.</span></span> <span data-ttu-id="6d04a-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d04a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d04a-155">description</span><span class="sxs-lookup"><span data-stu-id="6d04a-155">description</span></span>|<span data-ttu-id="6d04a-156">String</span><span class="sxs-lookup"><span data-stu-id="6d04a-156">String</span></span>|<span data-ttu-id="6d04a-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d04a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6d04a-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d04a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d04a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6d04a-159">displayName</span></span>|<span data-ttu-id="6d04a-160">String</span><span class="sxs-lookup"><span data-stu-id="6d04a-160">String</span></span>|<span data-ttu-id="6d04a-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d04a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6d04a-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d04a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d04a-163">versão</span><span class="sxs-lookup"><span data-stu-id="6d04a-163">version</span></span>|<span data-ttu-id="6d04a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6d04a-164">Int32</span></span>|<span data-ttu-id="6d04a-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d04a-165">Version of the device configuration.</span></span> <span data-ttu-id="6d04a-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d04a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d04a-167">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="6d04a-167">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="6d04a-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d04a-168">Boolean</span></span>|<span data-ttu-id="6d04a-169">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="6d04a-169">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="6d04a-170">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="6d04a-170">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="6d04a-171">String</span><span class="sxs-lookup"><span data-stu-id="6d04a-171">String</span></span>|<span data-ttu-id="6d04a-172">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="6d04a-172">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="6d04a-173">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="6d04a-173">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="6d04a-174">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d04a-174">String</span></span>|<span data-ttu-id="6d04a-175">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="6d04a-175">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="6d04a-176">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="6d04a-176">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="6d04a-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d04a-177">Boolean</span></span>|<span data-ttu-id="6d04a-178">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="6d04a-178">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="6d04a-179">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="6d04a-179">maintenanceWindowBlocked</span></span>|<span data-ttu-id="6d04a-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d04a-180">Boolean</span></span>|<span data-ttu-id="6d04a-181">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6d04a-181">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="6d04a-182">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="6d04a-182">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="6d04a-183">Int32</span><span class="sxs-lookup"><span data-stu-id="6d04a-183">Int32</span></span>|<span data-ttu-id="6d04a-184">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d04a-184">Maintenance window duration for device updates.</span></span> <span data-ttu-id="6d04a-185">Valores válidos: 0 a 5</span><span class="sxs-lookup"><span data-stu-id="6d04a-185">Valid values 0 to 5</span></span>|
|<span data-ttu-id="6d04a-186">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="6d04a-186">maintenanceWindowStartTime</span></span>|<span data-ttu-id="6d04a-187">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6d04a-187">TimeOfDay</span></span>|<span data-ttu-id="6d04a-188">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6d04a-188">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="6d04a-189">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="6d04a-189">miracastChannel</span></span>|[<span data-ttu-id="6d04a-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="6d04a-190">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="6d04a-191">O canal.</span><span class="sxs-lookup"><span data-stu-id="6d04a-191">The channel.</span></span> <span data-ttu-id="6d04a-192">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="6d04a-192">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="6d04a-193">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="6d04a-193">miracastBlocked</span></span>|<span data-ttu-id="6d04a-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d04a-194">Boolean</span></span>|<span data-ttu-id="6d04a-195">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6d04a-195">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="6d04a-196">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="6d04a-196">miracastRequirePin</span></span>|<span data-ttu-id="6d04a-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d04a-197">Boolean</span></span>|<span data-ttu-id="6d04a-198">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="6d04a-198">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="6d04a-199">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="6d04a-199">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="6d04a-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d04a-200">Boolean</span></span>|<span data-ttu-id="6d04a-201">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="6d04a-201">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="6d04a-202">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="6d04a-202">settingsBlockSessionResume</span></span>|<span data-ttu-id="6d04a-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="6d04a-203">Boolean</span></span>|<span data-ttu-id="6d04a-204">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="6d04a-204">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="6d04a-205">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="6d04a-205">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="6d04a-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d04a-206">Boolean</span></span>|<span data-ttu-id="6d04a-207">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="6d04a-207">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="6d04a-208">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="6d04a-208">settingsDefaultVolume</span></span>|<span data-ttu-id="6d04a-209">Int32</span><span class="sxs-lookup"><span data-stu-id="6d04a-209">Int32</span></span>|<span data-ttu-id="6d04a-210">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="6d04a-210">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="6d04a-211">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="6d04a-211">Permitted values are 0-100.</span></span> <span data-ttu-id="6d04a-212">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="6d04a-212">The default is 45.</span></span> <span data-ttu-id="6d04a-213">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="6d04a-213">Valid values 0 to 100</span></span>|
|<span data-ttu-id="6d04a-214">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6d04a-214">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="6d04a-215">Int32</span><span class="sxs-lookup"><span data-stu-id="6d04a-215">Int32</span></span>|<span data-ttu-id="6d04a-216">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="6d04a-216">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="6d04a-217">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6d04a-217">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="6d04a-218">Int32</span><span class="sxs-lookup"><span data-stu-id="6d04a-218">Int32</span></span>|<span data-ttu-id="6d04a-219">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="6d04a-219">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="6d04a-220">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6d04a-220">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="6d04a-221">Int32</span><span class="sxs-lookup"><span data-stu-id="6d04a-221">Int32</span></span>|<span data-ttu-id="6d04a-222">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="6d04a-222">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="6d04a-223">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="6d04a-223">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="6d04a-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d04a-224">Boolean</span></span>|<span data-ttu-id="6d04a-225">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="6d04a-225">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="6d04a-226">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="6d04a-226">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="6d04a-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d04a-227">String</span></span>|<span data-ttu-id="6d04a-228">The welcome screen background image URL.</span><span class="sxs-lookup"><span data-stu-id="6d04a-228">The welcome screen background image URL.</span></span> <span data-ttu-id="6d04a-229">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="6d04a-229">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="6d04a-230">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="6d04a-230">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="6d04a-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="6d04a-231">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="6d04a-232">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="6d04a-232">The welcome screen meeting information shown.</span></span> <span data-ttu-id="6d04a-233">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="6d04a-233">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="6d04a-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d04a-234">Response</span></span>
<span data-ttu-id="6d04a-235">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d04a-235">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d04a-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d04a-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d04a-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d04a-237">Request</span></span>
<span data-ttu-id="6d04a-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d04a-238">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6d04a-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d04a-239">Response</span></span>
<span data-ttu-id="6d04a-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d04a-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




