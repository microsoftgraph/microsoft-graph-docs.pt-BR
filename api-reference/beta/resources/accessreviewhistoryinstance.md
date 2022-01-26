---
title: Tipo de recurso accessReviewHistoryInstance
description: Representa uma recorrência de um objeto accessReviewHistoryDefinition.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0dc828d16566f11690603f5cea7b2154037cd1e6
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62226058"
---
# <a name="accessreviewhistoryinstance-resource-type"></a>Tipo de recurso accessReviewHistoryInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 Representa uma recorrência de um [objeto accessReviewHistoryDefinition.](accessreviewhistorydefinition.md) Uma definição de histórico que não se recorre terá exatamente uma instância.

 Cada **accessReviewHistoryInstance** juntamente com seu **accessReviewHistoryDefinition** associado contém as propriedades **reviewHistoryPeriodStartDateTime**, **reviewHistoryPeriodEndDateTime**, **decisions**, **scheduleSettings** e **scopes**. Essas propriedades são usadas ao agendar recorrências, bem como selecionar dados de revisão e podem ser modificadas. Cada **objeto accessReviewHistoryInstance** e os dados estão disponíveis apenas por 30 dias. Depois que **um status accessReviewHistoryInstance** é movido para um link pode ser gerado para recuperar os dados da instância chamando `done` [generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md).

## <a name="methods"></a>Métodos

| Método  | Tipo de retorno | Descrição |
|:---|:---|:---|
|[Listar accessReviewHistoryInstances](../api/accessreviewhistorydefinition-list-instances.md)|[Coleção accessReviewHistoryInstance](accessreviewhistoryinstance.md)| Recupere uma lista dos [objetos accessReviewHistoryInstance](accessreviewhistoryinstance.md) e suas propriedades.|
|[generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Gera um URI que pode ser usado para recuperar os dados de histórico de revisão da instância.|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|downloadUri|Cadeia de Caracteres|Uri que pode ser usado para recuperar dados de histórico de revisão. Esse URI ficará ativo por 24 horas após ser gerado. Obrigatório.|
|expirationDateTime|DateTimeOffset|Timestamp quando essa instância e dados associados expiram e o histórico é excluído. Obrigatório.|
|fulfilledDateTime|DateTimeOffset|Timestamp quando todos os dados disponíveis para esta instância foram coletados. Isso será definido depois que o status dessa instância for definido como `done` . Obrigatório.|
|id|Cadeia de caracteres|O identificador exclusivo atribuído de uma instância de histórico de revisão de acesso. Somente leitura. Obrigatório.|
|reviewHistoryPeriodEndDateTime|DateTimeOffset|Timestamp, as avaliações terminadas em ou antes dessa data serão incluídas nos dados de histórico buscados.|
|reviewHistoryPeriodStartDateTime|DateTimeOffset|Timestamp, as avaliações que começam em ou após essa data serão incluídas nos dados de histórico buscados.|
|runDateTime|DateTimeOffset|Timestamp quando os dados de histórico da instância estão agendados para serem gerados.|
|status|Conjunto de cadeias de caracteres|Representa o status da coleção de dados do histórico de revisão. Os valores possíveis são: `done`, `inProgress`, `error`, `requested`, `unknownFutureValue`. Depois que **o status** tiver sido marcado como , um link pode ser gerado para recuperar os dados da instância chamando o `done` método [generateDownloadUri.](../api/accessreviewhistoryinstance-generatedownloaduri.md)|

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
