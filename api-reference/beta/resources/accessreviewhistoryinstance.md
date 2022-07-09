---
title: Tipo de recurso accessReviewHistoryInstance
description: Representa uma recorrência de um objeto accessReviewHistoryDefinition.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c6b1d137c470bdf384bc60d2a20834860f7dbd01
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697908"
---
# <a name="accessreviewhistoryinstance-resource-type"></a>Tipo de recurso accessReviewHistoryInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 Representa uma recorrência de um [objeto accessReviewHistoryDefinition](accessreviewhistorydefinition.md) . Uma definição de histórico que não se repetir terá exatamente uma instância.

 Cada **accessReviewHistoryInstance** juntamente com seu **accessReviewHistoryDefinition** associado contêm as propriedades **reviewHistoryPeriodStartDateTime**, **reviewHistoryPeriodEndDateTime**, **decisions**, **scheduleSettings** e **escopos**. Essas propriedades são usadas ao agendar recorrências, bem como selecionar dados de revisão e podem ser modificadas. Cada **objeto e dados accessReviewHistoryInstance** só estão disponíveis por 30 dias. Depois que um status `done` **accessReviewHistoryInstance** for movido para um link, poderá ser gerado para recuperar os dados da instância chamando [generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md).

## <a name="methods"></a>Métodos

| Método  | Tipo de retorno | Descrição |
|:---|:---|:---|
|[Listar accessReviewHistoryInstances](../api/accessreviewhistorydefinition-list-instances.md)|[coleção accessReviewHistoryInstance](accessreviewhistoryinstance.md)| Recupere uma lista dos [objetos accessReviewHistoryInstance](accessreviewhistoryinstance.md) e suas propriedades.|
|[generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Gera um URI que pode ser usado para recuperar os dados do histórico de revisão da instância.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|downloadUri|Cadeia de Caracteres|URI que pode ser usado para recuperar dados de histórico de revisão. Esse URI ficará ativo por 24 horas após ser gerado. Obrigatório.|
|expirationDateTime|DateTimeOffset|Carimbo de data/hora quando essa instância e os dados associados expiram e o histórico é excluído. Obrigatório.|
|fulfilledDateTime|DateTimeOffset|Carimbo de data/hora quando todos os dados disponíveis para essa instância foram coletados. Isso será definido depois que o status dessa instância for definido como `done`. Obrigatório.|
|id|Cadeia de caracteres|O identificador exclusivo atribuído de uma instância de histórico de revisão de acesso. Somente leitura. Obrigatório.|
|reviewHistoryPeriodEndDateTime|DateTimeOffset|Carimbo de data/hora, as revisões que terminam em ou antes dessa data serão incluídas nos dados de histórico buscados.|
|reviewHistoryPeriodStartDateTime|DateTimeOffset|Carimbo de data/hora, as revisões que começam em ou após essa data serão incluídas nos dados de histórico buscados.|
|runDateTime|DateTimeOffset|Carimbo de data/hora quando os dados de histórico da instância estão agendados para serem gerados.|
|status|accessReviewHistoryStatus|Representa o status da coleta de dados do histórico de revisão. Os valores possíveis são: `done`, `inProgress`, `error`, `requested`, `unknownFutureValue`. Depois que **o status** tiver sido marcado como `done`, um link poderá ser gerado para recuperar os dados da instância chamando o [método generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md) .|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewHistoryInstance",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.accessReviewHistoryInstance",
  "id": "String (identifier)",
  "reviewHistoryPeriodStartDateTime": "String (timestamp)",
  "reviewHistoryPeriodEndDateTime": "String (timestamp)",
  "status": "String",
  "runDateTime": "String (timestamp)",
  "fulfilledDateTime": "String (timestamp)",
  "downloadUri": "String",
  "expirationDateTime": "String (timestamp)"
}
```
