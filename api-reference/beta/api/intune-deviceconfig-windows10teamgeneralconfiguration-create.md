---
title: Criar windows10TeamGeneralConfiguration
description: Criar um novo objeto windows10TeamGeneralConfiguration.
ms.openlocfilehash: 14c188164244bc092f800053749adb1194125ac4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040380"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="e52f6-103">Criar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="e52f6-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="e52f6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e52f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e52f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e52f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e52f6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e52f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e52f6-107">Criar um novo objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e52f6-107">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e52f6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e52f6-108">Prerequisites</span></span>
<span data-ttu-id="e52f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e52f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e52f6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e52f6-111">Permission type</span></span>|<span data-ttu-id="e52f6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e52f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e52f6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e52f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e52f6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e52f6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e52f6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e52f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e52f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e52f6-116">Not supported.</span></span>|
|<span data-ttu-id="e52f6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e52f6-117">Application</span></span>|<span data-ttu-id="e52f6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e52f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e52f6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e52f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e52f6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e52f6-120">Request headers</span></span>
|<span data-ttu-id="e52f6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e52f6-121">Header</span></span>|<span data-ttu-id="e52f6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e52f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e52f6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e52f6-123">Authorization</span></span>|<span data-ttu-id="e52f6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e52f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e52f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e52f6-125">Accept</span></span>|<span data-ttu-id="e52f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e52f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e52f6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e52f6-127">Request body</span></span>
<span data-ttu-id="e52f6-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e52f6-128">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="e52f6-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e52f6-129">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="e52f6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e52f6-130">Property</span></span>|<span data-ttu-id="e52f6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e52f6-131">Type</span></span>|<span data-ttu-id="e52f6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e52f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e52f6-133">id</span><span class="sxs-lookup"><span data-stu-id="e52f6-133">id</span></span>|<span data-ttu-id="e52f6-134">String</span><span class="sxs-lookup"><span data-stu-id="e52f6-134">String</span></span>|<span data-ttu-id="e52f6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e52f6-135">Key of the entity.</span></span> <span data-ttu-id="e52f6-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e52f6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e52f6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e52f6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e52f6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e52f6-138">DateTimeOffset</span></span>|<span data-ttu-id="e52f6-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e52f6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e52f6-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e52f6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e52f6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e52f6-141">roleScopeTagIds</span></span>|<span data-ttu-id="e52f6-142">String collection</span><span class="sxs-lookup"><span data-stu-id="e52f6-142">String collection</span></span>|<span data-ttu-id="e52f6-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="e52f6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e52f6-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e52f6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e52f6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e52f6-145">supportsScopeTags</span></span>|<span data-ttu-id="e52f6-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="e52f6-146">Boolean</span></span>|<span data-ttu-id="e52f6-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e52f6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e52f6-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e52f6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e52f6-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="e52f6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e52f6-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e52f6-150">This property is read-only.</span></span> <span data-ttu-id="e52f6-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e52f6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e52f6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e52f6-152">createdDateTime</span></span>|<span data-ttu-id="e52f6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e52f6-153">DateTimeOffset</span></span>|<span data-ttu-id="e52f6-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e52f6-154">DateTime the object was created.</span></span> <span data-ttu-id="e52f6-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e52f6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e52f6-156">description</span><span class="sxs-lookup"><span data-stu-id="e52f6-156">description</span></span>|<span data-ttu-id="e52f6-157">String</span><span class="sxs-lookup"><span data-stu-id="e52f6-157">String</span></span>|<span data-ttu-id="e52f6-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e52f6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e52f6-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e52f6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e52f6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e52f6-160">displayName</span></span>|<span data-ttu-id="e52f6-161">String</span><span class="sxs-lookup"><span data-stu-id="e52f6-161">String</span></span>|<span data-ttu-id="e52f6-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e52f6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e52f6-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e52f6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e52f6-164">version</span><span class="sxs-lookup"><span data-stu-id="e52f6-164">version</span></span>|<span data-ttu-id="e52f6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e52f6-165">Int32</span></span>|<span data-ttu-id="e52f6-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e52f6-166">Version of the device configuration.</span></span> <span data-ttu-id="e52f6-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e52f6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e52f6-168">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="e52f6-168">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="e52f6-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="e52f6-169">Boolean</span></span>|<span data-ttu-id="e52f6-170">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="e52f6-170">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="e52f6-171">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="e52f6-171">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="e52f6-172">String</span><span class="sxs-lookup"><span data-stu-id="e52f6-172">String</span></span>|<span data-ttu-id="e52f6-173">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="e52f6-173">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="e52f6-174">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="e52f6-174">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="e52f6-175">String</span><span class="sxs-lookup"><span data-stu-id="e52f6-175">String</span></span>|<span data-ttu-id="e52f6-176">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="e52f6-176">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="e52f6-177">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="e52f6-177">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="e52f6-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="e52f6-178">Boolean</span></span>|<span data-ttu-id="e52f6-179">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="e52f6-179">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="e52f6-180">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="e52f6-180">maintenanceWindowBlocked</span></span>|<span data-ttu-id="e52f6-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="e52f6-181">Boolean</span></span>|<span data-ttu-id="e52f6-182">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="e52f6-182">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="e52f6-183">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="e52f6-183">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="e52f6-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e52f6-184">Int32</span></span>|<span data-ttu-id="e52f6-185">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e52f6-185">Maintenance window duration for device updates.</span></span> <span data-ttu-id="e52f6-186">Valores válidos: 0 a 5</span><span class="sxs-lookup"><span data-stu-id="e52f6-186">Valid values 0 to 5</span></span>|
|<span data-ttu-id="e52f6-187">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="e52f6-187">maintenanceWindowStartTime</span></span>|<span data-ttu-id="e52f6-188">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e52f6-188">TimeOfDay</span></span>|<span data-ttu-id="e52f6-189">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e52f6-189">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="e52f6-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="e52f6-190">miracastChannel</span></span>|[<span data-ttu-id="e52f6-191">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="e52f6-191">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="e52f6-192">O canal.</span><span class="sxs-lookup"><span data-stu-id="e52f6-192">The channel.</span></span> <span data-ttu-id="e52f6-193">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="e52f6-193">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="e52f6-194">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="e52f6-194">miracastBlocked</span></span>|<span data-ttu-id="e52f6-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="e52f6-195">Boolean</span></span>|<span data-ttu-id="e52f6-196">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="e52f6-196">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="e52f6-197">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="e52f6-197">miracastRequirePin</span></span>|<span data-ttu-id="e52f6-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="e52f6-198">Boolean</span></span>|<span data-ttu-id="e52f6-199">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="e52f6-199">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="e52f6-200">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="e52f6-200">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="e52f6-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="e52f6-201">Boolean</span></span>|<span data-ttu-id="e52f6-202">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="e52f6-202">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="e52f6-203">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="e52f6-203">settingsBlockSessionResume</span></span>|<span data-ttu-id="e52f6-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="e52f6-204">Boolean</span></span>|<span data-ttu-id="e52f6-205">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="e52f6-205">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="e52f6-206">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="e52f6-206">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="e52f6-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="e52f6-207">Boolean</span></span>|<span data-ttu-id="e52f6-208">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="e52f6-208">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="e52f6-209">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="e52f6-209">settingsDefaultVolume</span></span>|<span data-ttu-id="e52f6-210">Int32</span><span class="sxs-lookup"><span data-stu-id="e52f6-210">Int32</span></span>|<span data-ttu-id="e52f6-211">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="e52f6-211">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="e52f6-212">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="e52f6-212">Permitted values are 0-100.</span></span> <span data-ttu-id="e52f6-213">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="e52f6-213">The default is 45.</span></span> <span data-ttu-id="e52f6-214">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="e52f6-214">Valid values 0 to 100</span></span>|
|<span data-ttu-id="e52f6-215">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="e52f6-215">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="e52f6-216">Int32</span><span class="sxs-lookup"><span data-stu-id="e52f6-216">Int32</span></span>|<span data-ttu-id="e52f6-217">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="e52f6-217">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="e52f6-218">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="e52f6-218">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="e52f6-219">Int32</span><span class="sxs-lookup"><span data-stu-id="e52f6-219">Int32</span></span>|<span data-ttu-id="e52f6-220">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="e52f6-220">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="e52f6-221">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="e52f6-221">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="e52f6-222">Int32</span><span class="sxs-lookup"><span data-stu-id="e52f6-222">Int32</span></span>|<span data-ttu-id="e52f6-223">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="e52f6-223">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="e52f6-224">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="e52f6-224">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="e52f6-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="e52f6-225">Boolean</span></span>|<span data-ttu-id="e52f6-226">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="e52f6-226">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="e52f6-227">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="e52f6-227">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="e52f6-228">String</span><span class="sxs-lookup"><span data-stu-id="e52f6-228">String</span></span>|<span data-ttu-id="e52f6-229">The welcome screen background image URL.</span><span class="sxs-lookup"><span data-stu-id="e52f6-229">The welcome screen background image URL.</span></span> <span data-ttu-id="e52f6-230">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="e52f6-230">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="e52f6-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="e52f6-231">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="e52f6-232">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="e52f6-232">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="e52f6-233">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="e52f6-233">The welcome screen meeting information shown.</span></span> <span data-ttu-id="e52f6-234">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="e52f6-234">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="e52f6-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="e52f6-235">Response</span></span>
<span data-ttu-id="e52f6-236">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e52f6-236">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e52f6-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e52f6-237">Example</span></span>
### <a name="request"></a><span data-ttu-id="e52f6-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e52f6-238">Request</span></span>
<span data-ttu-id="e52f6-239">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e52f6-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1306

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="e52f6-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="e52f6-240">Response</span></span>
<span data-ttu-id="e52f6-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e52f6-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





