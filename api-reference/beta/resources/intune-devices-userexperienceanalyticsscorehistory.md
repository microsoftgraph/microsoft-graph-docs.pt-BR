---
title: tipo de recurso userExperienceAnalyticsScoreHistory
description: O histórico de Pontuação de inicialização do dispositivo de análise da experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8706fd6c15033c4db5ac9fb6f923c53d382519a0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706916"
---
# <a name="userexperienceanalyticsscorehistory-resource-type"></a>tipo de recurso userExperienceAnalyticsScoreHistory

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O histórico de Pontuação de inicialização do dispositivo de análise da experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsScoreHistories](../api/intune-devices-userexperienceanalyticsscorehistory-list.md)|coleção [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Listar Propriedades e relações dos objetos [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .|
|[Obter userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-get.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .|
|[Criar userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-create.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Criar um novo objeto [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .|
|[Excluir userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-delete.md)|Nenhum|Exclui [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md).|
|[Atualizar userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-update.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do processo de inicialização do dispositivo de análise da experiência do usuário.|
|startupDateTime|DateTimeOffset|A experiência do usuário da data de início do dispositivo de análise.|
|startupScore|Int32|Pontuação de inicialização do dispositivo de análise da experiência do usuário. A pontuação será no intervalo 0-100, 100 é a pontuação ideal.|
|coreBootScore|Int32|A pontuação de inicialização do dispositivo de análise da experiência do usuário. A pontuação será no intervalo 0-100, 100 é a pontuação ideal.|
|coreSigninScore|Int32|A pontuação de entrada do core do dispositivo de análise da experiência do usuário. A pontuação será no intervalo 0-100, 100 é a pontuação ideal.|
|recommendedSoftwareScore|Int32|A pontuação de entrada do core do dispositivo de análise da experiência do usuário. A pontuação será no intervalo 0-100, 100 é a pontuação ideal.|
|restartScore|Int32|Reinicie o placar. A pontuação será no intervalo 0-100, 100 é a pontuação ideal, 0 indica reinicializações em excesso. Valores válidos de 0 a 9999999|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsScoreHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "String (identifier)",
  "startupDateTime": "String (timestamp)",
  "startupScore": 1024,
  "coreBootScore": 1024,
  "coreSigninScore": 1024,
  "recommendedSoftwareScore": 1024,
  "restartScore": 1024
}
```





