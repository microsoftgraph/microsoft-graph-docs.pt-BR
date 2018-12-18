---
title: Criar windows10TeamGeneralConfiguration
description: Criar um novo objeto windows10TeamGeneralConfiguration.
author: tfitzmac
ms.openlocfilehash: aa796f7896ce2cd30f93978daf60744710a2caf1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311050"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="b0c65-103">Criar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0c65-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="b0c65-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b0c65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0c65-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b0c65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0c65-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b0c65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0c65-107">Criar um novo objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b0c65-107">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0c65-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0c65-108">Prerequisites</span></span>
<span data-ttu-id="b0c65-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0c65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0c65-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0c65-111">Permission type</span></span>|<span data-ttu-id="b0c65-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0c65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0c65-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0c65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0c65-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0c65-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0c65-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0c65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0c65-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0c65-116">Not supported.</span></span>|
|<span data-ttu-id="b0c65-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0c65-117">Application</span></span>|<span data-ttu-id="b0c65-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0c65-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0c65-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0c65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b0c65-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0c65-120">Request headers</span></span>
|<span data-ttu-id="b0c65-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0c65-121">Header</span></span>|<span data-ttu-id="b0c65-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b0c65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0c65-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0c65-123">Authorization</span></span>|<span data-ttu-id="b0c65-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0c65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0c65-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0c65-125">Accept</span></span>|<span data-ttu-id="b0c65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0c65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0c65-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0c65-127">Request body</span></span>
<span data-ttu-id="b0c65-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b0c65-128">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="b0c65-129">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b0c65-129">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="b0c65-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0c65-130">Property</span></span>|<span data-ttu-id="b0c65-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0c65-131">Type</span></span>|<span data-ttu-id="b0c65-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0c65-133">id</span><span class="sxs-lookup"><span data-stu-id="b0c65-133">id</span></span>|<span data-ttu-id="b0c65-134">String</span><span class="sxs-lookup"><span data-stu-id="b0c65-134">String</span></span>|<span data-ttu-id="b0c65-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b0c65-135">Key of the entity.</span></span> <span data-ttu-id="b0c65-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0c65-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0c65-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0c65-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b0c65-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0c65-138">DateTimeOffset</span></span>|<span data-ttu-id="b0c65-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b0c65-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b0c65-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0c65-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0c65-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b0c65-141">roleScopeTagIds</span></span>|<span data-ttu-id="b0c65-142">String collection</span><span class="sxs-lookup"><span data-stu-id="b0c65-142">String collection</span></span>|<span data-ttu-id="b0c65-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="b0c65-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b0c65-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0c65-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0c65-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b0c65-145">supportsScopeTags</span></span>|<span data-ttu-id="b0c65-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0c65-146">Boolean</span></span>|<span data-ttu-id="b0c65-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="b0c65-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b0c65-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="b0c65-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b0c65-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="b0c65-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b0c65-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0c65-150">This property is read-only.</span></span> <span data-ttu-id="b0c65-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0c65-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0c65-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0c65-152">createdDateTime</span></span>|<span data-ttu-id="b0c65-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0c65-153">DateTimeOffset</span></span>|<span data-ttu-id="b0c65-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b0c65-154">DateTime the object was created.</span></span> <span data-ttu-id="b0c65-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0c65-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0c65-156">description</span><span class="sxs-lookup"><span data-stu-id="b0c65-156">description</span></span>|<span data-ttu-id="b0c65-157">String</span><span class="sxs-lookup"><span data-stu-id="b0c65-157">String</span></span>|<span data-ttu-id="b0c65-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0c65-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b0c65-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0c65-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0c65-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b0c65-160">displayName</span></span>|<span data-ttu-id="b0c65-161">String</span><span class="sxs-lookup"><span data-stu-id="b0c65-161">String</span></span>|<span data-ttu-id="b0c65-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0c65-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b0c65-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0c65-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0c65-164">version</span><span class="sxs-lookup"><span data-stu-id="b0c65-164">version</span></span>|<span data-ttu-id="b0c65-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b0c65-165">Int32</span></span>|<span data-ttu-id="b0c65-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0c65-166">Version of the device configuration.</span></span> <span data-ttu-id="b0c65-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0c65-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0c65-168">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="b0c65-168">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="b0c65-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0c65-169">Boolean</span></span>|<span data-ttu-id="b0c65-170">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="b0c65-170">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="b0c65-171">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="b0c65-171">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="b0c65-172">String</span><span class="sxs-lookup"><span data-stu-id="b0c65-172">String</span></span>|<span data-ttu-id="b0c65-173">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="b0c65-173">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="b0c65-174">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="b0c65-174">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="b0c65-175">String</span><span class="sxs-lookup"><span data-stu-id="b0c65-175">String</span></span>|<span data-ttu-id="b0c65-176">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="b0c65-176">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="b0c65-177">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="b0c65-177">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="b0c65-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0c65-178">Boolean</span></span>|<span data-ttu-id="b0c65-179">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="b0c65-179">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="b0c65-180">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="b0c65-180">maintenanceWindowBlocked</span></span>|<span data-ttu-id="b0c65-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0c65-181">Boolean</span></span>|<span data-ttu-id="b0c65-182">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b0c65-182">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="b0c65-183">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="b0c65-183">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="b0c65-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b0c65-184">Int32</span></span>|<span data-ttu-id="b0c65-185">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0c65-185">Maintenance window duration for device updates.</span></span> <span data-ttu-id="b0c65-186">Valores válidos: 0 a 5</span><span class="sxs-lookup"><span data-stu-id="b0c65-186">Valid values 0 to 5</span></span>|
|<span data-ttu-id="b0c65-187">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="b0c65-187">maintenanceWindowStartTime</span></span>|<span data-ttu-id="b0c65-188">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b0c65-188">TimeOfDay</span></span>|<span data-ttu-id="b0c65-189">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0c65-189">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="b0c65-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="b0c65-190">miracastChannel</span></span>|[<span data-ttu-id="b0c65-191">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="b0c65-191">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="b0c65-192">O canal.</span><span class="sxs-lookup"><span data-stu-id="b0c65-192">The channel.</span></span> <span data-ttu-id="b0c65-193">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="b0c65-193">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="b0c65-194">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="b0c65-194">miracastBlocked</span></span>|<span data-ttu-id="b0c65-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0c65-195">Boolean</span></span>|<span data-ttu-id="b0c65-196">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="b0c65-196">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="b0c65-197">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="b0c65-197">miracastRequirePin</span></span>|<span data-ttu-id="b0c65-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0c65-198">Boolean</span></span>|<span data-ttu-id="b0c65-199">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="b0c65-199">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="b0c65-200">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="b0c65-200">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="b0c65-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0c65-201">Boolean</span></span>|<span data-ttu-id="b0c65-202">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="b0c65-202">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="b0c65-203">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="b0c65-203">settingsBlockSessionResume</span></span>|<span data-ttu-id="b0c65-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0c65-204">Boolean</span></span>|<span data-ttu-id="b0c65-205">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="b0c65-205">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="b0c65-206">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="b0c65-206">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="b0c65-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0c65-207">Boolean</span></span>|<span data-ttu-id="b0c65-208">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="b0c65-208">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="b0c65-209">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="b0c65-209">settingsDefaultVolume</span></span>|<span data-ttu-id="b0c65-210">Int32</span><span class="sxs-lookup"><span data-stu-id="b0c65-210">Int32</span></span>|<span data-ttu-id="b0c65-211">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="b0c65-211">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="b0c65-212">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="b0c65-212">Permitted values are 0-100.</span></span> <span data-ttu-id="b0c65-213">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="b0c65-213">The default is 45.</span></span> <span data-ttu-id="b0c65-214">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="b0c65-214">Valid values 0 to 100</span></span>|
|<span data-ttu-id="b0c65-215">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b0c65-215">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="b0c65-216">Int32</span><span class="sxs-lookup"><span data-stu-id="b0c65-216">Int32</span></span>|<span data-ttu-id="b0c65-217">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="b0c65-217">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="b0c65-218">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b0c65-218">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="b0c65-219">Int32</span><span class="sxs-lookup"><span data-stu-id="b0c65-219">Int32</span></span>|<span data-ttu-id="b0c65-220">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="b0c65-220">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="b0c65-221">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b0c65-221">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="b0c65-222">Int32</span><span class="sxs-lookup"><span data-stu-id="b0c65-222">Int32</span></span>|<span data-ttu-id="b0c65-223">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="b0c65-223">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="b0c65-224">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="b0c65-224">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="b0c65-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0c65-225">Boolean</span></span>|<span data-ttu-id="b0c65-226">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="b0c65-226">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="b0c65-227">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="b0c65-227">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="b0c65-228">String</span><span class="sxs-lookup"><span data-stu-id="b0c65-228">String</span></span>|<span data-ttu-id="b0c65-229">The welcome screen background image URL.</span><span class="sxs-lookup"><span data-stu-id="b0c65-229">The welcome screen background image URL.</span></span> <span data-ttu-id="b0c65-230">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="b0c65-230">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="b0c65-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="b0c65-231">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="b0c65-232">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="b0c65-232">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="b0c65-233">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="b0c65-233">The welcome screen meeting information shown.</span></span> <span data-ttu-id="b0c65-234">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="b0c65-234">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="b0c65-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0c65-235">Response</span></span>
<span data-ttu-id="b0c65-236">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0c65-236">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0c65-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0c65-237">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0c65-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0c65-238">Request</span></span>
<span data-ttu-id="b0c65-239">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0c65-239">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0c65-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0c65-240">Response</span></span>
<span data-ttu-id="b0c65-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0c65-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





