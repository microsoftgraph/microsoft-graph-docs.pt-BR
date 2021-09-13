---
title: Tipo de recurso userExperienceAnalyticsScoreHistory
description: Histórico de pontuação de inicialização do dispositivo de análise de experiência do usuário.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 66f895b27cbc1314957a3bc24d67e1d13214f7aa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046971"
---
# <a name="userexperienceanalyticsscorehistory-resource-type"></a>Tipo de recurso userExperienceAnalyticsScoreHistory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Histórico de pontuação de inicialização do dispositivo de análise de experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsScoreHistories](../api/intune-devices-userexperienceanalyticsscorehistory-list.md)|[coleção userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Listar propriedades e relações dos [objetos userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|
|[Obter userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-get.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Leia propriedades e relações do [objeto userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|
|[Criar userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-create.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Crie um novo [objeto userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|
|[Excluir userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-delete.md)|Nenhum|Exclui um [userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md).|
|[Atualizar userExperienceAnalyticsScoreHistory](../api/intune-devices-userexperienceanalyticsscorehistory-update.md)|[userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|Atualize as propriedades de [um objeto userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do processo de inicialização do dispositivo de análise de experiência do usuário.|
|startupDateTime|DateTimeOffset|A data de inicialização do dispositivo de análise de experiência do usuário.|
|overallScore|Int32|Pontuação geral da análise de experiência do usuário. A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal. Valores válidos de 0 a 100|
|startupScore|Int32|Pontuação de inicialização do dispositivo de análise de experiência do usuário. A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.|
|coreBootScore|Int32|A pontuação de inicialização principal do dispositivo de análise de experiência do usuário. A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.|
|coreSigninScore|Int32|A pontuação de entrada principal do dispositivo de análise de experiência do usuário. A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.|
|recommendedSoftwareScore|Int32|A pontuação de entrada principal do dispositivo de análise de experiência do usuário. A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.|
|appHealthOverallScore|Int32|A pontuação geral de saúde geral do aplicativo de análise de experiência do usuário.|
|startupTotalDevices|Int32|A contagem total de dispositivos do desempenho de inicialização da categoria de análise de experiência do usuário.|
|recommendedSoftwareTotalDevices|Int32|A contagem total de dispositivos do software recomendado da categoria de análise de experiência do usuário.|
|appHealthTotalDevices|Int32|A contagem total de dispositivos da saúde do aplicativo de categoria de análise de experiência do usuário.|
|restartScore|Int32|Reinicie a pontuação. A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal, 0 indica reinicializações excessivas. Valores válidos de 0 a 9999999|

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
  "overallScore": 1024,
  "startupScore": 1024,
  "coreBootScore": 1024,
  "coreSigninScore": 1024,
  "recommendedSoftwareScore": 1024,
  "appHealthOverallScore": 1024,
  "startupTotalDevices": 1024,
  "recommendedSoftwareTotalDevices": 1024,
  "appHealthTotalDevices": 1024,
  "restartScore": 1024
}
```



