---
title: Atualizar windows10TeamGeneralConfiguration
description: Atualizar as propriedades de um objeto windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2eb7d05269438419e03d8df118fc587af49dc50dccb7f1e237542142255321c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54234054"
---
# <a name="update-windows10teamgeneralconfiguration"></a>Atualizar windows10TeamGeneralConfiguration

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualizar as propriedades de um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|azureOperationalInsightsBlockTelemetry|Boolean|Indica se os Insights Operacionais do Azure devem ou não ser bloqueados.|
|azureOperationalInsightsWorkspaceId|Cadeia de caracteres|A ID do espaço de trabalho dos Insights Operacionais do Azure.|
|azureOperationalInsightsWorkspaceKey|Cadeia de caracteres|A chave do espaço de trabalho dos Insights Operacionais do Azure.|
|connectAppBlockAutoLaunch|Boolean|Especifica se o aplicativo Connect deverá ser iniciado automaticamente sempre que uma projeção for iniciada.|
|maintenanceWindowBlocked|Boolean|Indica se a configuração de uma janela de manutenção para atualizações do dispositivo deverá ou não ser bloqueada.|
|maintenanceWindowDurationInHours|Int32|Duração da janela de manutenção para atualizações do dispositivo. Valores válidos: 0 a 5|
|maintenanceWindowStartTime|TimeOfDay|Hora de Início da janela de manutenção para atualizações do dispositivo.|
|miracastChannel|[miracastChannel](../resources/intune-deviceconfig-miracastchannel.md)|O canal. Os valores possíveis são: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.|
|miracastBlocked|Boolean|Indica se a projeção sem fio deve ou não ser bloqueada.|
|miracastRequirePin|Boolean|Indica se será exigido um pin para a projeção sem fio.|
|settingsBlockMyMeetingsAndFiles|Boolean|Especifica se o recurso "Meus arquivos e reuniões" no menu Iniciar, que mostra as reuniões e arquivos do usuário conectado do Office 365, deverá ser desativado.|
|settingsBlockSessionResume|Boolean|Especifica se a capacidade de retomar uma sessão quando a sessão expirar será permitida.|
|settingsBlockSigninSuggestions|Boolean|Especifica se o preenchimento automático da caixa de diálogo de entrada com os convidados de reuniões agendadas será desativado.|
|settingsDefaultVolume|Int32|Especifica o valor padrão de volume de uma nova sessão. Os valores permitidos ficam entre 0 e 100. O padrão é 45. Valores válidos de 0 a 100|
|settingsScreenTimeoutInMinutes|Int32|Especifica o número de minutos até a tela do Hub ser desligada.|
|settingsSessionTimeoutInMinutes|Int32|Especifica o número de minutos até a sessão atingir o tempo limite.|
|settingsSleepTimeoutInMinutes|Int32|Especifica o número de minutos até o Hub entrar no modo de suspensão.|
|welcomeScreenBlockAutomaticWakeUp|Boolean|Indica se a tela de boas-vindas será impedida de ser desativada automaticamente quando alguém entrar na sala.|
|welcomeScreenBackgroundImageUrl|Cadeia de caracteres|The welcome screen background image URL. A URL deve usar o protocolo HTTPS e retornar uma imagem PNG.|
|welcomeScreenMeetingInformation|[welcomeScreenMeetingInformation](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|As informações da reunião mostradas na tela de boas-vindas. Os valores possíveis são: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
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

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
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




