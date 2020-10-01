---
title: tipo de recurso accessReview
description: 'No recurso de revisões do Azure AD Access, o `accessReview` representa uma revisão do Access.  '
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a63291d9cefb1b6a0c249b09a95430303b3597d
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330160"
---
# <a name="accessreview-resource-type"></a>tipo de recurso accessReview

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma análise do Azure AD [Access](accessreviews-root.md).  

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviews](../api/accessreview-list.md) | coleção [accessReview](accessreview.md) | Listar accessReviews para um businessFlowTemplate. |
|[Obter accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Obtenha uma revisão do Access com uma ID específica. |
|[Criar accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Criar um novo accessReview. |
|[Atualizar accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | Atualizar um accessReview. |
|[Excluir accessReview](../api/accessreview-delete.md) | Nenhum.   | Excluir um accessReview. |
|[Listar revisores do accessReview](../api/accessreview-listreviewers.md) | coleção [UserIdentity](useridentity.md)|  Obter os revisores de um accessReview. |
|[Adicionar revisor accessReview](../api/accessreview-addreviewer.md) | Nenhum.    |   Adicionar um revisor a um accessReview. |
|[Remover revisor accessReview](../api/accessreview-removereviewer.md) | Nenhum. |    Remover um revisor de um accessReview. |
|[Listar decisões accessReview](../api/accessreview-listdecisions.md) | coleção [accessReviewDecision](accessreviewdecision.md) | Obtenha as decisões de um accessReview. |
|[Listar minhas decisões do accessReview](../api/accessreview-listmydecisions.md) | coleção [accessReviewDecision](accessreviewdecision.md) | Como revisor, obtenha as minhas decisões de um accessReview. |
|[Enviar lembrete accessReview](../api/accessreview-sendreminder.md) | Nenhum. | Envie um lembrete para os revisores de um accessReview. |
|[Parar accessReview](../api/accessreview-stop.md) | Nenhum. | Parar um accessReview. |
|[Redefinir decisões do accessReview](../api/accessreview-reset.md) | Nenhum.   |   Redefina as decisões em um accessReview em andamento. |
|[Aplicar decisões accessReview](../api/accessreview-apply.md) | Nenhum. | Aplique as decisões de um accessReview concluído. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição |
|:-------- |:---- |:----------- |
| id | Cadeia de caracteres | O identificador exclusivo atribuído a um recurso de uma revisão do Access. |
| displayName | Cadeia de caracteres | O nome de revisão do acesso. Obrigatório durante a criação. |
| startDateTime | DateTimeOffset | O DateTime quando a revisão está agendada para ser iniciada.  Isso pode ser uma data no futuro.  Obrigatório durante a criação. |
| endDateTime | DateTimeOffset | O DateTime quando a revisão é agendada para terminar. Este deve ser pelo menos um dia depois da data de início.  Obrigatório durante a criação. |
| status | Cadeia de caracteres | Este campo somente leitura especifica o status de um accessReview. Os Estados típicos incluem,,,,,, `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` e `AutoReviewed` . |
| description | Cadeia de caracteres | A descrição fornecida pelo criador de revisão de acesso, para mostrar aos revisores. |
| businessFlowTemplateId | Cadeia de caracteres | O identificador do modelo de fluxo de negócios. Obrigatório durante a criação.  Esse valor diferencia maiúsculas de minúsculas. |
| revisor | Cadeia de caracteres | O tipo de relação de revisor para o objeto de destino, um `self` `delegated` ou `entityOwners` . Obrigatório durante a criação. | 
| createdBy | [userIdentity](useridentity.md) | O usuário que criou essa revisão. |
| reviewedEntity | [identity](identity.md) | O objeto para o qual as revisões de acesso está examinando as atribuições de direitos de acesso. Isso pode ser o grupo para a revisão de associações de usuários em um grupo ou o aplicativo para uma revisão das atribuições de usuários a um aplicativo. Obrigatório durante a criação. | 
| configurações | [accessReviewSettings](accessreviewsettings.md) | As configurações de um accessReview, confira definição de tipo abaixo. |

## <a name="relationships"></a>Relações

| Relação | Tipo   | Descrição |
|:------------ |:---- |:----------- |
| revisores | coleção [UserIdentity](useridentity.md) | A coleção de revisores para uma revisão do Access, se o Access revisar revisualizador é do tipo `delegated` . |
| correta | coleção [accessReviewDecision](accessreviewdecision.md) | O conjunto de decisões para esta revisão do Access. |
| mydecisions | coleção [accessReviewDecision](accessreviewdecision.md) | O conjunto de decisões para o chamador, se o chamador for um revisor. |
| instances | coleção [accessReview](accessreview.md) | O conjunto de instâncias do Access revês passado, presente e futuro, se esse objeto for uma revisão de acesso recorrente. |

Se essas relações estão presentes em um objeto, depende se o objeto é uma revisão de acesso único, a série de uma revisão de acesso recorrente ou uma instância de uma revisão de acesso recorrente.

| Cenário | Tem revisores? | Tem decisões e mydecisions? | Tem instâncias? |
|:-------- |:-------------- |:------------------------------ |:-------------- |
| Revisão de acesso de uso único | Sim | Sim, depois de iniciado | Não |
| Análise de acesso recorrente | Sim | Não | Sim |
| Instância de uma análise de acesso recorrente | Sim | Sim, depois de iniciado | Não |

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


