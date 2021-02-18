---
title: Tipo de recurso accessReviewDecision
description: The accessReviewDecision represents an Azure AD access review decision of a particular entity's access.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 52d4e2a262d3a90010cc0e254e11f2d723a5e550
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292690"
---
# <a name="accessreviewdecision-resource-type"></a>Tipo de recurso accessReviewDecision

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

No recurso de revisões de acesso do Azure [AD,](accessreviews-root.md) ele representa uma decisão de revisão de acesso do `accessReviewDecision` Azure AD do acesso de uma entidade específica.  Em uma revisão de acesso ou em uma instância de uma revisão de acesso recorrente, há um `accessReviewDecision` por usuário revisado.  Por exemplo, se um grupo tiver dois convidados e um não convidado como membros e uma revisão de acesso dos convidados for executada para esse grupo, haverá dois objetos de decisão de revisão de acesso.  Se um revisador alterar sua decisão ou outro revisá-los, a `accessReviewDecision` atualização será atualizada.


## <a name="methods"></a>Métodos

Nenhum.  Os objetos desse tipo são criados automaticamente pelo recurso quando uma revisão de acesso é inicializada e não podem ser excluídos.  Eles podem ser recuperados de uma revisão de acesso usando [as decisões](../api/accessreview-listdecisions.md) e as relações de [mydecisions.](../api/accessreview-listmydecisions.md)

## <a name="properties"></a>Propriedades

Esta tabela ilustra as propriedades base dos objetos desse tipo. 

| Propriedade                        | Tipo                         | Descrição                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | A id da decisão dentro da revisão de acesso.                                                                                     |
| `accessReviewId`                |`String`                      | A ID gerada pelo recurso da revisão de acesso.                                                                                       |
| `reviewedBy`                    |[userIdentity](useridentity.md)| A identidade do revistor. Se a recomendação foi usada como revisão, o userPrincipalName está vazio.                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | A data e a hora em que a revisão mais recente desse direito de acesso foi fornecida.                                                                         |
| `reviewResult`                  |`String`                      | O resultado da revisão, um de `NotReviewed` , `Deny` ou `DontKnow` `Approve` .                                                                                    |
| `justification`                 |`String`                      | A justificativa comercial do revisador, se fornecida.                                                                         |
| `appliedBy`                     |[userIdentity](useridentity.md)| Quando a revisão for concluída, se os resultados foram aplicados manualmente, a identidade do usuário que aplicou a decisão. Se a revisão foi aplicada automaticamente, o userPrincipalName está vazio.                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | A data e a hora em que a decisão de revisão foi aplicada.                                                          |
| `applyResult`                   |`String`                      | O resultado da aplicação da decisão, um dos `NotApplied` `Success` , ou `Failed` `NotFound` `NotSupported` .                      |
| `accessRecommendation`          |`String`                      | O recurso - gerado recomendação mostrada para o revisador, um dos `Approve` ou `Deny` `NotAvailable` . |


Além disso, propriedades adicionais podem estar presentes dependendo do tipo de objeto do objeto que possui o acesso que foi decidido.  Por exemplo, se a decisão de revisão de acesso for a associação de grupo de um usuário específico ou o acesso a aplicativos, o usuário que potencialmente terá seu acesso removido será identificado por meio dessas propriedades:

| Propriedade                        | Tipo                         | Descrição                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | A id do usuário cujo acesso foi revisado.                                                                                    |
| `userDisplayName`                            |`String`                      | O nome de exibição do usuário cujo acesso foi revisado.                                                                                     |
| `userPrincipalName`                            |`String`                      | O nome principal do usuário cujo acesso foi revisado.                                                                                     |



## <a name="relationships"></a>Relações

Nenhum  Objetos desse tipo podem ser recuperados de [](../api/accessreview-listdecisions.md) uma revisão de acesso usando as decisões e as relações de [mydecisions](../api/accessreview-listmydecisions.md) do [objeto accessReview](accessreview.md) .

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar decisões de accessReview](../api/accessreview-listdecisions.md) |      [coleção accessReviewDecision](accessreviewdecision.md)| Obter as decisões de um accessReview.|
|[Listar minhas decisões de accessReview](../api/accessreview-listmydecisions.md) |     [coleção accessReviewDecision](accessreviewdecision.md)| Como revisor, receba minhas decisões de um accessReview.|

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


