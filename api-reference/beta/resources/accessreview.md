---
title: Tipo de recurso accessReview (preterido)
description: 'No recurso Azure AD revisões de acesso, ele representa `accessReview` uma revisão de acesso.  '
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 353dfec671a400e87f613779f9d50a6e68845a34
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819472"
---
# <a name="accessreview-resource-type-deprecated"></a>Tipo de recurso accessReview (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Representa uma Azure AD [de acesso.](accessreviews-root.md)  

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviews](../api/accessreview-list.md) | [coleção accessReview](accessreview.md) | Listar accessReviews para um businessFlowTemplate. |
|[Obter accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Obtenha uma revisão de acesso com uma ID específica. |
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Crie um novo accessReview. |
|[Atualizar accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Atualize um accessReview. |
|[Excluir accessReview](../api/accessreview-delete.md) | Nenhum   | Exclua um accessReview. |
|[Listar revisores accessReview](../api/accessreview-listreviewers.md) | [coleção userIdentity](useridentity.md)|  Obtenha os revisores de um accessReview. |
|[Adicionar revisor accessReview](../api/accessreview-addreviewer.md) | Nenhum    |   Adicione um revisor a um accessReview. |
|[Remover o revisor accessReview](../api/accessreview-removereviewer.md) | Nenhum |    Remover um revisor de um accessReview. |
|[Listar decisões de accessReview](../api/accessreview-listdecisions.md) | [coleção accessReviewDecision](accessreviewdecision.md) | Obtenha as decisões de um accessReview. |
|[Listar minhas decisões de accessReview](../api/accessreview-listmydecisions.md) | [coleção accessReviewDecision](accessreviewdecision.md) | Como revisor, obtenha minhas decisões de um accessReview. |
|[Enviar lembrete accessReview](../api/accessreview-sendreminder.md) | Nenhum | Envie um lembrete aos revisores de um accessReview. |
|[Parar accessReview](../api/accessreview-stop.md) | Nenhum | Pare um accessReview. |
|[Redefinir decisões de accessReview](../api/accessreview-reset.md) | Nenhum   |   Redefina as decisões em um accessReview em andamento. |
|[Aplicar decisões accessReview](../api/accessreview-apply.md) | Nenhum | Aplique as decisões de um accessReview concluído. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:-------- |:---- |:----------- |
| id | Cadeia de caracteres | O identificador exclusivo atribuído ao recurso de uma revisão de acesso. |
| displayName | Cadeia de caracteres | O nome da revisão de acesso. Obrigatório durante a criação. |
| startDateTime | DateTimeOffset | O DateTime quando a revisão está agendada para ser iniciada.  Isso pode ser uma data no futuro.  Obrigatório durante a criação. |
| endDateTime | DateTimeOffset | O DateTime quando a revisão está agendada para terminar. Isso deve ser pelo menos um dia depois da data de início.  Obrigatório durante a criação. |
| status | Cadeia de caracteres | Esse campo somente leitura especifica o status de um accessReview. Os estados típicos incluem `Initializing`, `NotStarted`, `Starting`,`InProgress` , `Completing`, `Completed`e `AutoReviewed``AutoReviewing`. |
| description | Cadeia de caracteres | A descrição fornecida pelo criador da revisão de acesso para mostrar aos revisores. |
| businessFlowTemplateId | Cadeia de caracteres | O identificador do modelo de fluxo de negócios. Obrigatório durante a criação.  Esse valor diferencia maiúsculas de minúsculas. |
| reviewerType | Cadeia de caracteres | O tipo de relação do revistor com o objeto de destino, um de `self`, `delegated` ou `entityOwners`. Obrigatório durante a criação. | 
| createdBy | [userIdentity](useridentity.md) | O usuário que criou essa revisão. |
| reviewedEntity | [identity](identity.md) | O objeto para o qual as revisões de acesso estão revisando as atribuições de direitos de acesso. Esse pode ser o grupo para a revisão de associações de usuários em um grupo ou o aplicativo para uma revisão das atribuições de usuários a um aplicativo. Obrigatório durante a criação. | 
| settings | [accessReviewSettings](accessreviewsettings.md) | As configurações de um accessReview, consulte a definição de tipo abaixo. |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:------------ |:---- |:----------- |
| Revisores | [coleção userIdentity](useridentity.md) | A coleção de revisores para uma revisão de acesso, se o reviewerType de acesso for do tipo `delegated`. |
| Decisões | [coleção accessReviewDecision](accessreviewdecision.md) | A coleção de decisões para essa revisão de acesso. |
| myDecisions | [coleção accessReviewDecision](accessreviewdecision.md) | A coleção de decisões para o chamador, se o chamador for um revisores. |
| instances | [coleção accessReview](accessreview.md) | A coleção de revisões de acesso revisões de instâncias passadas, presentes e futuras, se esse objeto for uma revisão de acesso recorrente. |

Se essas relações estão presentes em um objeto, depende se o objeto é uma revisão de acesso única, a série de uma revisão de acesso recorrente ou uma instância de uma revisão de acesso recorrente.

| Cenário | Tem revisores? | Tem decisões e myDecisions? | Tem instâncias? |
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


