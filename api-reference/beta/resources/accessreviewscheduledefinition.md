---
title: tipo de recurso accessReviewScheduleDefinition
description: Representa uma série de revisão ou de revisão do Access.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f8ee04dde7ee19d24be5de58237f08b4fb538e8c
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000766"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>tipo de recurso accessReviewScheduleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o agendamento de uma revisão do Azure AD [Access](accessreviewsv2-root.md). 

Um accessReviewScheduleDefinition contém uma lista de objetos [accessReviewInstance](accessreviewinstance.md) . Cada recorrência da definição de agendamento criará uma instância. As instâncias também representam cada grupo exclusivo que está sendo revisado. Se uma definição de programação revisa vários grupos, cada grupo terá uma instância exclusiva por cada recorrência. No caso de uma revisão única, somente uma instância será criada por grupo.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | coleção [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Lista todos os accessReviewScheduleDefinition. Não inclui instâncias associadas do accessReviewInstance nas listagens. |
|[Obter accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obtenha um accessReviewScheduleDefinition com uma ID especificada. |
|[Criar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Criar um novo accessReviewScheduleDefinition. |
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Nenhum. | Excluir um accessReviewScheduleDefinition com um identificador especificado. |
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Nenhum. | Atualize as propriedades de um accessReviewScheduleDefinition com um identificador especificado. |

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :------------------| :-------------- | :---------- |
| id | Cadeia de caracteres | O identificador exclusivo atribuído a um recurso de uma revisão do Access.|
| displayName | Cadeia de caracteres   | Nome da série de revisão do Access. Obrigatório durante a criação. |
| createdDateTime  |DateTimeOffset  | DateTime quando a série de revisão foi criada. |
| lastModifiedDateTime | DateTimeOffset   | DateTime quando a série de revisão foi modificada pela última vez.|
| status  |cadeia de caracteres   | Este campo somente leitura especifica o status de um accessReview. Os Estados típicos incluem,,,,,, `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` e `AutoReviewed` . |
| descriptionForAdmins  |string  |  Descrição fornecida pelos criadores de análise para fornecer mais contexto da análise para administradores. |
| descriptionForReviewers |string | Descrição fornecida pelos criadores de análise para fornecer mais contexto da revisão aos revisores. Os revisores verão esta descrição no email enviado a eles solicitando sua revisão. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Usuário que criou essa revisão. |
| escopo  |[accessReviewScope](../resources/accessreviewscope.md)  | Define o escopo de usuários revisados em um grupo. Para escopos suportados, confira [accessReviewScope](accessreviewscope.md). Obrigatório durante a criação. |
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | No caso de uma revisão todos os grupos, isso determina o escopo de quais grupos serão revisados. Cada grupo se tornará um accessReviewInstance exclusivo da série de revisão do Access.  Para escopos suportados, confira [accessReviewScope](accessreviewscope.md). | 
| configurações  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| As configurações para uma série de revisão do Access, confira definição de tipo abaixo. |
| revisores   |coleção [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de análise do Access é usada para definir quem são os revisores. Consulte [accessReviewReviewerScope](accessreviewreviewerscope.md). Obrigatório durante a criação. |
| backupReviewers   |coleção [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisor é usada para definir a lista de revisores de fallback. Esses revisores de fallback serão notificados para executar ações se nenhum usuário for encontrado na lista de revisores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como o revisor, mas o proprietário do grupo não existe, ou o gerente é especificado como revisor, mas o gerente do usuário não existe. Consulte [accessReviewReviewerScope](accessreviewreviewerscope.md). |
| instances |Coleção (Microsoft. Graph. accessReviewInstance)|  Conjunto de instâncias de revisões de acesso para esta série de análise do Access. As revisões do Access que não são recorrentes terão apenas uma instância; caso contrário, haverá uma instância para cada recorrência. |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `instances`               |coleção [accessReviewInstance](accessreviewinstance.md)         | Se o `accessReviewScheduleDefinition` é uma revisão de acesso recorrente, as instâncias representam cada recorrência. Uma revisão que não recorrente terá exatamente uma instância. As instâncias também representam cada grupo exclusivo em revisão no `accessReviewScheduleDefinition` . Se uma revisão tiver vários grupos e várias instâncias, cada grupo terá uma instância exclusiva para cada recorrência. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
  "baseType": "",
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
