---
title: Tipo de recurso userExperienceAnalyticsDeviceStartupHistory
description: A entidade histórico de inicialização do dispositivo de análise de experiência do usuário contém detalhes do histórico de desempenho de inicialização do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8ffc994a7f6be02a361ea21422bfefccf31352aa
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797244"
---
# <a name="userexperienceanalyticsdevicestartuphistory-resource-type"></a>Tipo de recurso userExperienceAnalyticsDeviceStartupHistory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade histórico de inicialização do dispositivo de análise de experiência do usuário contém detalhes do histórico de desempenho de inicialização do dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsDeviceStartupHistories](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-list.md)|[coleção userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|
|[Obter userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-get.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|
|[Criar userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-create.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Crie um novo [objeto userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|
|[Excluir userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-delete.md)|Nenhum(a)|Exclui um [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).|
|[Atualizar userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-update.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsDeviceStartupHistory.](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do histórico de inicialização do dispositivo de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|A ID do dispositivo de análise de experiência do usuário.|
|startTime|DateTimeOffset|A hora de inicialização do dispositivo de análise de experiência do usuário.|
|coreBootTimeInMs|Int32|O tempo de inicialização principal do dispositivo de análise de experiência do usuário em milissegundos.|
|groupPolicyBootTimeInMs|Int32|Análise de experiência do usuário Tempo de inicialização da política de grupo do dispositivo em milissegundos.|
|featureUpdateBootTimeInMs|Int32|O tempo de atualização de recursos do dispositivo de análise de experiência do usuário em milissegundos.|
|totalBootTimeInMs|Int32|O tempo total de inicialização do dispositivo de análise de experiência do usuário em milissegundos.|
|groupPolicyLoginTimeInMs|Int32|Análise de experiência do usuário Tempo de logon da política de grupo do dispositivo em milissegundos.|
|coreLoginTimeInMs|Int32|O tempo de logon principal do dispositivo de análise de experiência do usuário em milissegundos.|
|responsiveDesktopTimeInMs|Int32|A análise da experiência do usuário responde ao tempo da área de trabalho em milissegundos.|
|totalLoginTimeInMs|Int32|O tempo total de logon do dispositivo de análise de experiência do usuário em milissegundos.|
|isFirstLogin|Boleano|O primeiro logon do dispositivo de análise de experiência do usuário.|
|isFeatureUpdate|Boleano|O registro de inicialização do dispositivo de análise de experiência do usuário é uma atualização de recurso.|
|operatingSystemVersion|String|A versão do sistema operacional do registro de inicialização do dispositivo de análise de experiência do usuário.|
|restartCategory|[userExperienceAnalyticsOperatingSystemRestartCategory](../resources/intune-devices-userexperienceanalyticsoperatingsystemrestartcategory.md)|Categoria de reinicialização do sistema operacional. Os valores possíveis são: `unknown`, `restartWithUpdate`, `restartWithoutUpdate`, `blueScreen`, `shutdownWithUpdate`, `shutdownWithoutUpdate`, `longPowerButtonPress`, `bootError`, `update`.|
|restartStopCode|Cadeia de caracteres|Código de parada de reinicialização do sistema operacional. Isso mostra o código de verificação de bugs que pode ser usado para procurar o motivo da tela azul.|
|restartFaultBucket|Cadeia de caracteres|Bucket de falha de reinicialização do sistema operacional. O bucket de falhas é usado para encontrar informações adicionais sobre uma falha no sistema.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "String (identifier)",
  "deviceId": "String",
  "startTime": "String (timestamp)",
  "coreBootTimeInMs": 1024,
  "groupPolicyBootTimeInMs": 1024,
  "featureUpdateBootTimeInMs": 1024,
  "totalBootTimeInMs": 1024,
  "groupPolicyLoginTimeInMs": 1024,
  "coreLoginTimeInMs": 1024,
  "responsiveDesktopTimeInMs": 1024,
  "totalLoginTimeInMs": 1024,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "String",
  "restartCategory": "String",
  "restartStopCode": "String",
  "restartFaultBucket": "String"
}
```



