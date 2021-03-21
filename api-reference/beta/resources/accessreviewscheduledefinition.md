---
title: Tipo de recurso accessReviewScheduleDefinition
description: Representa uma série de revisão de acesso ou revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 27b5debdbb9e55eafe55a4c1a7bc66d87b7290cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962662"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>Tipo de recurso accessReviewScheduleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa o agendamento de uma revisão de acesso do Azure [AD.](accessreviewsv2-root.md) 

Um accessReviewScheduleDefinition contém uma lista de [objetos accessReviewInstance.](accessreviewinstance.md) Cada recorrência da definição de agendamento criará uma instância. As instâncias também representam cada grupo exclusivo que está sendo revisado. Se uma definição de agenda analisar vários grupos, cada grupo terá uma instância exclusiva por cada recorrência. No caso de uma revisão única, apenas uma instância será criada por grupo.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [Coleção accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Lista todos os accessReviewScheduleDefinition. Não inclui instâncias de accessReviewInstance associadas em listagem. |
|[Obter accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obter um accessReviewScheduleDefinition com uma id especificada. |
|[Criar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Crie um novo accessReviewScheduleDefinition. |
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Nenhum | Exclua um accessReviewScheduleDefinition com um identificador especificado. |
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Nenhum | Atualizar propriedades de um accessReviewScheduleDefinition com um identificador especificado. |

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :------------------| :-------------- | :---------- |
| id | Cadeia de caracteres | O identificador exclusivo atribuído ao recurso de uma revisão de acesso.|
| displayName | Cadeia de caracteres   | Nome da série de revisão de acesso. Obrigatório durante a criação. |
| createdDateTime  |DateTimeOffset  | Timestamp quando a série de revisão foi criada. |
| lastModifiedDateTime | DateTimeOffset   | Timestamp quando a série de revisão foi modificada pela última vez.|
| status  |Cadeia de caracteres   | Este campo somente leitura especifica o status de um accessReview. Os estados típicos `Initializing` `NotStarted` incluem , `Starting` , , , , , e `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . |
| descriptionForAdmins  |cadeia de caracteres  |  Descrição fornecida pelos criadores de revisão para fornecer mais contexto da revisão aos administradores. |
| descriptionForReviewers |cadeia de caracteres | Descrição fornecida pelos criadores de revisão para fornecer mais contexto da revisão aos revisadores. Os revisadores verão essa descrição no email enviado a eles solicitando sua revisão. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Usuário que criou essa revisão. |
| escopo  |[accessReviewScope](../resources/accessreviewscope.md)  | Define o escopo dos usuários revisados. Para escopos com suporte, consulte [accessReviewScope](accessreviewscope.md). Obrigatório durante a criação. |
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | No caso de uma revisão de usuários convidados em todos os grupos do Microsoft 365, isso determina o escopo de quais grupos serão revisados. Cada grupo se tornará um accessReviewInstance exclusivo da série de revisão de acesso.  Para escopos com suporte, consulte [accessReviewScope](accessreviewscope.md). | 
| configurações  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| As configurações de uma série de revisão de acesso, consulte a definição de tipo abaixo. |
| revisadores   |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisão de acesso é usada para definir quem são os revistores. Consulte [accessReviewReviewerScope](accessreviewreviewerscope.md). Obrigatório durante a criação. |
| backupReviewers   |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos do revistor é usada para definir a lista de revisadores de fallback. Esses revisadores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisadores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como o revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe. Consulte [accessReviewReviewerScope](accessreviewreviewerscope.md). |
| instances |Collection(microsoft.graph.accessReviewInstance)|  Conjunto de instâncias de críticas de acesso para esta série de revisão de acesso. As avaliações do Access que não se recorrem terão apenas uma instância; caso contrário, haverá uma instância para cada recorrência. |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `instances`               |[Coleção accessReviewInstance](accessreviewinstance.md)         | Se for `accessReviewScheduleDefinition` uma revisão de acesso recorrente, as instâncias representarão cada recorrência. Uma revisão que não se recorre terá exatamente uma instância. As instâncias também representam cada recurso exclusivo sob revisão no `accessReviewScheduleDefinition` . Se uma revisão tiver vários recursos e várias instâncias, cada recurso terá uma instância exclusiva para cada recorrência. |

### <a name="supported-queries-for-accessreviewscheduledefinition"></a>Consultas com suporte para accessReviewScheduleDefinition
A seguir, há consultas com suporte em [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md) com base no [accessReviewScope](accessreviewscope.md).

|Cenário| Consulta |
|--|--|
| Listar `accessReviewScheduleDefinition` todos os grupos individuais (exclui definições com escopo para todos os grupos do Microsoft 365 com usuários convidados) | /beta/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups') |
| Listar todos em um grupo específico (exclui definições com escopo para todos os grupos do `accessReviewScheduleDefinition` Microsoft 365 com usuários convidados) | /beta/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups/{group id}') |
| Listar `accessReviewScheduleDefinition` todos os grupos do Microsoft 365 com usuários convidados | /beta/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, './members') |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "descriptionForAdmins": "String",
  "descriptionForReviewers": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "instanceEnumerationScope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  },
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
  }
}
```
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
