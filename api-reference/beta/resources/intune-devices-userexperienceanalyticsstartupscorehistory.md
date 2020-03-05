---
title: tipo de recurso userExperienceAnalyticsStartupScoreHistory
description: O histórico de Pontuação de inicialização do dispositivo de análise da experiência do usuário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ccf5de7e4a9b877b1466f632ba2e1821aaed6161
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528428"
---
# <a name="userexperienceanalyticsstartupscorehistory-resource-type"></a>tipo de recurso userExperienceAnalyticsStartupScoreHistory

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O histórico de Pontuação de inicialização do dispositivo de análise da experiência do usuário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar userExperienceAnalyticsStartupScoreHistories](../api/intune-devices-userexperienceanalyticsstartupscorehistory-list.md)|coleção [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)|Listar Propriedades e relações dos objetos [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .|
|[Obter userExperienceAnalyticsStartupScoreHistory](../api/intune-devices-userexperienceanalyticsstartupscorehistory-get.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)|Leia as propriedades e as relações do objeto [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .|
|[Criar userExperienceAnalyticsStartupScoreHistory](../api/intune-devices-userexperienceanalyticsstartupscorehistory-create.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)|Criar um novo objeto [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .|
|[Excluir userExperienceAnalyticsStartupScoreHistory](../api/intune-devices-userexperienceanalyticsstartupscorehistory-delete.md)|Nenhum|Exclui [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md).|
|[Atualizar userExperienceAnalyticsStartupScoreHistory](../api/intune-devices-userexperienceanalyticsstartupscorehistory-update.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md)|Atualiza as propriedades de um objeto [userExperienceAnalyticsStartupScoreHistory](../resources/intune-devices-userexperienceanalyticsstartupscorehistory.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do processo de inicialização do dispositivo de análise da experiência do usuário.|
|startupDateTime|DateTimeOffset|A experiência do usuário da data de início do dispositivo de análise.|
|startupScore|Int32|Pontuação de inicialização do dispositivo de análise da experiência do usuário.|
|coreBootScore|Int32|A pontuação de inicialização do dispositivo de análise da experiência do usuário.|
|coreSigninScore|Int32|A pontuação de entrada do core do dispositivo de análise da experiência do usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsStartupScoreHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "id": "String (identifier)",
  "startupDateTime": "String (timestamp)",
  "startupScore": 1024,
  "coreBootScore": 1024,
  "coreSigninScore": 1024
}
```



