---
title: Listar accessReviewHistoryDefinitions
description: Obter uma lista dos objetos accessReviewHistoryDefinition.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fdee38b23bbc8c7cc37a9416e6efd30a43f1c546
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992056"
---
# <a name="list-accessreviewhistorydefinitions"></a>Listar accessReviewHistoryDefinitions
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere os [objetos accessReviewHistoryDefinition criados](../resources/accessreviewhistorydefinition.md) nos últimos 30 dias, incluindo todas as propriedades aninhadas.

>[!NOTE]
>O tamanho padrão da página para essa API é de 100 **objetos accessReviewHistoryDefinitions.** Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta. Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).
>
>Se nenhum parâmetro de consulta for fornecido e houver mais de 100 resultados, o Microsoft Graph paginará automaticamente os resultados em 100 resultados por página.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|AccessReview.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|AccessReview.ReadWrite.All|

Se o usuário de entrada não for um membro de função de diretório do Administrador Global ou um membro da função de diretório Leitor Global, somente as definições criadas pelo usuário in-loco serão retornadas.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/historyDefinitions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte `$top` aos `$filter` parâmetros de consulta , e OData para ajudar a personalizar `$skip` a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters). 

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) no corpo da resposta.

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

# <a name="go"></a>[Go](#tab/go)
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
      "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
      "displayName": "Last quarter's group reviews April 2021",
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
      "fulfilledDateTime": "2021-04-14T00:22:58.5276552Z",
      "downloadUri": "https://contoso.com/df-erm-reports/Last quarter's group reviews April 2021-22be232e-a93d-42a3-8ac5-313cfd29a0eb.csv?sv=2015-04-05&ss=b&srt=o&sp=rl&st=2021-04-15T00:22:58.5276552Z&se=2021-03-23T19:41:38.0000000Z&spr=https&sig=84rlGCIgU4ToMn%2FFLncBXq95O8a8RsFlwQY1Knl%2Fo%2FI%3D",
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
        },  
        {
          "@odata.type": "#microsoft.graph.accessReviewQueryScope",
          "queryType": "MicrosoftGraph",     
          "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
          "queryRoot": null
        }
      ]
    }
  ]
}
```
