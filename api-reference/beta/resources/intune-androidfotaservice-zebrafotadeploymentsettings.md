---
title: Tipo de recurso zebraFotaDeploymentSettings
description: O tipo complexo de implantação do Zebra FOTA que descreve as configurações necessárias para criar uma implantação de FOTA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b055ae91e93919a3f6b8af63d7ae7a207ffaaac
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213069"
---
# <a name="zebrafotadeploymentsettings-resource-type"></a>Tipo de recurso zebraFotaDeploymentSettings

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O tipo complexo de implantação do Zebra FOTA que descreve as configurações necessárias para criar uma implantação de FOTA.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|deviceModel|Cadeia de caracteres|Implante a atualização somente para dispositivos com esse modelo.|
|updateType|[zebraFotaUpdateType](../resources/intune-androidfotaservice-zebrafotaupdatetype.md)|O tipo de atualização da implantação. Os valores possíveis são personalizados, mais recentes e automáticos. Quando o modo personalizado é definido, a solicitação deve fornecer valores de artefato. Quando o tipo mais recente for definido, a atualização mais recente lançada se tornará o sistema operacional de destino. Se a versão mais recente for especificada, os valores de destino do firmware não serão necessários. Observação: a versão mais recente pode atualizar o dispositivo para uma nova versão do Android. Quando o valor é definido como automático, o dispositivo sempre procura o pacote mais recente disponível e tenta atualizar sempre que um novo pacote está disponível. Isso continuará até que o administrador cancele a atualização automática. Enquanto outros modos retornam uma ID começando com FOTA-x, o modo automático retorna uma ID começando com AUTO-x. Os valores possíveis são: `custom`, `latest`, `auto`, `unknownFutureValue`.|
|timeZoneOffsetInMinutes|Int32|Esse atributo indica o deslocamento de tempo de implantação (por exemplo,`180` representa um deslocamento de `+03:00`, e `-270` representa um deslocamento de `-04:30`). O deslocamento de tempo é o fuso horário em que os dispositivos estão localizados. Os dados de início e término da implantação usam esse fuso horário|
|firmwareTargetBoardSupportPackageVersion|Cadeia de Caracteres|BSP (Pacote de Suporte de Placa) da implantação. Por exemplo: '01.18.02.00'). Necessário apenas para o tipo de atualização personalizado.|
|firmwareTargetPatch|Cadeia de Caracteres|Nome do patch de destino (por exemplo: 'U06'). Necessário apenas para o tipo de atualização personalizado.|
|firmwareTargetOsVersion|Cadeia de Caracteres|Versão do sistema operacional de destino (por exemplo: '8.1.0'). Necessário apenas para o tipo de atualização personalizado.|
|scheduleMode|[zebraFotaScheduleMode](../resources/intune-androidfotaservice-zebrafotaschedulemode.md)|Modo de agendamento de instalação de implantação. O padrão é installNow. Todas as datas e horas de implantações agendadas estão no fuso horário do dispositivo. Para Instalar Agora, a data e a hora estão em UTC (mesma data e hora em qualquer lugar do mundo). Os valores possíveis são: `installNow`, `scheduled`, `unknownFutureValue`.|
|scheduleDurationInDays|Int32|Máximo de 28 dias. O padrão é 28 dias. A sequência de datas é: 1) Data de início do download. 2) Data de início da instalação. 3) Agendar data de término. Se algum dos valores não for fornecido, a data fornecida na etapa anterior da sequência será usada. Se nenhum valor for fornecido, o valor da cadeia de caracteres do UTC atual será usado.|
|downloadRuleNetworkType|[zebraFotaNetworkType](../resources/intune-androidfotaservice-zebrafotanetworktype.md)|Baixe o tipo de rede conforme descrito em 'zebraFotaNetworkType'. Padrão: any. Os valores possíveis são: `any`, `wifi`, `cellular`, `wifiAndCellular`, `unknownFutureValue`.|
|downloadRuleStartDateTime|DateTimeOffset|Data e hora no fuso horário do dispositivo quando o download será iniciado (por exemplo, `2018-07-25T10:20:32`). O valor padrão agora é UTC e o máximo é de 10 dias após a criação da implantação.|
|installRuleStartDateTime|DateTimeOffset|Data e hora no fuso horário do dispositivo quando a instalação será iniciada. Padrão – baixe startDate se configurado; caso contrário, o padrão é NOW. Ignorado quando o tipo de atualização de implantação foi definido como automático.|
|installRuleWindowStartTime|TimeOfDay|Hora do dia (00:00:00 – 23:30:00) quando a instalação deve começar. A hora é expressa em um formato de 24 horas, como hh:mm, e está no fuso horário do dispositivo. Padrão – 00:00:00. Respeitado por todos os valores de tipo de atualização, incluindo AUTO.|
|installRuleWindowEndTime|TimeOfDay|Hora do dia após a qual a instalação não pode ser iniciada. O intervalo possível é de 00:30:00 a 23:59:59. Deve ser maior que 'installRuleWindowStartTime' em 30 minutos. A hora é expressa em um formato de 24 horas, como hh:mm, e está no fuso horário do dispositivo. Padrão – 23:59:59. Respeitado por todos os valores de tipo de atualização, incluindo AUTO.|
|batteryRuleMinimumBatteryLevelPercentage|Int32|Nível mínimo de bateria (%) necessário para download e instalação. Padrão: -1 (Padrões do sistema). O máximo é 100.|
|batteryRuleRequireCharger|Booliano|Sinalizador indicando se o carregador é necessário. Quando definido como false, o cliente pode instalar atualizações se o dispositivo estiver dentro ou fora do carregador. Aplicado somente para instalação. O padão é falso.|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.zebraFotaDeploymentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaDeploymentSettings",
  "deviceModel": "String",
  "updateType": "String",
  "timeZoneOffsetInMinutes": 1024,
  "firmwareTargetBoardSupportPackageVersion": "String",
  "firmwareTargetPatch": "String",
  "firmwareTargetOsVersion": "String",
  "scheduleMode": "String",
  "scheduleDurationInDays": 1024,
  "downloadRuleNetworkType": "String",
  "downloadRuleStartDateTime": "String (timestamp)",
  "installRuleStartDateTime": "String (timestamp)",
  "installRuleWindowStartTime": "String (time of day)",
  "installRuleWindowEndTime": "String (time of day)",
  "batteryRuleMinimumBatteryLevelPercentage": 1024,
  "batteryRuleRequireCharger": true
}
```




