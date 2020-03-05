---
title: tipo de recurso accessReviewDecision
description: No recurso de revisões do Azure AD Access, `accessReviewDecision` o representa uma decisão de revisão do Azure ad Access de um determinado acesso de uma entidade.  Em uma revisão do Access, ou uma instância de uma revisão de acesso recorrente, há uma `accessReviewDecision` por usuário revisado.  Por exemplo, se um grupo tiver dois convidados e um não convidado como membros, e uma revisão de acesso de convidados for executada para esse grupo, haverá dois objetos de decisão de análise do Access.  Se um revisor alterar sua decisão ou outro revisor o substituir, o `accessReviewDecision` será atualizado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e92eb6b17b76ac3f8e44404dfbc776463170e0fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508475"
---
# <a name="accessreviewdecision-resource-type"></a>tipo de recurso accessReviewDecision

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões do Azure AD [Access](accessreviews-root.md) , `accessReviewDecision` o representa uma decisão de revisão do Azure ad Access de um determinado acesso de uma entidade.  Em uma revisão do Access, ou uma instância de uma revisão de acesso recorrente, há uma `accessReviewDecision` por usuário revisado.  Por exemplo, se um grupo tiver dois convidados e um não convidado como membros, e uma revisão de acesso de convidados for executada para esse grupo, haverá dois objetos de decisão de análise do Access.  Se um revisor alterar sua decisão ou outro revisor o substituir, o `accessReviewDecision` será atualizado.


## <a name="methods"></a>Métodos

Nenhum.  Os objetos desse tipo são criados automaticamente pelo recurso quando uma revisão do Access Inicializa e não pode ser excluída.  Eles podem ser recuperados de uma revisão de acesso usando as relações de [decisões](../api/accessreview-listdecisions.md) e [mydecisions](../api/accessreview-listmydecisions.md) .

## <a name="properties"></a>Propriedades

Esta tabela ilustra as propriedades básicas de objetos desse tipo. 

| Propriedade                        | Tipo                         | Descrição                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | A identificação da decisão dentro da revisão do Access.                                                                                     |
| `accessReviewId`                |`String`                      | A ID gerada pelo recurso da revisão do Access.                                                                                       |
| `reviewedBy`                    |[userIdentity](useridentity.md)| A identidade do revisor. Se a recomendação tiver sido usada como revisão, o userPrincipalName estará vazio.                                                                                      |
| `reviewedDate`                  |`DateTimeOffset`              | A data e a hora em que a revisão mais recente desse direito de acesso foi fornecida.                                                                         |
| `reviewResult`                  |`String`                      | O resultado da revisão, um `NotReviewed`de, `Deny` `DontKnow` ou. `Approve`                                                                                    |
| `justification`                 |`String`                      | A justificativa de negócios do revisor, se fornecido.                                                                         |
| `appliedBy`                     |[userIdentity](useridentity.md)| Quando a revisão for concluída, se os resultados forem aplicados manualmente, a identidade do usuário que aplicou a decisão. Se a revisão foi aplicada automaticamente, o userPrincipalName estará vazio.                                                          |
| `appliedDateTime`               |`DateTimeOffset`              | A data e a hora em que a decisão de revisão foi aplicada.                                                          |
| `applyResult`                   |`String`                      | O resultado da aplicação da decisão, um de `NotApplied`, `Success` `Failed` `NotFound` ou `NotSupported`.                      |
| `accessRecommendation`          |`String`                      | A recomendação gerada pelo recurso mostrada para o revisor, um `Approve` `Deny` ou. `NotAvailable` |


Além disso, as propriedades adicionais podem estar presentes dependendo do tipo de objeto do objeto que possui o acesso que foi escolhido.  Por exemplo, se a decisão de revisão do Access for a associação de grupo ou o acesso de um usuário específico, o usuário que estiver possivelmente com o acesso será removido é identificado por estas propriedades:

| Propriedade                        | Tipo                         | Descrição                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | A ID do usuário cujo acesso foi revisado.                                                                                    |
| `userDisplayName`                            |`String`                      | O nome de exibição do usuário cujo acesso foi revisado.                                                                                     |
| `userPrincipalName`                            |`String`                      | O nome principal de usuário do usuário cujo acesso foi revisado.                                                                                     |



## <a name="relationships"></a>Relações

Nenhum  Os objetos desse tipo podem ser recuperados de uma análise do Access usando as relações de [decisões](../api/accessreview-listdecisions.md) e [mydecisions](../api/accessreview-listmydecisions.md) do objeto [accessReview](accessreview.md) .

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar decisões accessReview](../api/accessreview-listdecisions.md) |      coleção [accessReviewDecision](accessreviewdecision.md)| Obtenha as decisões de um accessReview.|
|[Listar minhas decisões do accessReview](../api/accessreview-listmydecisions.md) |     coleção [accessReviewDecision](accessreviewdecision.md)| Como revisor, obtenha as minhas decisões de um accessReview.|

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
