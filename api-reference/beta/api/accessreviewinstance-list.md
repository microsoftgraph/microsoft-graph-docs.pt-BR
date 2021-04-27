---
title: Listar accessReviewInstance
description: Recupere objetos accessReviewInstance.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c3896ea46ee4c853b6b3d1bfce4bfc79bb487c9a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048418"
---
# <a name="list-accessreviewinstance"></a>Listar accessReviewInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere os [objetos accessReviewInstance](../resources/accessreviewinstance.md) para um [accessReviewScheduleDefinition específico.](../resources/accessreviewscheduledefinition.md) Uma lista de zero ou mais **objetos accessReviewInstance** são retornados, incluindo todas as propriedades aninhadas. Os objetos retornados não incluem accessReviewInstanceDecisionItems associados. Para recuperar as decisões na instância, use [List accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem-list.md).

>[!NOTE]
>Se muitos **accessReviewInstances são retornados,** para melhorar a eficiência e evitar tempos-extra, recupere o resultado definido em páginas, incluindo o parâmetro de consulta $top com um tamanho de página de no máximo 100 e o parâmetro de consulta $skip=0 na solicitação. Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com uma propriedade @odata.nextLink na resposta que contém uma URL para a próxima página de resultados. Se essa propriedade estiver presente, continue fazendo solicitações adicionais com a URL @odata.nextLink em cada resposta, até que todos os resultados sejam retornados, conforme descrito na pa paja do Microsoft Graph dados em seu aplicativo.
>
>Se nenhum parâmetro de consulta for fornecido e houver mais de 100 resultados, o Microsoft Graph paginará automaticamente os resultados em 100 resultados por página.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.Read.All, AccessReview.ReadWrite.All  |
|Application                            | AccessReview.Read.All, AccessReview.ReadWrite.All |

O usuário interno também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso. Para exibir apenas as instâncias em que o usuário interno recebe o revistor, consulte [Listar instâncias de](accessreviewinstance-pendingaccessreviewinstances.md) revisão de acesso pendentes

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
Nenhum

## <a name="request-body"></a>Corpo da solicitação
Não fornecer um corpo de solicitação.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e uma matriz de `200 OK` [objetos accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.

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

- [Listar accessReviewScheduleDefinition](accessreviewscheduledefinition-list.md)
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
