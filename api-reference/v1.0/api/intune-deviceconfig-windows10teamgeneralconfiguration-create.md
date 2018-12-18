---
title: Criar windows10TeamGeneralConfiguration
description: Criar um novo objeto windows10TeamGeneralConfiguration.
author: tfitzmac
ms.openlocfilehash: 1634de20684f751dbb540b2fa619cd9153d8b0f1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340289"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="6bc3e-103">Criar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bc3e-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="6bc3e-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bc3e-105">Criar um novo objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bc3e-105">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6bc3e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6bc3e-106">Prerequisites</span></span>
<span data-ttu-id="6bc3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bc3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bc3e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bc3e-109">Permission type</span></span>|<span data-ttu-id="6bc3e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6bc3e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bc3e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bc3e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6bc3e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bc3e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6bc3e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bc3e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bc3e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-114">Not supported.</span></span>|
|<span data-ttu-id="6bc3e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bc3e-115">Application</span></span>|<span data-ttu-id="6bc3e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bc3e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bc3e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6bc3e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bc3e-118">Request headers</span></span>
|<span data-ttu-id="6bc3e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6bc3e-119">Header</span></span>|<span data-ttu-id="6bc3e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="6bc3e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bc3e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bc3e-121">Authorization</span></span>|<span data-ttu-id="6bc3e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bc3e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6bc3e-123">Accept</span></span>|<span data-ttu-id="6bc3e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6bc3e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bc3e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bc3e-125">Request body</span></span>
<span data-ttu-id="6bc3e-126">No corpo da solicitação, forneça uma representação JSON do objeto windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-126">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="6bc3e-127">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-127">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="6bc3e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6bc3e-128">Property</span></span>|<span data-ttu-id="6bc3e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6bc3e-129">Type</span></span>|<span data-ttu-id="6bc3e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bc3e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bc3e-131">id</span><span class="sxs-lookup"><span data-stu-id="6bc3e-131">id</span></span>|<span data-ttu-id="6bc3e-132">String</span><span class="sxs-lookup"><span data-stu-id="6bc3e-132">String</span></span>|<span data-ttu-id="6bc3e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-133">Key of the entity.</span></span> <span data-ttu-id="6bc3e-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bc3e-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bc3e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bc3e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6bc3e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bc3e-136">DateTimeOffset</span></span>|<span data-ttu-id="6bc3e-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-137">DateTime the object was last modified.</span></span> <span data-ttu-id="6bc3e-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bc3e-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bc3e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bc3e-139">createdDateTime</span></span>|<span data-ttu-id="6bc3e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bc3e-140">DateTimeOffset</span></span>|<span data-ttu-id="6bc3e-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-141">DateTime the object was created.</span></span> <span data-ttu-id="6bc3e-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bc3e-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bc3e-143">description</span><span class="sxs-lookup"><span data-stu-id="6bc3e-143">description</span></span>|<span data-ttu-id="6bc3e-144">String</span><span class="sxs-lookup"><span data-stu-id="6bc3e-144">String</span></span>|<span data-ttu-id="6bc3e-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6bc3e-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bc3e-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bc3e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6bc3e-147">displayName</span></span>|<span data-ttu-id="6bc3e-148">String</span><span class="sxs-lookup"><span data-stu-id="6bc3e-148">String</span></span>|<span data-ttu-id="6bc3e-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6bc3e-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bc3e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bc3e-151">version</span><span class="sxs-lookup"><span data-stu-id="6bc3e-151">version</span></span>|<span data-ttu-id="6bc3e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6bc3e-152">Int32</span></span>|<span data-ttu-id="6bc3e-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-153">Version of the device configuration.</span></span> <span data-ttu-id="6bc3e-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bc3e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bc3e-155">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="6bc3e-155">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="6bc3e-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bc3e-156">Boolean</span></span>|<span data-ttu-id="6bc3e-157">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-157">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="6bc3e-158">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="6bc3e-158">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="6bc3e-159">String</span><span class="sxs-lookup"><span data-stu-id="6bc3e-159">String</span></span>|<span data-ttu-id="6bc3e-160">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-160">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="6bc3e-161">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="6bc3e-161">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="6bc3e-162">String</span><span class="sxs-lookup"><span data-stu-id="6bc3e-162">String</span></span>|<span data-ttu-id="6bc3e-163">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-163">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="6bc3e-164">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="6bc3e-164">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="6bc3e-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bc3e-165">Boolean</span></span>|<span data-ttu-id="6bc3e-166">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-166">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="6bc3e-167">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="6bc3e-167">maintenanceWindowBlocked</span></span>|<span data-ttu-id="6bc3e-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bc3e-168">Boolean</span></span>|<span data-ttu-id="6bc3e-169">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-169">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="6bc3e-170">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="6bc3e-170">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="6bc3e-171">Int32</span><span class="sxs-lookup"><span data-stu-id="6bc3e-171">Int32</span></span>|<span data-ttu-id="6bc3e-172">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-172">Maintenance window duration for device updates.</span></span> <span data-ttu-id="6bc3e-173">Valores válidos: 0 a 5</span><span class="sxs-lookup"><span data-stu-id="6bc3e-173">Valid values 0 to 5</span></span>|
|<span data-ttu-id="6bc3e-174">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="6bc3e-174">maintenanceWindowStartTime</span></span>|<span data-ttu-id="6bc3e-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6bc3e-175">TimeOfDay</span></span>|<span data-ttu-id="6bc3e-176">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-176">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="6bc3e-177">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="6bc3e-177">miracastChannel</span></span>|[<span data-ttu-id="6bc3e-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="6bc3e-178">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="6bc3e-179">O canal.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-179">The channel.</span></span> <span data-ttu-id="6bc3e-180">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-180">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="6bc3e-181">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="6bc3e-181">miracastBlocked</span></span>|<span data-ttu-id="6bc3e-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bc3e-182">Boolean</span></span>|<span data-ttu-id="6bc3e-183">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-183">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="6bc3e-184">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="6bc3e-184">miracastRequirePin</span></span>|<span data-ttu-id="6bc3e-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bc3e-185">Boolean</span></span>|<span data-ttu-id="6bc3e-186">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-186">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="6bc3e-187">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="6bc3e-187">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="6bc3e-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bc3e-188">Boolean</span></span>|<span data-ttu-id="6bc3e-189">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-189">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="6bc3e-190">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="6bc3e-190">settingsBlockSessionResume</span></span>|<span data-ttu-id="6bc3e-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bc3e-191">Boolean</span></span>|<span data-ttu-id="6bc3e-192">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-192">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="6bc3e-193">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="6bc3e-193">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="6bc3e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bc3e-194">Boolean</span></span>|<span data-ttu-id="6bc3e-195">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-195">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="6bc3e-196">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="6bc3e-196">settingsDefaultVolume</span></span>|<span data-ttu-id="6bc3e-197">Int32</span><span class="sxs-lookup"><span data-stu-id="6bc3e-197">Int32</span></span>|<span data-ttu-id="6bc3e-198">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-198">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="6bc3e-199">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-199">Permitted values are 0-100.</span></span> <span data-ttu-id="6bc3e-200">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-200">The default is 45.</span></span> <span data-ttu-id="6bc3e-201">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="6bc3e-201">Valid values 0 to 100</span></span>|
|<span data-ttu-id="6bc3e-202">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6bc3e-202">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="6bc3e-203">Int32</span><span class="sxs-lookup"><span data-stu-id="6bc3e-203">Int32</span></span>|<span data-ttu-id="6bc3e-204">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-204">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="6bc3e-205">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6bc3e-205">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="6bc3e-206">Int32</span><span class="sxs-lookup"><span data-stu-id="6bc3e-206">Int32</span></span>|<span data-ttu-id="6bc3e-207">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-207">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="6bc3e-208">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6bc3e-208">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="6bc3e-209">Int32</span><span class="sxs-lookup"><span data-stu-id="6bc3e-209">Int32</span></span>|<span data-ttu-id="6bc3e-210">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-210">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="6bc3e-211">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="6bc3e-211">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="6bc3e-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="6bc3e-212">Boolean</span></span>|<span data-ttu-id="6bc3e-213">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-213">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="6bc3e-214">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="6bc3e-214">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="6bc3e-215">String</span><span class="sxs-lookup"><span data-stu-id="6bc3e-215">String</span></span>|<span data-ttu-id="6bc3e-216">The welcome screen background image URL.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-216">The welcome screen background image URL.</span></span> <span data-ttu-id="6bc3e-217">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-217">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="6bc3e-218">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="6bc3e-218">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="6bc3e-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="6bc3e-219">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="6bc3e-220">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-220">The welcome screen meeting information shown.</span></span> <span data-ttu-id="6bc3e-221">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-221">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="6bc3e-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bc3e-222">Response</span></span>
<span data-ttu-id="6bc3e-223">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-223">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bc3e-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6bc3e-224">Example</span></span>
### <a name="request"></a><span data-ttu-id="6bc3e-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bc3e-225">Request</span></span>
<span data-ttu-id="6bc3e-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1150

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="6bc3e-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bc3e-227">Response</span></span>
<span data-ttu-id="6bc3e-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6bc3e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1322

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



