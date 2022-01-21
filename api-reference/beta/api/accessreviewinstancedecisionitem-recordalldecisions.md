---
title: 'accessReviewInstanceDecisionItem: recordAllDecisions'
description: Grave as decisões de um objeto accessReviewInstanceDecisionItem.
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fb5fd711253e15c8609ce7cac16452dae6a6c9c1
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162175"
---
# <a name="accessreviewinstancedecisionitem-recordalldecisions"></a>accessReviewInstanceDecisionItem: recordAllDecisions
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Como revisor de uma revisão de acesso, grave uma decisão para [um accessReviewInstanceDecisionItem](../resources/accessReviewInstanceDecisionItem.md) atribuído a você e que corresponde às IDs principais ou de recurso especificadas. Se nenhuma IDs for especificada, as decisões serão aplicadas a cada **accessReviewInstanceDecisionItem** para o qual você é o revisor.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.Read.All, AccessReview.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application                            | AccessReview.Read.All, AccessReview.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/decisions/filterByCurrentUser(on='reviewer')/recordAllDecisions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|decision|Cadeia de caracteres| A decisão de fornecer. Os valores possíveis são `Approve` `Deny` , , `DontKnow` . |
|justification|Cadeia de caracteres|Justificativa para fornecer a decisão.|
|principalId|Cadeia de caracteres|Se fornecido, todos os itens de decisão correspondentes ao principalId terão essa decisão registrada.|
|resourceId|Cadeia de caracteres|Se fornecido, todos os itens de decisão correspondentes ao resourceId terão essa decisão registrada.|



## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "accessreviewinstancedecisionitem-recordalldecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/decisions/filterByCurrentUser(on='reviewer')/recordAllDecisions
Content-Type: application/json

{
  "decision": "Deny",
  "justification": "Alice switched teams and no longer works with this group",
  "principalId": "2043848d-e422-473c-8607-88a3319ff491",
  "resourceId": "733ef921-89e1-4d7e-aeff-83612223c37e"
}
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

