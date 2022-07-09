---
title: Tipo de recurso accessReviewHistoryDefinition
description: Representa uma coleção de dados de histórico de revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ce078243c0cfdd53f07854c98602c0de615e9288
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698314"
---
# <a name="accessreviewhistorydefinition-resource-type"></a>Tipo de recurso accessReviewHistoryDefinition

Namespace: microsoft.graph

Representa uma coleção de dados históricos de revisão de acesso e os escopos usados para coletar esses dados.

Um **accessReviewHistoryDefinition contém** uma lista [de objetos accessReviewHistoryInstance](accessReviewHistoryInstance.md) . Cada recorrência da definição de histórico cria uma instância. No caso de uma definição de histórico única, apenas uma instância é criada.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessReviewHistoryDefinitions](../api/accessreviewset-list-historydefinitions.md)|[coleção accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Obtenha uma lista dos [objetos accessReviewHistoryDefinition](accessreviewhistorydefinition.md) e suas propriedades.|
|[Criar accessReviewHistoryDefinition](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Crie um novo [objeto accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[Obter accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Leia as propriedades e as relações de um [objeto accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[userIdentity](useridentity.md)| Usuário que criou essa definição de histórico de revisão. |
|createdDateTime|DateTimeOffset|Carimbo de data/hora quando a definição de revisão de acesso foi criada.|
|Decisões|Coleção de cadeias de caracteres|Determina quais decisões de revisão serão incluídas nos dados do histórico de revisão buscados, se especificado. Opcional ao criar. Todas as decisões serão incluídas por padrão se nenhuma decisão for fornecida ao criar. Os valores possíveis são: `approve`, `deny`, `dontKnow`, `notReviewed`e `notNotified`.|
|displayName|Cadeia de caracteres|Nome da coleta de dados do histórico de revisão de acesso. Obrigatório.|
|id|Cadeia de caracteres|O identificador exclusivo atribuído de uma definição de histórico de revisão de acesso.|
|reviewHistoryPeriodEndDateTime|DateTimeOffset| Um carimbo de data/hora. As revisões que terminam em ou antes dessa data serão incluídas nos dados de histórico buscados. Só será necessário se **scheduleSettings** não estiver definido. |
|reviewHistoryPeriodStartDateTime|DateTimeOffset|Um carimbo de data/hora. As revisões que começam em ou antes dessa data serão incluídas nos dados de histórico buscados. Só será necessário se **scheduleSettings** não estiver definido.|
| scheduleSettings  |[accessReviewHistoryScheduleSettings](accessReviewHistoryScheduleSettings.md)| As configurações de uma série de definições de histórico de revisão de acesso recorrente. Obrigatório somente se **reviewHistoryPeriodStartDateTime** ou **reviewHistoryPeriodEndDateTime** não estiver definido. Ainda não há suporte.|
|escopos|[coleção accessReviewScope](accessreviewscope.md)|Usado para definir o escopo de quais revisões estão incluídas nos dados de histórico buscados. Busca revisões cujo escopo corresponde a esse escopo fornecido. Obrigatório.|
|status| accessReviewHistoryStatus|Representa o status da coleta de dados do histórico de revisão. Os valores possíveis são: `done`, `inProgress`, `error`, `requested`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|instances|[coleção accessReviewHistoryInstance](accessreviewhistoryinstance.md)| Se **accessReviewHistoryDefinition** for uma definição recorrente, as instâncias representarão cada recorrência. Uma definição que não se repetir terá exatamente uma instância.|

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
