---
title: Tipo de recurso accessReviewScheduleDefinition
description: Representa uma série de revisão de acesso ou revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f95047602ec1a73549b6b5c4217e32890a5996e6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161156"
---
# <a name="accessreviewscheduledefinition-resource-type"></a>Tipo de recurso accessReviewScheduleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o agendamento de uma revisão de acesso do Azure [AD.](accessreviewsv2-root.md) 

Um accessReviewScheduleDefinition contém uma lista de [objetos accessReviewInstance](accessreviewinstance.md) . Cada recorrência da definição de agenda criará uma instância. As instâncias também representam cada grupo exclusivo que está sendo revisado. Se uma definição de agenda analisar vários grupos, cada grupo terá uma instância exclusiva para cada recorrência. No caso de uma revisão única, apenas uma instância será criada por grupo.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [coleção accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Lista cada accessReviewScheduleDefinition. Não inclui instâncias de accessReviewInstance associadas em listagem. |
|[Acessar AccessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obter um accessReviewScheduleDefinition com uma id especificada. |
|[Criar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Crie um novo accessReviewScheduleDefinition. |
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Nenhum. | Exclua um accessReviewScheduleDefinition com um identificador especificado. |
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Nenhum. | Atualizar propriedades de um accessReviewScheduleDefinition com um identificador especificado. |

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :------------------| :-------------- | :---------- |
| id | String | O identificador exclusivo atribuído ao recurso de uma revisão de acesso.|
| displayName | String   | Nome da série de revisão de acesso. Obrigatório durante a criação. |
| createdDateTime  |DateTimeOffset  | DateTime quando a série de revisão foi criada. |
| lastModifiedDateTime | DateTimeOffset   | DateTime quando a série de revisão foi modificada pela última vez.|
| status  |cadeia de caracteres   | Este campo somente leitura especifica o status de um accessReview. Os estados típicos `Initializing` `NotStarted` incluem , `Starting` , , , e `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . |
| descriptionForAdmins  |string  |  Descrição fornecida pelos criadores de revisão para fornecer mais contexto da análise aos administradores. |
| descriptionForReviewers |string | Descrição fornecida pelos criadores de revisão para fornecer mais contexto da análise aos revisadores. Os revisadores verão essa descrição no email enviado a eles solicitando sua análise. |
| createdBy  |[userIdentity](../resources/useridentity.md)  | Usuário que criou essa análise. |
| escopo  |[accessReviewScope](../resources/accessreviewscope.md)  | Define o escopo dos usuários revisados em um grupo. Para escopos com suporte, consulte [accessReviewScope](accessreviewscope.md). Obrigatório durante a criação. |
| instanceEnumerationScope|[accessReviewScope](../resources/accessreviewscope.md)  | No caso de uma revisão de todos os grupos, isso determina o escopo de quais grupos serão revisados. Cada grupo se tornará um accessReviewInstance exclusivo da série de revisão de acesso.  Para escopos com suporte, consulte [accessReviewScope](accessreviewscope.md). | 
| configurações  |[accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| As configurações para uma série de revisão de acesso, consulte a definição de tipo abaixo. |
| reviewers   |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisão de acesso é usada para definir quem são os revisadores. Consulte [accessReviewReviewerScope](accessreviewreviewerscope.md). Obrigatório durante a criação. |
| backupReviewers   |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos do revisador é usada para definir a lista de revisadores de fallback. Esses revisadores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisadores especificada. Isso pode ocorrer quando o proprietário do grupo é especificado como revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente do usuário não existe. Consulte [accessReviewReviewerScope](accessreviewreviewerscope.md). |
| instances |Collection(microsoft.graph.accessReviewInstance)|  Conjunto de instâncias de revisões de acesso para esta série de revisão de acesso. As revisões de acesso que não recorrem terão apenas uma instância; Caso contrário, haverá uma instância para cada recorrência. |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `instances`               |[Coleção accessReviewInstance](accessreviewinstance.md)         | Se for `accessReviewScheduleDefinition` uma revisão de acesso recorrente, as instâncias representarão cada recorrência. Uma revisão que não recorre terá exatamente uma instância. Instâncias também representam cada grupo exclusivo sob revisão no `accessReviewScheduleDefinition` . Se uma revisão tiver vários grupos e várias instâncias, cada grupo terá uma instância exclusiva para cada recorrência. |

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
