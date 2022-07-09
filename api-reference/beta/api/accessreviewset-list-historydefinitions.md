---
title: Listar historyDefinitions
description: Obtenha uma lista dos objetos accessReviewHistoryDefinition.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a7faa9287447f6cf5e1615cc5839846eba14ad37
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696851"
---
# <a name="list-historydefinitions"></a>Listar historyDefinitions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere os [objetos accessReviewHistoryDefinition criados](../resources/accessreviewhistorydefinition.md) nos últimos 30 dias, incluindo todas as propriedades aninhadas.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|AccessReview.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|AccessReview.ReadWrite.All|

Se o usuário conectado não for um membro da função de diretório global do Administração ou um membro da função de diretório Leitor Global, somente as definições que o usuário conectado criou serão retornadas.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identityGovernance/accessReviews/historyDefinitions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método dá suporte aos `$top`parâmetros de consulta , `$filter``$expand`e `$skip` OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters). A `?$expand=instances` inclusão retornará [os objetos accessReviewHistoryDefinitions](../resources/accessreviewhistorydefinition.md) juntamente com suas instâncias associadas.

O tamanho de página padrão para essa API é de 100 **objetos accessReviewHistoryDefinitions** . Para melhorar a eficiência e evitar tempos limite devido a grandes conjuntos de resultados, aplique a paginação usando os `$skip` `$top` parâmetros e de consulta. Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de [objetos accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewhistorydefinition"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewhistorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewhistorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewhistorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewhistorydefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accessreviewhistorydefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition",
  "isCollection": "true"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
            "id": "67e3de15-d263-45a9-8f4f-71271b495db7",
            "displayName": "Last year's ELM assignment reviews - one time",
            "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
            "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
            "decisions": [
                "approve",
                "deny",
                "dontKnow",
                "notReviewed",
                "notNotified"
            ],
            "status": "done",
            "createdDateTime": "2021-04-14T00:22:48.9392594Z",
            "createdBy": {
                "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
                "displayName": "MOD Administrator",
                "userPrincipalName": "admin@contoso.com"
            },
            "scopes": [
                {
                    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                    "queryType": "MicrosoftGraph",
                    "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
                    "queryRoot": null
                }
            ]
        }
    ]
}
```
