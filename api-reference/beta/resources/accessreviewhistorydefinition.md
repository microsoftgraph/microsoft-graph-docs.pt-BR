---
title: Tipo de recurso accessReviewHistoryDefinition
description: Representa uma coleção de dados de histórico de revisão de acesso.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b36062da1387e50f4ffbae88a8e7cae1fa31f268
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225550"
---
# <a name="accessreviewhistorydefinition-resource-type"></a>Tipo de recurso accessReviewHistoryDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção de dados históricos de revisão de acesso e os escopos usados para coletar esses dados.

Um **accessReviewHistoryDefinition** contém uma lista de [objetos accessReviewHistoryInstance.](accessReviewHistoryInstance.md) Cada recorrência da definição de histórico cria uma instância. No caso de uma definição de histórico única, apenas uma instância é criada.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessReviewHistoryDefinitions](../api/accessreviewset-list-historydefinitions.md)|[Coleção accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Obter uma lista dos [objetos accessReviewHistoryDefinition](accessreviewhistorydefinition.md) e suas propriedades.|
|[Criar accessReviewHistoryDefinition](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Crie um novo [objeto accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)|
|[Obter accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Leia as propriedades e as relações de [um objeto accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[userIdentity](useridentity.md)| Usuário que criou essa definição de histórico de revisão. |
|createdDateTime|DateTimeOffset|Timestamp quando a definição de revisão de acesso foi criada.|
|decisions|Conjunto de cadeias de caracteres|Determina quais decisões de revisão serão incluídas nos dados de histórico de revisão buscados, se especificado. Opcional ao criar. Todas as decisões serão incluídas por padrão se nenhuma decisão for fornecida na criação. Os valores possíveis são: `approve` , , , e `deny` `dontKnow` `notReviewed` `notNotified` .|
|displayName|Cadeia de caracteres|Nome da coleção de dados do histórico de revisão de acesso. Obrigatório.|
|id|Cadeia de caracteres|O identificador exclusivo atribuído de uma definição de histórico de revisão de acesso.|
|reviewHistoryPeriodEndDateTime|DateTimeOffset| Um timestamp. As avaliações que terminam antes ou antes dessa data serão incluídas nos dados de histórico buscados. Somente será necessário se **scheduleSettings** não for definido. |
|reviewHistoryPeriodStartDateTime|DateTimeOffset|Um timestamp. As avaliações que começam em ou antes dessa data serão incluídas nos dados de histórico buscados. Somente será necessário se **scheduleSettings** não for definido.|
| scheduleSettings  |[accessReviewHistoryScheduleSettings](accessReviewHistoryScheduleSettings.md)| As configurações de uma série de definição de histórico de revisão de acesso recorrente. Somente será necessário se **reviewHistoryPeriodStartDateTime** ou **reviewHistoryPeriodEndDateTime** não estiver definido.|
|escopos|[Coleção accessReviewScope](accessreviewscope.md)|Usado para analisar quais avaliações são incluídas nos dados de histórico buscados. Busca avaliações cujo escopo corresponde a esse escopo fornecido. Obrigatório.|
|status|Conjunto de cadeias de caracteres|Representa o status da coleção de dados do histórico de revisão. Os valores possíveis são: `done`, `inProgress`, `error`, `requested`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|instances|[Coleção accessReviewHistoryInstance](accessreviewhistoryinstance.md)| Se **accessReviewHistoryDefinition** for uma definição recorrente, as instâncias representarão cada recorrência. Uma definição que não se recorre terá exatamente uma instância.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "reviewHistoryPeriodStartDateTime": "String (timestamp)",
  "reviewHistoryPeriodEndDateTime": "String (timestamp)",
  "status": "String",
  "decisions": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "scopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "scheduleSettings": {
    "@odata.type": "microsoft.graph.accessReviewHistoryScheduleSettings"
  }
}
```
