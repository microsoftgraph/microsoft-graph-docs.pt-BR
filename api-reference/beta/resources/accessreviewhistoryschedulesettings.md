---
title: Tipo de recurso accessReviewHistoryScheduleSettings
description: Em avaliações de acesso do Azure AD, accessReviewHistoryScheduleSettings representa as configurações associadas a uma série de definições de histórico de revisão de acesso.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7f1e10372fbd2db23ae70ea413e007993c6f85a0
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62226292"
---
# <a name="accessreviewhistoryschedulesettings-resource-type"></a>Tipo de recurso accessReviewHistoryScheduleSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define as configurações de um [objeto accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| recurrence|[patternedRecurrence](patternedrecurrence.md) | Configurações detalhadas para recorrência usando o objeto Outlook de recorrência padrão. <br/><br/>**Observação:** Somente **as propriedades dayOfMonth**, **interval** e **type** ( , ) `weekly` são `absoluteMonthly` suportadas. Use a propriedade **startDate** em **recurrenceRange** para determinar o dia em que a revisão é iniciada. Obrigatório. |
|reportRange|Cadeia de Caracteres|Uma cadeia de caracteres de duração no formato de duração ISO 8601 especificando o período de retorno dos dados de histórico de revisão gerados. Por exemplo, se uma definição de histórico estiver agendada para ser executado no dia 1º de cada mês, **o reportRange** será `P1M` . Nesse caso, no primeiro de cada mês, os dados do histórico de revisão de acesso serão coletados contendo apenas os dados de revisão do mês anterior. <br/><br/>**Observação:** Há suporte **apenas** **para** propriedades **ISO** 8601 anos , meses e dias. Obrigatório.|

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
