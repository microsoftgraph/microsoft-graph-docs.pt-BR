# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="6aed6-101">Atualizar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="6aed6-101">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="6aed6-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6aed6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6aed6-103">Atualizar as propriedades de um objeto [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6aed6-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6aed6-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6aed6-104">Prerequisites</span></span>
<span data-ttu-id="6aed6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6aed6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6aed6-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6aed6-107">Permission type</span></span>|<span data-ttu-id="6aed6-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6aed6-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6aed6-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6aed6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6aed6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aed6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6aed6-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6aed6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6aed6-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6aed6-112">Not supported.</span></span>|
|<span data-ttu-id="6aed6-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6aed6-113">Application</span></span>|<span data-ttu-id="6aed6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6aed6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6aed6-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6aed6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6aed6-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6aed6-116">Request headers</span></span>
|<span data-ttu-id="6aed6-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6aed6-117">Header</span></span>|<span data-ttu-id="6aed6-118">Valor</span><span class="sxs-lookup"><span data-stu-id="6aed6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6aed6-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="6aed6-119">Authorization</span></span>|<span data-ttu-id="6aed6-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6aed6-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6aed6-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6aed6-121">Accept</span></span>|<span data-ttu-id="6aed6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6aed6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6aed6-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6aed6-123">Request body</span></span>
<span data-ttu-id="6aed6-124">No corpo da solicitação, forneça uma representação JSON do objeto [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6aed6-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="6aed6-125">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6aed6-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="6aed6-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6aed6-126">Property</span></span>|<span data-ttu-id="6aed6-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="6aed6-127">Type</span></span>|<span data-ttu-id="6aed6-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="6aed6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aed6-129">id</span><span class="sxs-lookup"><span data-stu-id="6aed6-129">id</span></span>|<span data-ttu-id="6aed6-130">String</span><span class="sxs-lookup"><span data-stu-id="6aed6-130">String</span></span>|<span data-ttu-id="6aed6-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6aed6-131">Key of the setting.</span></span> <span data-ttu-id="6aed6-132">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6aed6-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6aed6-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6aed6-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6aed6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6aed6-134">DateTimeOffset</span></span>|<span data-ttu-id="6aed6-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6aed6-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="6aed6-136">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6aed6-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6aed6-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6aed6-137">createdDateTime</span></span>|<span data-ttu-id="6aed6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6aed6-138">DateTimeOffset</span></span>|<span data-ttu-id="6aed6-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6aed6-139">DateTime the object was created.</span></span> <span data-ttu-id="6aed6-140">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6aed6-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6aed6-141">descrição</span><span class="sxs-lookup"><span data-stu-id="6aed6-141">description</span></span>|<span data-ttu-id="6aed6-142">String</span><span class="sxs-lookup"><span data-stu-id="6aed6-142">String</span></span>|<span data-ttu-id="6aed6-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6aed6-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6aed6-144">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6aed6-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6aed6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="6aed6-145">displayName</span></span>|<span data-ttu-id="6aed6-146">String</span><span class="sxs-lookup"><span data-stu-id="6aed6-146">String</span></span>|<span data-ttu-id="6aed6-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6aed6-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6aed6-148">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6aed6-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6aed6-149">version</span><span class="sxs-lookup"><span data-stu-id="6aed6-149">version</span></span>|<span data-ttu-id="6aed6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6aed6-150">Int32</span></span>|<span data-ttu-id="6aed6-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6aed6-151">Version of the device configuration.</span></span> <span data-ttu-id="6aed6-152">Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6aed6-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6aed6-153">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="6aed6-153">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="6aed6-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aed6-154">Boolean</span></span>|<span data-ttu-id="6aed6-155">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="6aed6-155">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="6aed6-156">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="6aed6-156">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="6aed6-157">String</span><span class="sxs-lookup"><span data-stu-id="6aed6-157">String</span></span>|<span data-ttu-id="6aed6-158">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="6aed6-158">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="6aed6-159">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="6aed6-159">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="6aed6-160">String</span><span class="sxs-lookup"><span data-stu-id="6aed6-160">String</span></span>|<span data-ttu-id="6aed6-161">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="6aed6-161">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="6aed6-162">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="6aed6-162">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="6aed6-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aed6-163">Boolean</span></span>|<span data-ttu-id="6aed6-164">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="6aed6-164">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="6aed6-165">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="6aed6-165">maintenanceWindowBlocked</span></span>|<span data-ttu-id="6aed6-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aed6-166">Boolean</span></span>|<span data-ttu-id="6aed6-167">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6aed6-167">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="6aed6-168">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="6aed6-168">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="6aed6-169">Int32</span><span class="sxs-lookup"><span data-stu-id="6aed6-169">Int32</span></span>|<span data-ttu-id="6aed6-170">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6aed6-170">Maintenance window duration for device updates.</span></span> <span data-ttu-id="6aed6-171">Valores válidos de 1 a 5</span><span class="sxs-lookup"><span data-stu-id="6aed6-171">Valid values 1 to 5</span></span>|
|<span data-ttu-id="6aed6-172">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="6aed6-172">maintenanceWindowStartTime</span></span>|<span data-ttu-id="6aed6-173">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="6aed6-173">TimeOfDay</span></span>|<span data-ttu-id="6aed6-174">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6aed6-174">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="6aed6-175">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="6aed6-175">miracastChannel</span></span>|<span data-ttu-id="6aed6-176">String</span><span class="sxs-lookup"><span data-stu-id="6aed6-176">String</span></span>|<span data-ttu-id="6aed6-177">O canal.</span><span class="sxs-lookup"><span data-stu-id="6aed6-177">The channel.</span></span> <span data-ttu-id="6aed6-178">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="6aed6-178">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="6aed6-179">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="6aed6-179">miracastBlocked</span></span>|<span data-ttu-id="6aed6-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aed6-180">Boolean</span></span>|<span data-ttu-id="6aed6-181">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="6aed6-181">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="6aed6-182">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="6aed6-182">miracastRequirePin</span></span>|<span data-ttu-id="6aed6-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aed6-183">Boolean</span></span>|<span data-ttu-id="6aed6-184">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="6aed6-184">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="6aed6-185">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="6aed6-185">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="6aed6-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aed6-186">Boolean</span></span>|<span data-ttu-id="6aed6-187">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="6aed6-187">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="6aed6-188">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="6aed6-188">settingsBlockSessionResume</span></span>|<span data-ttu-id="6aed6-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aed6-189">Boolean</span></span>|<span data-ttu-id="6aed6-190">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="6aed6-190">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="6aed6-191">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="6aed6-191">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="6aed6-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aed6-192">Boolean</span></span>|<span data-ttu-id="6aed6-193">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="6aed6-193">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="6aed6-194">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="6aed6-194">settingsDefaultVolume</span></span>|<span data-ttu-id="6aed6-195">Int32</span><span class="sxs-lookup"><span data-stu-id="6aed6-195">Int32</span></span>|<span data-ttu-id="6aed6-196">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="6aed6-196">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="6aed6-197">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="6aed6-197">Permitted values are 0-100.</span></span> <span data-ttu-id="6aed6-198">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="6aed6-198">The default is zero.</span></span> <span data-ttu-id="6aed6-199">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="6aed6-199">Valid values 0 to 100</span></span>|
|<span data-ttu-id="6aed6-200">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6aed6-200">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="6aed6-201">Int32</span><span class="sxs-lookup"><span data-stu-id="6aed6-201">Int32</span></span>|<span data-ttu-id="6aed6-202">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="6aed6-202">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="6aed6-203">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6aed6-203">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="6aed6-204">Int32</span><span class="sxs-lookup"><span data-stu-id="6aed6-204">Int32</span></span>|<span data-ttu-id="6aed6-205">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="6aed6-205">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="6aed6-206">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="6aed6-206">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="6aed6-207">Int32</span><span class="sxs-lookup"><span data-stu-id="6aed6-207">Int32</span></span>|<span data-ttu-id="6aed6-208">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="6aed6-208">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="6aed6-209">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="6aed6-209">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="6aed6-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="6aed6-210">Boolean</span></span>|<span data-ttu-id="6aed6-211">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="6aed6-211">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="6aed6-212">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="6aed6-212">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="6aed6-213">String</span><span class="sxs-lookup"><span data-stu-id="6aed6-213">String</span></span>|<span data-ttu-id="6aed6-214">A URL da imagem de tela de fundo da tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="6aed6-214">The welcome screen background image URL.</span></span> <span data-ttu-id="6aed6-215">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="6aed6-215">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="6aed6-216">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="6aed6-216">welcomeScreenMeetingInformation</span></span>|<span data-ttu-id="6aed6-217">String</span><span class="sxs-lookup"><span data-stu-id="6aed6-217">String</span></span>|<span data-ttu-id="6aed6-218">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="6aed6-218">The welcome screen meeting information shown.</span></span> <span data-ttu-id="6aed6-219">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="6aed6-219">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="6aed6-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aed6-220">Response</span></span>
<span data-ttu-id="6aed6-221">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6aed6-221">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6aed6-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6aed6-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="6aed6-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6aed6-223">Request</span></span>
<span data-ttu-id="6aed6-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6aed6-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1142

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="6aed6-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="6aed6-225">Response</span></span>
<span data-ttu-id="6aed6-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6aed6-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



