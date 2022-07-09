---
title: Listar instâncias
description: Recuperar objetos accessReviewInstance.
ms.localizationpriority: medium
author: zhusijia26
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 852640c90e02cd659e3b9e31c37c1625abd9121a
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696842"
---
# <a name="list-instances"></a>Instâncias de lista

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere os [objetos accessReviewInstance](../resources/accessreviewinstance.md) para um [accessReviewScheduleDefinition específico](../resources/accessreviewscheduledefinition.md). Uma lista de zero ou mais **objetos accessReviewInstance** é retornada, incluindo todas as suas propriedades aninhadas. Os objetos retornados não incluem accessReviewInstanceDecisionItems associados. Para recuperar as decisões na instância, use [List accessReviewInstanceDecisionItem](accessreviewinstance-list-decisions.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.Read.All, AccessReview.ReadWrite.All  |
|Aplicativo                            | AccessReview.Read.All, AccessReview.ReadWrite.All |

O usuário conectado também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso. Para exibir apenas as instâncias em que o usuário conectado recebe o revistor, consulte [Listar instâncias de revisão de acesso pendentes](accessreviewinstance-pendingaccessreviewinstances.md)

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá `$select`suporte a `$filter`parâmetros `$orderBy`de consulta , , `$skip`e `$top` OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

O tamanho de página padrão para essa API é de 100 **objetos accessReviewInstance** . Para melhorar a eficiência e evitar tempos limite devido a grandes conjuntos de resultados, aplique a paginação usando os `$skip` `$top` parâmetros e de consulta. Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).

## <a name="request-headers"></a>Cabeçalhos de solicitação
Nenhum.

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código `200 OK` de resposta e uma matriz de [objetos accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.

## <a name="examples"></a>Exemplos
### <a name="request"></a>Solicitação
O exemplo a seguir mostra uma solicitação para recuperar todas as instâncias de revisão de acesso para uma definição.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances?$top=100&$skip=0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accessreviewinstance-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('8564a649-4f67-4e09-88e7-55def6530e88')/instances",
    "@odata.count": 2,
    "value": [
        {
            "id": "7bc18cf4-3d70-4009-bc8e-a7c5adb30849",
            "startDateTime": "2021-03-09T23:10:28.83Z",
            "endDateTime": "2021-03-09T23:10:28.83Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/f661fdd0-f0f7-42c0-8281-e89c6527ac63/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        },
        {
            "id": "f1f35945-3f42-4941-9f7b-465e545f6f99",
            "startDateTime": "2021-03-09T23:10:28.83Z",
            "endDateTime": "2021-03-09T23:10:28.83Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/f4ac55b3-3b3c-417e-85bd-183bbda3ccf2/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```

## <a name="see-also"></a>Confira também

- [Listar accessReviewScheduleDefinition](accessreviewset-list-definitions.md)
- [Obter accessReviewInstance](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
