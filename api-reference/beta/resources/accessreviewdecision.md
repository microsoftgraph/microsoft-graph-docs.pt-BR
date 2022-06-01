---
title: Tipo de recurso accessReviewDecision (preterido)
description: A accessReviewDecision representa Azure AD decisão de revisão de acesso de acesso de uma entidade específica.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eb85de238c852d1e4e397cd142e7bb4863e3f2a1
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820795"
---
# <a name="accessreviewdecision-resource-type-deprecated"></a>Tipo de recurso accessReviewDecision (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

No recurso Azure AD [revisões](accessreviews-root.md) de acesso, `accessReviewDecision` representa uma decisão Azure AD de revisão de acesso de uma determinada entidade.  Em uma revisão de acesso ou em uma instância de uma revisão de acesso recorrente, há uma por `accessReviewDecision` usuário revisado.  Por exemplo, se um grupo tiver dois convidados e um não convidado como membros e uma revisão de acesso de convidados for executada para esse grupo, haverá dois objetos de decisão de revisão de acesso.  Se um revisores alterar sua decisão ou outro revisores substituí-los, ele `accessReviewDecision` será atualizado.


## <a name="methods"></a>Métodos

Nenhum.  Objetos desse tipo são criados automaticamente pelo recurso quando uma revisão de acesso é inicializada e não podem ser excluídos.  Eles podem ser recuperados de uma revisão de acesso usando as [decisões](../api/accessreview-listdecisions.md) [e as relações de mydecisions](../api/accessreview-listmydecisions.md) .

## <a name="properties"></a>Propriedades

Esta tabela ilustra as propriedades base de objetos desse tipo. 

| Propriedade                        | Tipo                         | Descrição                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | A ID da decisão na revisão de acesso.                                                                                     |
| `accessReviewId`                |`String`                      | A ID gerada pelo recurso da revisão de acesso.                                                                                       |
| `reviewedBy`                    |[userIdentity](useridentity.md)| A identidade do revistor. Se a recomendação tiver sido usada como revisão, o userPrincipalName estará vazio.                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | A data e a hora em que a revisão mais recente desse direito de acesso foi fornecida.                                                                         |
| `reviewResult`                  |`String`                      | O resultado da revisão, um de `NotReviewed`, `Deny`ou `DontKnow` `Approve`.                                                                                    |
| `justification`                 |`String`                      | A justificativa comercial do revisores, se fornecida.                                                                         |
| `appliedBy`                     |[userIdentity](useridentity.md)| Quando a revisão for concluída, se os resultados forem aplicados manualmente, a identidade do usuário que aplicou a decisão. Se a revisão foi aplicada automaticamente, o userPrincipalName estará vazio.                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | A data e a hora em que a decisão de revisão foi aplicada.                                                          |
| `applyResult`                   |`String`                      | O resultado da aplicação da decisão, um de `NotApplied`, `Success`, `Failed`ou `NotFound` `NotSupported`.                      |
| `accessRecommendation`          |`String`                      | A recomendação gerada pelo recurso mostrada ao revistor, uma das `Approve`, `Deny` ou `NotAvailable`. |


Além disso, propriedades adicionais podem estar presentes dependendo do tipo de objeto do objeto que possui o acesso que foi decidido.  Por exemplo, se a decisão de revisão de acesso for a associação de grupo ou o acesso ao aplicativo de um usuário específico, o usuário que potencialmente terá seu acesso removido será identificado por meio destas propriedades:

| Propriedade                        | Tipo                         | Descrição                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | A ID do usuário cujo acesso foi revisado.                                                                                    |
| `userDisplayName`                            |`String`                      | O nome de exibição do usuário cujo acesso foi revisado.                                                                                     |
| `userPrincipalName`                            |`String`                      | O nome principal do usuário cujo acesso foi revisado.                                                                                     |



## <a name="relationships"></a>Relações

Nenhum  Objetos desse tipo podem ser recuperados de uma revisão de acesso usando as [](../api/accessreview-listdecisions.md) decisões e as relações [de mydecisions](../api/accessreview-listmydecisions.md) do [objeto accessReview](accessreview.md).

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar decisões de accessReview](../api/accessreview-listdecisions.md) |      [coleção accessReviewDecision](accessreviewdecision.md)| Obtenha as decisões de um accessReview.|
|[Listar minhas decisões de accessReview](../api/accessreview-listmydecisions.md) |     [coleção accessReviewDecision](accessreviewdecision.md)| Como revisor, obtenha minhas decisões de um accessReview.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReviewDecision"
}-->

```json
{
"id": "string (identifier)",
"accessReviewId": "string (identifier)",
"reviewedBy": "microsoft.graph.userIdentity",
"reviewedDate": "string (timestamp)",
"reviewResult": "string",
"justification": "string",
"appliedBy": "microsoft.graph.userIdentity",
"appliedDateTime": "string (timestamp)",
"applyResult": "string",
"accessRecommendation": "string",
"userId": "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


