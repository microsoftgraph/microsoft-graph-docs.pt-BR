---
title: Tipo de recurso accessReviewHistoryScheduleSettings
description: Em avaliações de acesso do Azure AD, accessReviewHistoryScheduleSettings representa as configurações associadas a uma série de definições de histórico de revisão de acesso.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 32c8eff3229b0597a5dc05cfeffa66fe8ed2d851
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337608"
---
# <a name="accessreviewhistoryschedulesettings-resource-type"></a>Tipo de recurso accessReviewHistoryScheduleSettings

Namespace: microsoft.graph

Define as configurações de um [objeto accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| recurrence|[patternedRecurrence](patternedrecurrence.md) | Configurações detalhadas para recorrência usando o objeto Outlook de recorrência padrão. <br/><br/>**Observação:** Somente **as propriedades dayOfMonth**, **interval** e **type** (`weekly`, `absoluteMonthly`) são suportadas. Use a propriedade **startDate** em **recurrenceRange** para determinar o dia em que a revisão é iniciada. Obrigatório. |
|reportRange|String|Uma cadeia de caracteres de duração no formato de duração ISO 8601 especificando o período de retorno dos dados de histórico de revisão gerados. Por exemplo, se uma definição de histórico estiver agendada para ser executado no dia 1º de cada mês, **o reportRange** será `P1M`. Nesse caso, no primeiro de cada mês, os dados do histórico de revisão de acesso serão coletados contendo apenas os dados de revisão do mês anterior. <br/><br/>**Observação:** Há **suporte** apenas para **propriedades** **ISO** 8601 de anos, meses e dias. Obrigatório.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewHistoryScheduleSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryScheduleSettings",
  "reportRange": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  }
}
```
