# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="4a4fc-101">Criar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4a4fc-101">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="4a4fc-102">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a4fc-103">Criar um novo objeto [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4a4fc-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4a4fc-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a4fc-104">Prerequisites</span></span>
<span data-ttu-id="4a4fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a4fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4a4fc-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a4fc-107">Permission type</span></span>|<span data-ttu-id="4a4fc-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a4fc-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a4fc-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a4fc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4a4fc-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a4fc-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a4fc-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a4fc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a4fc-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-112">Not supported.</span></span>|
|<span data-ttu-id="4a4fc-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a4fc-113">Application</span></span>|<span data-ttu-id="4a4fc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a4fc-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a4fc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4a4fc-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a4fc-116">Request headers</span></span>
|<span data-ttu-id="4a4fc-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a4fc-117">Header</span></span>|<span data-ttu-id="4a4fc-118">Valor</span><span class="sxs-lookup"><span data-stu-id="4a4fc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a4fc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a4fc-119">Authorization</span></span>|<span data-ttu-id="4a4fc-120">Bearer &lt;token&gt; obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4a4fc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4a4fc-121">Accept</span></span>|<span data-ttu-id="4a4fc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4a4fc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a4fc-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a4fc-123">Request body</span></span>
<span data-ttu-id="4a4fc-124">No corpo da solicitação, forneça uma representação JSON do objeto windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="4a4fc-125">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="4a4fc-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a4fc-126">Property</span></span>|<span data-ttu-id="4a4fc-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a4fc-127">Type</span></span>|<span data-ttu-id="4a4fc-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a4fc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a4fc-129">id</span><span class="sxs-lookup"><span data-stu-id="4a4fc-129">id</span></span>|<span data-ttu-id="4a4fc-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a4fc-130">String</span></span>|<span data-ttu-id="4a4fc-131">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-131">Key of the setting.</span></span> <span data-ttu-id="4a4fc-132">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a4fc-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a4fc-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a4fc-133">lastModifiedDateTime</span></span>|<span data-ttu-id="4a4fc-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a4fc-134">DateTimeOffset</span></span>|<span data-ttu-id="4a4fc-135">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="4a4fc-136">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a4fc-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a4fc-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a4fc-137">createdDateTime</span></span>|<span data-ttu-id="4a4fc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a4fc-138">DateTimeOffset</span></span>|<span data-ttu-id="4a4fc-139">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-139">DateTime the object was created.</span></span> <span data-ttu-id="4a4fc-140">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a4fc-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a4fc-141">description</span><span class="sxs-lookup"><span data-stu-id="4a4fc-141">description</span></span>|<span data-ttu-id="4a4fc-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a4fc-142">String</span></span>|<span data-ttu-id="4a4fc-143">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4a4fc-144">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a4fc-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a4fc-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4a4fc-145">displayName</span></span>|<span data-ttu-id="4a4fc-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a4fc-146">String</span></span>|<span data-ttu-id="4a4fc-147">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4a4fc-148">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a4fc-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a4fc-149">version</span><span class="sxs-lookup"><span data-stu-id="4a4fc-149">version</span></span>|<span data-ttu-id="4a4fc-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4a4fc-150">Int32</span></span>|<span data-ttu-id="4a4fc-151">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-151">Version of the device configuration.</span></span> <span data-ttu-id="4a4fc-152">Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4a4fc-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4a4fc-153">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="4a4fc-153">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="4a4fc-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a4fc-154">Boolean</span></span>|<span data-ttu-id="4a4fc-155">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-155">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="4a4fc-156">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="4a4fc-156">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="4a4fc-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a4fc-157">String</span></span>|<span data-ttu-id="4a4fc-158">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-158">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="4a4fc-159">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="4a4fc-159">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="4a4fc-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a4fc-160">String</span></span>|<span data-ttu-id="4a4fc-161">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-161">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="4a4fc-162">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="4a4fc-162">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="4a4fc-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a4fc-163">Boolean</span></span>|<span data-ttu-id="4a4fc-164">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-164">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="4a4fc-165">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="4a4fc-165">maintenanceWindowBlocked</span></span>|<span data-ttu-id="4a4fc-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a4fc-166">Boolean</span></span>|<span data-ttu-id="4a4fc-167">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-167">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="4a4fc-168">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="4a4fc-168">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="4a4fc-169">Int32</span><span class="sxs-lookup"><span data-stu-id="4a4fc-169">Int32</span></span>|<span data-ttu-id="4a4fc-170">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-170">Maintenance window duration for device updates.</span></span> <span data-ttu-id="4a4fc-171">Valores válidos de 1 a 5</span><span class="sxs-lookup"><span data-stu-id="4a4fc-171">Valid values 1 to 5</span></span>|
|<span data-ttu-id="4a4fc-172">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="4a4fc-172">maintenanceWindowStartTime</span></span>|<span data-ttu-id="4a4fc-173">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4a4fc-173">TimeOfDay</span></span>|<span data-ttu-id="4a4fc-174">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-174">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="4a4fc-175">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="4a4fc-175">miracastChannel</span></span>|<span data-ttu-id="4a4fc-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a4fc-176">String</span></span>|<span data-ttu-id="4a4fc-177">O canal.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-177">The channel.</span></span> <span data-ttu-id="4a4fc-178">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-178">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="4a4fc-179">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="4a4fc-179">miracastBlocked</span></span>|<span data-ttu-id="4a4fc-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a4fc-180">Boolean</span></span>|<span data-ttu-id="4a4fc-181">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-181">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="4a4fc-182">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="4a4fc-182">miracastRequirePin</span></span>|<span data-ttu-id="4a4fc-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a4fc-183">Boolean</span></span>|<span data-ttu-id="4a4fc-184">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-184">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="4a4fc-185">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="4a4fc-185">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="4a4fc-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a4fc-186">Boolean</span></span>|<span data-ttu-id="4a4fc-187">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-187">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="4a4fc-188">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="4a4fc-188">settingsBlockSessionResume</span></span>|<span data-ttu-id="4a4fc-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a4fc-189">Boolean</span></span>|<span data-ttu-id="4a4fc-190">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-190">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="4a4fc-191">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="4a4fc-191">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="4a4fc-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a4fc-192">Boolean</span></span>|<span data-ttu-id="4a4fc-193">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-193">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="4a4fc-194">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="4a4fc-194">settingsDefaultVolume</span></span>|<span data-ttu-id="4a4fc-195">Int32</span><span class="sxs-lookup"><span data-stu-id="4a4fc-195">Int32</span></span>|<span data-ttu-id="4a4fc-196">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-196">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="4a4fc-197">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-197">Permitted values are 0-100.</span></span> <span data-ttu-id="4a4fc-198">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-198">The default is zero.</span></span> <span data-ttu-id="4a4fc-199">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="4a4fc-199">Valid values 0 to 100</span></span>|
|<span data-ttu-id="4a4fc-200">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="4a4fc-200">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="4a4fc-201">Int32</span><span class="sxs-lookup"><span data-stu-id="4a4fc-201">Int32</span></span>|<span data-ttu-id="4a4fc-202">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-202">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="4a4fc-203">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="4a4fc-203">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="4a4fc-204">Int32</span><span class="sxs-lookup"><span data-stu-id="4a4fc-204">Int32</span></span>|<span data-ttu-id="4a4fc-205">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-205">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="4a4fc-206">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="4a4fc-206">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="4a4fc-207">Int32</span><span class="sxs-lookup"><span data-stu-id="4a4fc-207">Int32</span></span>|<span data-ttu-id="4a4fc-208">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-208">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="4a4fc-209">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="4a4fc-209">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="4a4fc-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a4fc-210">Boolean</span></span>|<span data-ttu-id="4a4fc-211">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-211">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="4a4fc-212">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="4a4fc-212">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="4a4fc-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a4fc-213">String</span></span>|<span data-ttu-id="4a4fc-214">The welcome screen background image URL.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-214">The welcome screen background image URL.</span></span> <span data-ttu-id="4a4fc-215">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-215">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="4a4fc-216">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="4a4fc-216">welcomeScreenMeetingInformation</span></span>|<span data-ttu-id="4a4fc-217">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a4fc-217">String</span></span>|<span data-ttu-id="4a4fc-218">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-218">The welcome screen meeting information shown.</span></span> <span data-ttu-id="4a4fc-219">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-219">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="4a4fc-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a4fc-220">Response</span></span>
<span data-ttu-id="4a4fc-221">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10TeamGeneralConfiguration](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-221">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a4fc-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a4fc-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a4fc-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a4fc-223">Request</span></span>
<span data-ttu-id="4a4fc-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1214

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="4a4fc-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a4fc-225">Response</span></span>
<span data-ttu-id="4a4fc-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a4fc-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



