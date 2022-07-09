---
title: Tipo de recurso accessReviewHistoryScheduleSettings
description: Nas Azure AD de acesso, accessReviewHistoryScheduleSettings representa as configurações associadas a uma série de definições de histórico de revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 70483c049a555bf2315a8f0cb49bd652893bef91
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696515"
---
# <a name="accessreviewhistoryschedulesettings-resource-type"></a>Tipo de recurso accessReviewHistoryScheduleSettings

Namespace: microsoft.graph

Define as configurações de um [objeto accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| recurrence|[patternedRecurrence](patternedrecurrence.md) | Configurações detalhadas para recorrência usando o objeto de recorrência padrão do Outlook. <br/><br/>**Nota:** Somente **as propriedades dayOfMonth**, **interval** e **type** (`weekly`, `absoluteMonthly`) têm suporte. Use a propriedade **startDate** **em recurrenceRange** para determinar o dia em que a revisão é iniciada. Obrigatório. |
|reportRange|Cadeia de Caracteres|Uma cadeia de caracteres de duração no formato de duração ISO 8601 que especifica o período de retorno dos dados de histórico de revisão gerados. Por exemplo, se uma definição de histórico estiver agendada para ser executada no dia 1º de cada mês, **o reportRange** será `P1M`. Nesse caso, no primeiro de cada mês, os dados do histórico de revisão de acesso serão coletados contendo apenas os dados de revisão do mês anterior. <br/><br/>**Nota:** Há **suporte** apenas **para propriedades** **ISO** 8601 de anos, meses e dias. Obrigatório.|

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
