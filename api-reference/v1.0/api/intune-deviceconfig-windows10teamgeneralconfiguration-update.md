---
title: Atualizar windows10TeamGeneralConfiguration
description: Atualizar as propriedades de um objeto windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab049fecd546462123796aff2fd3ac975e71932f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251017"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="d62ac-103">Atualizar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="d62ac-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="d62ac-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d62ac-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d62ac-105">Atualizar as propriedades de um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d62ac-105">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d62ac-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d62ac-106">Prerequisites</span></span>
<span data-ttu-id="d62ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d62ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d62ac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d62ac-109">Permission type</span></span>|<span data-ttu-id="d62ac-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d62ac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d62ac-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d62ac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d62ac-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d62ac-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d62ac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d62ac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d62ac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d62ac-114">Not supported.</span></span>|
|<span data-ttu-id="d62ac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d62ac-115">Application</span></span>|<span data-ttu-id="d62ac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d62ac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d62ac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d62ac-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d62ac-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d62ac-118">Request headers</span></span>
|<span data-ttu-id="d62ac-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d62ac-119">Header</span></span>|<span data-ttu-id="d62ac-120">Valor</span><span class="sxs-lookup"><span data-stu-id="d62ac-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d62ac-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d62ac-121">Authorization</span></span>|<span data-ttu-id="d62ac-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d62ac-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d62ac-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d62ac-123">Accept</span></span>|<span data-ttu-id="d62ac-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d62ac-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d62ac-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d62ac-125">Request body</span></span>
<span data-ttu-id="d62ac-126">No corpo da solicitação, forneça uma representação JSON do objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d62ac-126">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="d62ac-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d62ac-127">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="d62ac-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d62ac-128">Property</span></span>|<span data-ttu-id="d62ac-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d62ac-129">Type</span></span>|<span data-ttu-id="d62ac-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d62ac-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d62ac-131">id</span><span class="sxs-lookup"><span data-stu-id="d62ac-131">id</span></span>|<span data-ttu-id="d62ac-132">String</span><span class="sxs-lookup"><span data-stu-id="d62ac-132">String</span></span>|<span data-ttu-id="d62ac-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d62ac-133">Key of the entity.</span></span> <span data-ttu-id="d62ac-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d62ac-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d62ac-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d62ac-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d62ac-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d62ac-136">DateTimeOffset</span></span>|<span data-ttu-id="d62ac-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d62ac-137">DateTime the object was last modified.</span></span> <span data-ttu-id="d62ac-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d62ac-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d62ac-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d62ac-139">createdDateTime</span></span>|<span data-ttu-id="d62ac-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d62ac-140">DateTimeOffset</span></span>|<span data-ttu-id="d62ac-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d62ac-141">DateTime the object was created.</span></span> <span data-ttu-id="d62ac-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d62ac-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d62ac-143">description</span><span class="sxs-lookup"><span data-stu-id="d62ac-143">description</span></span>|<span data-ttu-id="d62ac-144">String</span><span class="sxs-lookup"><span data-stu-id="d62ac-144">String</span></span>|<span data-ttu-id="d62ac-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d62ac-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d62ac-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d62ac-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d62ac-147">displayName</span><span class="sxs-lookup"><span data-stu-id="d62ac-147">displayName</span></span>|<span data-ttu-id="d62ac-148">String</span><span class="sxs-lookup"><span data-stu-id="d62ac-148">String</span></span>|<span data-ttu-id="d62ac-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d62ac-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d62ac-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d62ac-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d62ac-151">version</span><span class="sxs-lookup"><span data-stu-id="d62ac-151">version</span></span>|<span data-ttu-id="d62ac-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d62ac-152">Int32</span></span>|<span data-ttu-id="d62ac-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d62ac-153">Version of the device configuration.</span></span> <span data-ttu-id="d62ac-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d62ac-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d62ac-155">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="d62ac-155">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="d62ac-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="d62ac-156">Boolean</span></span>|<span data-ttu-id="d62ac-157">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="d62ac-157">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="d62ac-158">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="d62ac-158">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="d62ac-159">String</span><span class="sxs-lookup"><span data-stu-id="d62ac-159">String</span></span>|<span data-ttu-id="d62ac-160">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="d62ac-160">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="d62ac-161">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="d62ac-161">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="d62ac-162">String</span><span class="sxs-lookup"><span data-stu-id="d62ac-162">String</span></span>|<span data-ttu-id="d62ac-163">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="d62ac-163">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="d62ac-164">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="d62ac-164">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="d62ac-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="d62ac-165">Boolean</span></span>|<span data-ttu-id="d62ac-166">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="d62ac-166">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="d62ac-167">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="d62ac-167">maintenanceWindowBlocked</span></span>|<span data-ttu-id="d62ac-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="d62ac-168">Boolean</span></span>|<span data-ttu-id="d62ac-169">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d62ac-169">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="d62ac-170">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="d62ac-170">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="d62ac-171">Int32</span><span class="sxs-lookup"><span data-stu-id="d62ac-171">Int32</span></span>|<span data-ttu-id="d62ac-172">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d62ac-172">Maintenance window duration for device updates.</span></span> <span data-ttu-id="d62ac-173">Valores válidos: 0 a 5</span><span class="sxs-lookup"><span data-stu-id="d62ac-173">Valid values 0 to 5</span></span>|
|<span data-ttu-id="d62ac-174">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="d62ac-174">maintenanceWindowStartTime</span></span>|<span data-ttu-id="d62ac-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d62ac-175">TimeOfDay</span></span>|<span data-ttu-id="d62ac-176">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d62ac-176">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="d62ac-177">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="d62ac-177">miracastChannel</span></span>|[<span data-ttu-id="d62ac-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="d62ac-178">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="d62ac-179">O canal.</span><span class="sxs-lookup"><span data-stu-id="d62ac-179">The channel.</span></span> <span data-ttu-id="d62ac-180">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="d62ac-180">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="d62ac-181">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="d62ac-181">miracastBlocked</span></span>|<span data-ttu-id="d62ac-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="d62ac-182">Boolean</span></span>|<span data-ttu-id="d62ac-183">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="d62ac-183">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="d62ac-184">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="d62ac-184">miracastRequirePin</span></span>|<span data-ttu-id="d62ac-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="d62ac-185">Boolean</span></span>|<span data-ttu-id="d62ac-186">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="d62ac-186">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="d62ac-187">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="d62ac-187">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="d62ac-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="d62ac-188">Boolean</span></span>|<span data-ttu-id="d62ac-189">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="d62ac-189">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="d62ac-190">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="d62ac-190">settingsBlockSessionResume</span></span>|<span data-ttu-id="d62ac-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="d62ac-191">Boolean</span></span>|<span data-ttu-id="d62ac-192">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="d62ac-192">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="d62ac-193">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="d62ac-193">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="d62ac-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d62ac-194">Boolean</span></span>|<span data-ttu-id="d62ac-195">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="d62ac-195">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="d62ac-196">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="d62ac-196">settingsDefaultVolume</span></span>|<span data-ttu-id="d62ac-197">Int32</span><span class="sxs-lookup"><span data-stu-id="d62ac-197">Int32</span></span>|<span data-ttu-id="d62ac-198">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="d62ac-198">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="d62ac-199">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="d62ac-199">Permitted values are 0-100.</span></span> <span data-ttu-id="d62ac-200">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="d62ac-200">The default is 45.</span></span> <span data-ttu-id="d62ac-201">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="d62ac-201">Valid values 0 to 100</span></span>|
|<span data-ttu-id="d62ac-202">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d62ac-202">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="d62ac-203">Int32</span><span class="sxs-lookup"><span data-stu-id="d62ac-203">Int32</span></span>|<span data-ttu-id="d62ac-204">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="d62ac-204">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="d62ac-205">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d62ac-205">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="d62ac-206">Int32</span><span class="sxs-lookup"><span data-stu-id="d62ac-206">Int32</span></span>|<span data-ttu-id="d62ac-207">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="d62ac-207">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="d62ac-208">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d62ac-208">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="d62ac-209">Int32</span><span class="sxs-lookup"><span data-stu-id="d62ac-209">Int32</span></span>|<span data-ttu-id="d62ac-210">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="d62ac-210">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="d62ac-211">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="d62ac-211">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="d62ac-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="d62ac-212">Boolean</span></span>|<span data-ttu-id="d62ac-213">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="d62ac-213">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="d62ac-214">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="d62ac-214">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="d62ac-215">String</span><span class="sxs-lookup"><span data-stu-id="d62ac-215">String</span></span>|<span data-ttu-id="d62ac-216">The welcome screen background image URL.</span><span class="sxs-lookup"><span data-stu-id="d62ac-216">The welcome screen background image URL.</span></span> <span data-ttu-id="d62ac-217">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="d62ac-217">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="d62ac-218">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="d62ac-218">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="d62ac-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="d62ac-219">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="d62ac-220">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="d62ac-220">The welcome screen meeting information shown.</span></span> <span data-ttu-id="d62ac-221">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="d62ac-221">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="d62ac-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="d62ac-222">Response</span></span>
<span data-ttu-id="d62ac-223">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d62ac-223">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d62ac-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d62ac-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="d62ac-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d62ac-225">Request</span></span>
<span data-ttu-id="d62ac-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d62ac-226">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d62ac-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="d62ac-227">Response</span></span>
<span data-ttu-id="d62ac-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d62ac-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



