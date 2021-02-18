---
title: Tipo de recurso accessReview
description: 'No recurso de revisões de acesso do Azure AD, ele representa `accessReview` uma revisão de acesso.  '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: da155d49eedf03cdc935eeefc6b6808847176a41
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292711"
---
# <a name="accessreview-resource-type"></a>Tipo de recurso accessReview

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Representa uma revisão de acesso do Azure [AD.](accessreviews-root.md)  

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviews](../api/accessreview-list.md) | [coleção accessReview](accessreview.md) | Listar accessReviews para um businessFlowTemplate. |
|[Obter accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Obter uma revisão de acesso com uma ID específica. |
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Crie um novo accessReview. |
|[Atualizar accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Atualize um accessReview. |
|[Excluir accessReview](../api/accessreview-delete.md) | Nenhum.   | Exclua um accessReview. |
|[Listar revisores de accessReview](../api/accessreview-listreviewers.md) | [coleção userIdentity](useridentity.md)|  Obter os revisores de um accessReview. |
|[Adicionar o revisor accessReview](../api/accessreview-addreviewer.md) | Nenhum.    |   Adicione um revisor a um accessReview. |
|[Remover o revisor accessReview](../api/accessreview-removereviewer.md) | Nenhum. |    Remover um revisor de um accessReview. |
|[Listar decisões de accessReview](../api/accessreview-listdecisions.md) | [coleção accessReviewDecision](accessreviewdecision.md) | Obter as decisões de um accessReview. |
|[Listar minhas decisões de accessReview](../api/accessreview-listmydecisions.md) | [coleção accessReviewDecision](accessreviewdecision.md) | Como revisor, receba minhas decisões de um accessReview. |
|[Enviar lembrete accessReview](../api/accessreview-sendreminder.md) | Nenhum. | Envie um lembrete aos revisores de um accessReview. |
|[Parar accessReview](../api/accessreview-stop.md) | Nenhum. | Pare um accessReview. |
|[Redefinir decisões de accessReview](../api/accessreview-reset.md) | Nenhum.   |   Redefinir as decisões em um accessReview em andamento. |
|[Aplicar decisões de accessReview](../api/accessreview-apply.md) | Nenhum. | Aplicar as decisões de um accessReview concluído. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:-------- |:---- |:----------- |
| id | String | O identificador exclusivo atribuído ao recurso de uma revisão de acesso. |
| displayName | String | O nome da revisão de acesso. Obrigatório durante a criação. |
| startDateTime | DateTimeOffset | DateTime quando a revisão está agendada para ser iniciar.  Isso pode ser uma data no futuro.  Obrigatório durante a criação. |
| endDateTime | DateTimeOffset | DateTime quando a revisão está agendada para terminar. Deve ser pelo menos um dia depois da data de início.  Obrigatório durante a criação. |
| status | String | Este campo somente leitura especifica o status de um accessReview. Os estados típicos `Initializing` `NotStarted` incluem , `Starting` , , , e `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . |
| description | String | A descrição fornecida pelo criador da revisão de acesso, para mostrar aos revisadores. |
| businessFlowTemplateId | String | O identificador do modelo de fluxo de negócios. Obrigatório durante a criação.  Esse valor faz a resição entre os casos. |
| reviewerType | String | O tipo de relação do revistor para o objeto de destino, um dos `self` ou `delegated` `entityOwners` . Obrigatório durante a criação. | 
| createdBy | [userIdentity](useridentity.md) | O usuário que criou essa análise. |
| reviewedEntity | [identity](identity.md) | O objeto para o qual o acesso revisa está revendo as atribuições de direitos de acesso. Pode ser o grupo para revisão de associações de usuários em um grupo ou o aplicativo para uma revisão das atribuições de usuários para um aplicativo. Obrigatório durante a criação. | 
| settings | [accessReviewSettings](accessreviewsettings.md) | As configurações de um accessReview, consulte a definição de tipo abaixo. |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:------------ |:---- |:----------- |
| reviewers | [coleção userIdentity](useridentity.md) | A coleção de revisadores para uma revisão de acesso, se o reviewerType de acesso for do tipo `delegated` . |
| decisões | [coleção accessReviewDecision](accessreviewdecision.md) | O conjunto de decisões para esta revisão de acesso. |
| myDecisions | [coleção accessReviewDecision](accessreviewdecision.md) | A coleção de decisões para o chamador, se o chamador for um revistor. |
| instances | [coleção accessReview](accessreview.md) | A coleção de instâncias de revisões de acesso passadas, atuais e futuras, se esse objeto for uma revisão de acesso recorrente. |

Se essas relações estão presentes em um objeto, depende se o objeto é uma revisão de acesso única, a série de uma revisão de acesso recorrente ou uma instância de uma revisão de acesso recorrente.

| Cenário | Tem revisadores? | Tem decisões e myDecisions? | Tem instâncias? |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| Revisão de acesso única | Sim | Sim, uma vez iniciado | Não |
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


