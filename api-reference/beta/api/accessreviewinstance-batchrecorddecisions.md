---
title: 'accessReviewInstance: batchRecordDecisions'
description: Permite que os revisores revisem todos os objetos accessReviewInstanceDecisionItem em lotes.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ab7e7e3580275aa127bbb01e34484a823d4b01bf
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030744"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a>accessReviewInstance: batchRecordDecisions
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Permite que os revisores revisem todos os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) em lotes usando **principalId,** **resourceId** ou nenhum deles.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|AccessReview.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|AccessReview.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
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
| decision  | String | Decisão de acesso para a entidade que está sendo revisada. Os valores possíveis são: `Approve`, `Deny`, `NotReviewed`, `DontKnow`. Obrigatório.  |
|  justification | String | Contexto da revisão fornecida aos administradores. Obrigatório se **justificationRequiredOnApproval** `True` estiver no **accessReviewScheduleDefinition**.  |
|principalId|String|Se fornecido, todos os **accessReviewInstanceDecisionItems** com **principalId** correspondente serão revisados neste lote. Se não for fornecido, todos os **principaisIds** serão revisados.|
|resourceId|Cadeia de caracteres|Se fornecido, todos os **accessReviewInstanceDecisionItems** com **resourceId** correspondentes serão revisados neste lote. Se não for fornecido, todos **os resourceIds** serão revisados.|



## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
Content-Type: application/json

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-batchrecorddecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-batchrecorddecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-batchrecorddecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-batchrecorddecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
