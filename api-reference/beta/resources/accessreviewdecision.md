---
title: tipo de recurso de accessReviewDecision
description: No Windows Azure AD access analisa o recurso, o `accessReviewDecision` representa uma decisão de revisão de acesso do Azure AD de acesso de uma entidade específica.  Dentro de uma revisão de acesso ou uma instância de uma análise mais acesso recorrentes, há um `accessReviewDecision` por usuário revisado.  Por exemplo, se um grupo tem dois convidados e um não-convidado como membros e uma revisão de acesso de convidados é executada para esse grupo, e em seguida, haverá dois objetos de decisão de revisão de acesso.  Se um revisor altera sua decisão ou outro revisor substitui-los, em seguida, a `accessReviewDecision` é atualizado.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9642c8a51e4e9efe1a1748243b0e24aeff07cfa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517397"
---
# <a name="accessreviewdecision-resource-type"></a>tipo de recurso de accessReviewDecision

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de [acesso analisa](accessreviews-root.md) Azure AD, o `accessReviewDecision` representa uma decisão de revisão de acesso do Azure AD de acesso de uma entidade específica.  Dentro de uma revisão de acesso ou uma instância de uma análise mais acesso recorrentes, há um `accessReviewDecision` por usuário revisado.  Por exemplo, se um grupo tem dois convidados e um não-convidado como membros e uma revisão de acesso de convidados é executada para esse grupo, e em seguida, haverá dois objetos de decisão de revisão de acesso.  Se um revisor altera sua decisão ou outro revisor substitui-los, em seguida, a `accessReviewDecision` é atualizado.


## <a name="methods"></a>Métodos

Nenhum.  Objetos desse tipo são criados automaticamente pelo recurso quando um acesso Revise inicializa e não podem ser excluídas.  Eles podem ser recuperados de uma revisão de acesso usando as relações de [decisões](../api/accessreview-listdecisions.md) e [mydecisions](../api/accessreview-listmydecisions.md) .

## <a name="properties"></a>Propriedades

Esta tabela ilustra as propriedades de base dos objetos desse tipo. 

| Propriedade                        | Tipo                         | Descrição                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | A identificação da decisão dentro da revisão do access.                                                                                     |
| `accessReviewId`                |`String`                      | A id da revisão acesso gerados pelo recurso.                                                                                       |
| `reviewedBy`                    |[userIdentity](useridentity.md)| A identidade do revisor.                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | A data e hora da revisão mais recente para que isso direito de acesso foi fornecido.                                                                         |
| `reviewResult`                  |`String`                      | O resultado da revisão.                                                                                    |
| `justification`                 |`String`                      | Justificativa do revisor comercial, se fornecido.                                                                         |
| `appliedBy`                     |[userIdentity](useridentity.md)| Quando a revisão completa, se os resultados foram aplicados manualmente, a identidade do usuário do usuário que é aplicado a decisão.                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | A data e a hora quando a decisão de revisão foi aplicada.                                                          |
| `applyResult`                   |`String`                      | O resultado da aplicação a decisão, uma das `NotApplied`, `Success`, `Failed`, `NotFound` ou `NotSupported`.                      |
| `accessRecommendation`          |`String`                      | A recomendação recurso-gerado mostrada ao revisor, uma das `Approve`, `Deny` ou `NotAvailable`. |


Além disso, as propriedades adicionais podem estar presentes dependendo do tipo de objeto do objeto com o access que foi decidido.  Por exemplo, se a decisão de revisão de acesso é a associação de grupo de um usuário específico ou acesso de aplicativo, o usuário que será potencialmente ter seu acesso a ser removida é identificado através dessas propriedades:

| Propriedade                        | Tipo                         | Descrição                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | A id de usuário cujo acesso foi examinado.                                                                                    |
| `userDisplayName`                            |`String`                      | O nome de exibição do usuário cujo acesso foi examinado.                                                                                     |
| `userPrincipalName`                            |`String`                      | O nome principal de usuário do usuário cujo acesso foi examinado.                                                                                     |



## <a name="relationships"></a>Relações

Nenhum  Objetos desse tipo podem ser recuperados de uma revisão de acesso usando as relações de [decisões](../api/accessreview-listdecisions.md) e [mydecisions](../api/accessreview-listmydecisions.md) do objeto [accessReview](accessreview.md) .

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista accessReview decisões](../api/accessreview-listdecisions.md) |      coleção [accessReviewDecision](accessreviewdecision.md)| Obtenha as decisões de um accessReview.|
|[Listar meus decisões accessReview](../api/accessreview-listmydecisions.md) |     coleção [accessReviewDecision](accessreviewdecision.md)| Como um revisor, obtenha Minhas decisões de um accessReview.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviewdecision.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
