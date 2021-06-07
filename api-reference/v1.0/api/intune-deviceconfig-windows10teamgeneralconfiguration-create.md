---
title: Criar windows10TeamGeneralConfiguration
description: Criar um novo objeto windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8286551f14d7fcedaa7233814240afe5c4610abe
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760444"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="debc4-103">Criar windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="debc4-103">Create windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="debc4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="debc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="debc4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="debc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="debc4-106">Criar um novo objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="debc4-106">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="debc4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="debc4-107">Prerequisites</span></span>
<span data-ttu-id="debc4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="debc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="debc4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="debc4-110">Permission type</span></span>|<span data-ttu-id="debc4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="debc4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="debc4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="debc4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="debc4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="debc4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="debc4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="debc4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="debc4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="debc4-115">Not supported.</span></span>|
|<span data-ttu-id="debc4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="debc4-116">Application</span></span>|<span data-ttu-id="debc4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="debc4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="debc4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="debc4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="debc4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="debc4-119">Request headers</span></span>
|<span data-ttu-id="debc4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="debc4-120">Header</span></span>|<span data-ttu-id="debc4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="debc4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="debc4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="debc4-122">Authorization</span></span>|<span data-ttu-id="debc4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="debc4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="debc4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="debc4-124">Accept</span></span>|<span data-ttu-id="debc4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="debc4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="debc4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="debc4-126">Request body</span></span>
<span data-ttu-id="debc4-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="debc4-127">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="debc4-128">A tabela a seguir mostra as propriedades obrigatórias ao criar windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="debc4-128">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="debc4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="debc4-129">Property</span></span>|<span data-ttu-id="debc4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="debc4-130">Type</span></span>|<span data-ttu-id="debc4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="debc4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="debc4-132">id</span><span class="sxs-lookup"><span data-stu-id="debc4-132">id</span></span>|<span data-ttu-id="debc4-133">String</span><span class="sxs-lookup"><span data-stu-id="debc4-133">String</span></span>|<span data-ttu-id="debc4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="debc4-134">Key of the entity.</span></span> <span data-ttu-id="debc4-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="debc4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="debc4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="debc4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="debc4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="debc4-137">DateTimeOffset</span></span>|<span data-ttu-id="debc4-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="debc4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="debc4-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="debc4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="debc4-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="debc4-140">createdDateTime</span></span>|<span data-ttu-id="debc4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="debc4-141">DateTimeOffset</span></span>|<span data-ttu-id="debc4-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="debc4-142">DateTime the object was created.</span></span> <span data-ttu-id="debc4-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="debc4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="debc4-144">description</span><span class="sxs-lookup"><span data-stu-id="debc4-144">description</span></span>|<span data-ttu-id="debc4-145">String</span><span class="sxs-lookup"><span data-stu-id="debc4-145">String</span></span>|<span data-ttu-id="debc4-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="debc4-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="debc4-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="debc4-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="debc4-148">displayName</span><span class="sxs-lookup"><span data-stu-id="debc4-148">displayName</span></span>|<span data-ttu-id="debc4-149">String</span><span class="sxs-lookup"><span data-stu-id="debc4-149">String</span></span>|<span data-ttu-id="debc4-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="debc4-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="debc4-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="debc4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="debc4-152">versão</span><span class="sxs-lookup"><span data-stu-id="debc4-152">version</span></span>|<span data-ttu-id="debc4-153">Int32</span><span class="sxs-lookup"><span data-stu-id="debc4-153">Int32</span></span>|<span data-ttu-id="debc4-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="debc4-154">Version of the device configuration.</span></span> <span data-ttu-id="debc4-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="debc4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="debc4-156">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="debc4-156">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="debc4-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="debc4-157">Boolean</span></span>|<span data-ttu-id="debc4-158">Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="debc4-158">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="debc4-159">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="debc4-159">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="debc4-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="debc4-160">String</span></span>|<span data-ttu-id="debc4-161">A ID do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="debc4-161">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="debc4-162">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="debc4-162">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="debc4-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="debc4-163">String</span></span>|<span data-ttu-id="debc4-164">A chave do espaço de trabalho dos Insights Operacionais do Azure.</span><span class="sxs-lookup"><span data-stu-id="debc4-164">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="debc4-165">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="debc4-165">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="debc4-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="debc4-166">Boolean</span></span>|<span data-ttu-id="debc4-167">Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.</span><span class="sxs-lookup"><span data-stu-id="debc4-167">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="debc4-168">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="debc4-168">maintenanceWindowBlocked</span></span>|<span data-ttu-id="debc4-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="debc4-169">Boolean</span></span>|<span data-ttu-id="debc4-170">Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="debc4-170">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="debc4-171">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="debc4-171">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="debc4-172">Int32</span><span class="sxs-lookup"><span data-stu-id="debc4-172">Int32</span></span>|<span data-ttu-id="debc4-173">Duração da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="debc4-173">Maintenance window duration for device updates.</span></span> <span data-ttu-id="debc4-174">Valores válidos: 0 a 5</span><span class="sxs-lookup"><span data-stu-id="debc4-174">Valid values 0 to 5</span></span>|
|<span data-ttu-id="debc4-175">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="debc4-175">maintenanceWindowStartTime</span></span>|<span data-ttu-id="debc4-176">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="debc4-176">TimeOfDay</span></span>|<span data-ttu-id="debc4-177">Hora de Início da janela de manutenção para atualizações do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="debc4-177">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="debc4-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="debc4-178">miracastChannel</span></span>|[<span data-ttu-id="debc4-179">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="debc4-179">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="debc4-180">O canal.</span><span class="sxs-lookup"><span data-stu-id="debc4-180">The channel.</span></span> <span data-ttu-id="debc4-181">Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="debc4-181">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="debc4-182">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="debc4-182">miracastBlocked</span></span>|<span data-ttu-id="debc4-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="debc4-183">Boolean</span></span>|<span data-ttu-id="debc4-184">Indica se a projeção sem fio deve ou não ser bloqueada.</span><span class="sxs-lookup"><span data-stu-id="debc4-184">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="debc4-185">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="debc4-185">miracastRequirePin</span></span>|<span data-ttu-id="debc4-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="debc4-186">Boolean</span></span>|<span data-ttu-id="debc4-187">Indica se será exigido um pin para a projeção sem fio.</span><span class="sxs-lookup"><span data-stu-id="debc4-187">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="debc4-188">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="debc4-188">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="debc4-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="debc4-189">Boolean</span></span>|<span data-ttu-id="debc4-190">Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.</span><span class="sxs-lookup"><span data-stu-id="debc4-190">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="debc4-191">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="debc4-191">settingsBlockSessionResume</span></span>|<span data-ttu-id="debc4-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="debc4-192">Boolean</span></span>|<span data-ttu-id="debc4-193">Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.</span><span class="sxs-lookup"><span data-stu-id="debc4-193">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="debc4-194">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="debc4-194">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="debc4-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="debc4-195">Boolean</span></span>|<span data-ttu-id="debc4-196">Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.</span><span class="sxs-lookup"><span data-stu-id="debc4-196">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="debc4-197">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="debc4-197">settingsDefaultVolume</span></span>|<span data-ttu-id="debc4-198">Int32</span><span class="sxs-lookup"><span data-stu-id="debc4-198">Int32</span></span>|<span data-ttu-id="debc4-199">Especifica o valor padrão de volume de uma nova sessão.</span><span class="sxs-lookup"><span data-stu-id="debc4-199">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="debc4-200">Os valores permitidos ficam entre 0 e 100.</span><span class="sxs-lookup"><span data-stu-id="debc4-200">Permitted values are 0-100.</span></span> <span data-ttu-id="debc4-201">O padrão é 45.</span><span class="sxs-lookup"><span data-stu-id="debc4-201">The default is 45.</span></span> <span data-ttu-id="debc4-202">Valores válidos de 0 a 100</span><span class="sxs-lookup"><span data-stu-id="debc4-202">Valid values 0 to 100</span></span>|
|<span data-ttu-id="debc4-203">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="debc4-203">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="debc4-204">Int32</span><span class="sxs-lookup"><span data-stu-id="debc4-204">Int32</span></span>|<span data-ttu-id="debc4-205">Especifica o número de minutos até a tela do Hub ser desligada.</span><span class="sxs-lookup"><span data-stu-id="debc4-205">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="debc4-206">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="debc4-206">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="debc4-207">Int32</span><span class="sxs-lookup"><span data-stu-id="debc4-207">Int32</span></span>|<span data-ttu-id="debc4-208">Especifica o número de minutos até a sessão atingir o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="debc4-208">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="debc4-209">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="debc4-209">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="debc4-210">Int32</span><span class="sxs-lookup"><span data-stu-id="debc4-210">Int32</span></span>|<span data-ttu-id="debc4-211">Especifica o número de minutos até o Hub entrar no modo de suspensão.</span><span class="sxs-lookup"><span data-stu-id="debc4-211">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="debc4-212">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="debc4-212">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="debc4-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="debc4-213">Boolean</span></span>|<span data-ttu-id="debc4-214">Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.</span><span class="sxs-lookup"><span data-stu-id="debc4-214">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="debc4-215">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="debc4-215">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="debc4-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="debc4-216">String</span></span>|<span data-ttu-id="debc4-217">The welcome screen background image URL.</span><span class="sxs-lookup"><span data-stu-id="debc4-217">The welcome screen background image URL.</span></span> <span data-ttu-id="debc4-218">A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.</span><span class="sxs-lookup"><span data-stu-id="debc4-218">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="debc4-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="debc4-219">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="debc4-220">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="debc4-220">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="debc4-221">As informações da reunião mostradas na tela de boas-vindas.</span><span class="sxs-lookup"><span data-stu-id="debc4-221">The welcome screen meeting information shown.</span></span> <span data-ttu-id="debc4-222">Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="debc4-222">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="debc4-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="debc4-223">Response</span></span>
<span data-ttu-id="debc4-224">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="debc4-224">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="debc4-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="debc4-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="debc4-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="debc4-226">Request</span></span>
<span data-ttu-id="debc4-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="debc4-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="debc4-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="debc4-228">Response</span></span>
<span data-ttu-id="debc4-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="debc4-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




