---
title: Atualizar windows10TeamGeneralConfiguration
description: Atualizar as propriedades de um objeto windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a90858f35f0ae555ea8a74f2cfc4eed26cd7ea3a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442002"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="98605-103">Atualizar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="98605-103">Update windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="98605-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98605-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98605-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98605-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98605-106">Atualizar as propriedades de um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="98605-106">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98605-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98605-107">Prerequisites</span></span>
<span data-ttu-id="98605-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98605-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98605-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98605-110">Permission type</span></span>|<span data-ttu-id="98605-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98605-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98605-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98605-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98605-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98605-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98605-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98605-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98605-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98605-115">Not supported.</span></span>|
|<span data-ttu-id="98605-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98605-116">Application</span></span>|<span data-ttu-id="98605-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98605-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98605-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98605-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="98605-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98605-119">Request headers</span></span>
|<span data-ttu-id="98605-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98605-120">Header</span></span>|<span data-ttu-id="98605-121">Valor</span><span class="sxs-lookup"><span data-stu-id="98605-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98605-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="98605-122">Authorization</span></span>|<span data-ttu-id="98605-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98605-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98605-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98605-124">Accept</span></span>|<span data-ttu-id="98605-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98605-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98605-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98605-126">Request body</span></span>
<span data-ttu-id="98605-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="98605-127">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="98605-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="98605-128">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="98605-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98605-129">Property</span></span>|<span data-ttu-id="98605-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="98605-130">Type</span></span>|<span data-ttu-id="98605-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="98605-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98605-132">id</span><span class="sxs-lookup"><span data-stu-id="98605-132">id</span></span>|<span data-ttu-id="98605-133">String</span><span class="sxs-lookup"><span data-stu-id="98605-133">String</span></span>|<span data-ttu-id="98605-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="98605-134">Key of the entity.</span></span> <span data-ttu-id="98605-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98605-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98605-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98605-136">lastModifiedDateTime</span></span>|<span data-ttu-id="98605-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98605-137">DateTimeOffset</span></span>|<span data-ttu-id="98605-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="98605-138">DateTime the object was last modified.</span></span> <span data-ttu-id="98605-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98605-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98605-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98605-140">createdDateTime</span></span>|<span data-ttu-id="98605-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98605-141">DateTimeOffset</span></span>|<span data-ttu-id="98605-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="98605-142">DateTime the object was created.</span></span> <span data-ttu-id="98605-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98605-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98605-144">description</span><span class="sxs-lookup"><span data-stu-id="98605-144">description</span></span>|<span data-ttu-id="98605-145">String</span><span class="sxs-lookup"><span data-stu-id="98605-145">String</span></span>|<span data-ttu-id="98605-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98605-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="98605-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98605-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98605-148">displayName</span><span class="sxs-lookup"><span data-stu-id="98605-148">displayName</span></span>|<span data-ttu-id="98605-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98605-149">String</span></span>|<span data-ttu-id="98605-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98605-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="98605-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98605-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98605-152">versão</span><span class="sxs-lookup"><span data-stu-id="98605-152">version</span></span>|<span data-ttu-id="98605-153">Int32</span><span class="sxs-lookup"><span data-stu-id="98605-153">Int32</span></span>|<span data-ttu-id="98605-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98605-154">Version of the device configuration.</span></span> <span data-ttu-id="98605-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="98605-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="98605-156">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="98605-156">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="98605-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="98605-157">Boolean</span></span>|<span data-ttu-id="98605-158">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="98605-158">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="98605-159">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="98605-159">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="98605-160">String</span><span class="sxs-lookup"><span data-stu-id="98605-160">String</span></span>|<span data-ttu-id="98605-161">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="98605-161">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="98605-162">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="98605-162">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="98605-163">String</span><span class="sxs-lookup"><span data-stu-id="98605-163">String</span></span>|<span data-ttu-id="98605-164">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="98605-164">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="98605-165">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="98605-165">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="98605-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="98605-166">Boolean</span></span>|<span data-ttu-id="98605-167">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="98605-167">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="98605-168">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="98605-168">maintenanceWindowBlocked</span></span>|<span data-ttu-id="98605-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="98605-169">Boolean</span></span>|<span data-ttu-id="98605-170">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98605-170">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="98605-171">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="98605-171">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="98605-172">Int32</span><span class="sxs-lookup"><span data-stu-id="98605-172">Int32</span></span>|<span data-ttu-id="98605-173">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98605-173">Maintenance window duration for device updates.</span></span> <span data-ttu-id="98605-174">Valores válidos: 0 a 5</span><span class="sxs-lookup"><span data-stu-id="98605-174">Valid values 0 to 5</span></span>|
|<span data-ttu-id="98605-175">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="98605-175">maintenanceWindowStartTime</span></span>|<span data-ttu-id="98605-176">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="98605-176">TimeOfDay</span></span>|<span data-ttu-id="98605-177">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="98605-177">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="98605-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="98605-178">miracastChannel</span></span>|[<span data-ttu-id="98605-179">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="98605-179">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="98605-180">O canal.</span><span class="sxs-lookup"><span data-stu-id="98605-180">The channel.</span></span> <span data-ttu-id="98605-181">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="98605-181">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="98605-182">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="98605-182">miracastBlocked</span></span>|<span data-ttu-id="98605-183">Booliano</span><span class="sxs-lookup"><span data-stu-id="98605-183">Boolean</span></span>|<span data-ttu-id="98605-184">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="98605-184">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="98605-185">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="98605-185">miracastRequirePin</span></span>|<span data-ttu-id="98605-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="98605-186">Boolean</span></span>|<span data-ttu-id="98605-187">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="98605-187">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="98605-188">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="98605-188">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="98605-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="98605-189">Boolean</span></span>|<span data-ttu-id="98605-190">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="98605-190">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="98605-191">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="98605-191">settingsBlockSessionResume</span></span>|<span data-ttu-id="98605-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="98605-192">Boolean</span></span>|<span data-ttu-id="98605-193">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="98605-193">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="98605-194">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="98605-194">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="98605-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="98605-195">Boolean</span></span>|<span data-ttu-id="98605-196">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="98605-196">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="98605-197">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="98605-197">settingsDefaultVolume</span></span>|<span data-ttu-id="98605-198">Int32</span><span class="sxs-lookup"><span data-stu-id="98605-198">Int32</span></span>|<span data-ttu-id="98605-199">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="98605-199">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="98605-200">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="98605-200">Permitted values are 0-100.</span></span> <span data-ttu-id="98605-201">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="98605-201">The default is 45.</span></span> <span data-ttu-id="98605-202">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="98605-202">Valid values 0 to 100</span></span>|
|<span data-ttu-id="98605-203">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="98605-203">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="98605-204">Int32</span><span class="sxs-lookup"><span data-stu-id="98605-204">Int32</span></span>|<span data-ttu-id="98605-205">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="98605-205">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="98605-206">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="98605-206">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="98605-207">Int32</span><span class="sxs-lookup"><span data-stu-id="98605-207">Int32</span></span>|<span data-ttu-id="98605-208">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="98605-208">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="98605-209">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="98605-209">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="98605-210">Int32</span><span class="sxs-lookup"><span data-stu-id="98605-210">Int32</span></span>|<span data-ttu-id="98605-211">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="98605-211">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="98605-212">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="98605-212">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="98605-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="98605-213">Boolean</span></span>|<span data-ttu-id="98605-214">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="98605-214">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="98605-215">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="98605-215">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="98605-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98605-216">String</span></span>|<span data-ttu-id="98605-217">The welcome screen background image URL.</span><span class="sxs-lookup"><span data-stu-id="98605-217">The welcome screen background image URL.</span></span> <span data-ttu-id="98605-218">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="98605-218">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="98605-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="98605-219">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="98605-220">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="98605-220">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="98605-221">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="98605-221">The welcome screen meeting information shown.</span></span> <span data-ttu-id="98605-222">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="98605-222">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="98605-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="98605-223">Response</span></span>
<span data-ttu-id="98605-224">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98605-224">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98605-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98605-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="98605-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98605-226">Request</span></span>
<span data-ttu-id="98605-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98605-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="98605-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="98605-228">Response</span></span>
<span data-ttu-id="98605-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98605-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






