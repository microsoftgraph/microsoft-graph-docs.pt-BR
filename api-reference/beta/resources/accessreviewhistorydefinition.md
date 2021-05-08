---
title: Tipos de recursos accessReviewHistoryDefinition
description: Representa uma coleção de dados de histórico de revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 96619cb95c11a77106c86cbdcc720f1a486721c7
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232898"
---
# <a name="accessreviewhistorydefinition-resource-type"></a>Tipo de recurso accessReviewHistoryDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção de dados de histórico de revisão de acesso e os escopos usados para coletar esses dados. As **propriedades reviewHistoryPeriodStartDateTime**, **reviewHistoryPeriodEndDateTime**, **decisions** e scopes de **um accessReviewHistoryDefinition** são usadas ao selecionar dados de histórico de revisão e podem ser **modificadas.** Cada **objeto accessReviewHistoryDefinition** está disponível apenas por 30 dias. Depois que o status de uma definição de histórico é movido para um link pode ser gerado para recuperar os dados da definição chamando `done` [generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessReviewHistoryDefinitions](../api/accessreviewhistorydefinition-list.md)|[Coleção accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Obter uma lista dos [objetos accessReviewHistoryDefinition](accessreviewhistorydefinition.md) e suas propriedades.|
|[Criar accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-post.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Crie um novo [objeto accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)|
|[Obter accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Leia as propriedades e as relações de [um objeto accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)|
|[generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Gere um URI que pode ser usado para recuperar dados de histórico de revisão.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|[userIdentity](useridentity.md)| Usuário que criou essa definição de histórico de revisão. |
|createdDateTime|DateTimeOffset|Timestamp quando a definição de revisão de acesso foi criada.|
|decisions|Coleção de cadeias de caracteres|Determina quais decisões de revisão serão incluídas nos dados de histórico de revisão buscados, se especificado. Opcional ao criar. Todas as decisões serão incluídas por padrão se nenhuma decisão for fornecida na criação. Os valores possíveis são: `approve` , , , e `deny` `dontKnow` `notReviewed` `notNotified` .|
|displayName|String|Nome da coleção de dados do histórico de revisão de acesso. Obrigatório.|
|downloadUri|String|Uri que pode ser usado para recuperar dados de histórico de revisão. Esse URI ficará ativo por 24 horas após ser gerado.|
|fulfilledDateTime|DateTimeOffset|Timestamp quando todos os dados disponíveis para essa definição foram coletados. Isso será definido depois que o status dessa definição for definido como `done` .|
|id|String|O identificador exclusivo atribuído de uma definição de histórico de revisão de acesso.|
|reviewHistoryPeriodEndDateTime|DateTimeOffset|Timestamp, as avaliações que começam em ou após essa data serão incluídas nos dados de histórico buscados. Obrigatório.|
|reviewHistoryPeriodStartDateTime|DateTimeOffset|Timestamp, as avaliações que começam em ou antes dessa data serão incluídas nos dados de histórico buscados. Obrigatório.|
|escopos|coleção microsoft.graph.accessReviewQueryScope|Usado para analisar quais avaliações são incluídas nos dados de histórico buscados. Busca avaliações cujo escopo corresponde a esse escopo fornecido. Consulte [accessreviewqueryscope](accessreviewqueryscope.md). Obrigatório.|
|status|Coleção de cadeias de caracteres|Representa o status da coleção de dados do histórico de revisão. Os valores possíveis são: `done`, `inprogress`, `error`, `requested`.|

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
  "decisions": [
    {
      "@odata.type": "String"
    }
  ],
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "fulfilledDateTime": "String (timestamp)",
  "downloadUri": "String",
  "createdBy": {
    "@odata.type": "#microsoft.graph.userIdentity"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    }
  ]
}
```
