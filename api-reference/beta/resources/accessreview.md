---
title: Tipo de recurso accessReview
description: 'No recurso de revisões de acesso do Azure AD, o representa `accessReview` uma revisão de acesso.  '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 75f844a165b8e5603f2d423a9d0a7aef17ab9186
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579274"
---
# <a name="accessreview-resource-type-deprecated"></a>Tipo de recurso accessReview (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Representa uma revisão de acesso do Azure [AD.](accessreviews-root.md)  

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviews](../api/accessreview-list.md) | [Coleção accessReview](accessreview.md) | Listar accessReviews para um businessFlowTemplate. |
|[Obter accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Obter uma revisão de acesso com uma id específica. |
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Crie um novo accessReview. |
|[Atualizar accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Atualize um accessReview. |
|[Excluir accessReview](../api/accessreview-delete.md) | Nenhum.   | Excluir um accessReview. |
|[Listar revisores do accessReview](../api/accessreview-listreviewers.md) | [Coleção userIdentity](useridentity.md)|  Obter os revisores de um accessReview. |
|[Adicionar o revisor accessReview](../api/accessreview-addreviewer.md) | Nenhum.    |   Adicione um revisor a um accessReview. |
|[Remover o revisor accessReview](../api/accessreview-removereviewer.md) | Nenhum. |    Remova um revisor de um accessReview. |
|[Listar decisões do accessReview](../api/accessreview-listdecisions.md) | [Coleção accessReviewDecision](accessreviewdecision.md) | Obter as decisões de um accessReview. |
|[Listar minhas decisões do accessReview](../api/accessreview-listmydecisions.md) | [Coleção accessReviewDecision](accessreviewdecision.md) | Como revisor, receba minhas decisões de um accessReview. |
|[Enviar lembrete accessReview](../api/accessreview-sendreminder.md) | Nenhum. | Envie um lembrete aos revisores de um accessReview. |
|[Parar accessReview](../api/accessreview-stop.md) | Nenhum. | Pare um accessReview. |
|[Redefinir as decisões do accessReview](../api/accessreview-reset.md) | Nenhum.   |   Redefinir as decisões em um accessReview em andamento. |
|[Aplicar decisões do accessReview](../api/accessreview-apply.md) | Nenhum. | Aplicar as decisões de um accessReview concluído. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:-------- |:---- |:----------- |
| id | String | O identificador exclusivo atribuído ao recurso de uma revisão de acesso. |
| displayName | String | O nome da revisão de acesso. Obrigatório durante a criação. |
| startDateTime | DateTimeOffset | DateTime quando a revisão está agendada para ser inicial.  Isso pode ser uma data no futuro.  Obrigatório durante a criação. |
| endDateTime | DateTimeOffset | DateTime quando a revisão está agendada para terminar. Isso deve ser pelo menos um dia depois da data de início.  Obrigatório durante a criação. |
| status | String | Este campo somente leitura especifica o status de um accessReview. Os estados típicos `Initializing` `NotStarted` incluem , `Starting` , , , , , e `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . |
| descrição | String | A descrição fornecida pelo criador da revisão de acesso, para mostrar aos revisadores. |
| businessFlowTemplateId | String | O identificador do modelo de fluxo de negócios. Obrigatório durante a criação.  Esse valor é sensível a minúsculas. |
| reviewerType | String | O tipo de relação do revistor para o objeto de destino, um `self` de , `delegated` ou `entityOwners` . Obrigatório durante a criação. | 
| createdBy | [userIdentity](useridentity.md) | O usuário que criou essa revisão. |
| reviewedEntity | [identity](identity.md) | O objeto para o qual as análises de acesso estão revendo as atribuições de direitos de acesso. Esse pode ser o grupo para a revisão de associações de usuários em um grupo ou o aplicativo para uma revisão de atribuições de usuários para um aplicativo. Obrigatório durante a criação. | 
| settings | [accessReviewSettings](accessreviewsettings.md) | As configurações de um accessReview, consulte a definição de tipo abaixo. |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:------------ |:---- |:----------- |
| revisadores | [Coleção userIdentity](useridentity.md) | A coleção de revisadores para uma revisão de acesso, se o access reviewerType for do tipo `delegated` . |
| decisions | [Coleção accessReviewDecision](accessreviewdecision.md) | O conjunto de decisões para essa revisão de acesso. |
| myDecisions | [Coleção accessReviewDecision](accessreviewdecision.md) | A coleção de decisões para o chamador, se o chamador for um revistor. |
| instances | [Coleção accessReview](accessreview.md) | A coleção de instâncias de críticas de acesso passado, presente e futuro, se esse objeto for uma revisão de acesso recorrente. |

Se essas relações estão presentes em um objeto, depende se o objeto é uma revisão de acesso único, a série de uma revisão de acesso recorrente ou uma instância de uma revisão de acesso recorrente.

| Cenário | Tem revisadores? | Tem decisões e myDecisions? | Tem instâncias? |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| Revisão de acesso único | Sim | Sim, uma vez iniciado | Não |
| Revisão de acesso recorrente | Sim | Não | Sim |
| Instância de uma revisão de acesso recorrente | Sim | Sim, uma vez iniciado | Não |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReview"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "description": "string",
 "businessFlowTemplateId": "string (identifier)",
 "reviewerType": "string",
 "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
 "reviewedEntity": {"@odata.type": "microsoft.graph.identity"},
 "settings": {"@odata.type": "microsoft.graph.accessReviewSettings"},
 "reviewers": [{"@odata.type": "microsoft.graph.userIdentity"}]
}

```

<!--
{
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


