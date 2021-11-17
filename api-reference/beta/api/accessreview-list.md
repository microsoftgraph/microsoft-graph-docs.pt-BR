---
title: Listar accessReviews
description: Recupere objetos accessReview para um businessFlowTemplate.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b03ba3340c74aeb4936e5442256dc5a47965be67
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988067"
---
# <a name="list-accessreviews"></a>Listar accessReviews

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere os [objetos accessReview](../resources/accessreview.md) para um [determinado businessFlowTemplate](../resources/businessflowtemplate.md). Uma lista de zero ou mais objetos **accessReview** são retornados, para cada revisão de acesso única e recorrente que foi criada com esse modelo de fluxo de negócios.  Observe que as IDs do modelo de fluxo de negócios são sensíveis a minúsculas.

>[!NOTE]
> Se qualquer uma das avaliações de acesso que correspondem ao filtro for uma revisão de acesso recorrente, um objeto **accessReview** será retornado para representar cada série recorrente como um todo, além de qualquer instância atual, passada e próxima. Por exemplo, se houver uma revisão de acesso recorrente mensal de membros convidados do grupo A, uma revisão de acesso recorrente trimestral de membros convidados do grupo B e uma revisão de acesso único de membros convidados do grupo C, cada uma dessas recorrências acabou de ser iniciada e o chamador consulta para análises de acesso com um modelo de fluxo de negócios de avaliações de membros convidados de grupos,  três objetos serão retornados representando as três séries, bem como três objetos para as instâncias de revisão de acesso atuais e, potencialmente, três objetos para as próximas instâncias. Para recuperar as instâncias de uma revisão de acesso recorrente ou a instância de revisão de  acesso agendada para um determinado mês ou trimestre, o chamador pode navegar subsequentemente pela relação de instância do objeto **accessReview** recorrente. A **relação** de instância se vincula aos **objetos accessReview** para uma instância atual ou anterior da revisão de acesso recorrente.

Se muitas análises de acesso corresponderem ao filtro, para melhorar a eficiência e evitar tempos-de-tempo, recupere o resultado definido em páginas, incluindo o parâmetro de consulta com um tamanho de página, por exemplo, 100 e o parâmetro de consulta na `$top` `$skip=0` solicitação. Esses parâmetros podem ser incluídos mesmo quando você não previu que a solicitação abrange várias páginas. Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com uma propriedade na resposta que contém uma URL para `@odata.nextLink` a próxima página de resultados. Se essa propriedade estiver presente, continue fazendo solicitações adicionais com o `@odata.nextLink` URL em cada resposta, até que todos os resultados sejam retornados, conforme descrito em [paginação de dados do Microsoft Graph no aplicativo](/graph/paging).

Os **objetos accessReview** retornados por essa API não incluirão propriedades de estrutura aninhadas, como **configurações** ou relações.  Para recuperar as configurações ou as relações de revisão de acesso, use a API [get accessReview.](accessreview-get.md)


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | AccessReview.Read.All, AccessReview.ReadWrite.Membership |

 O usuário inscreveu também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}&$top={pagesize}&$skip=0
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não fornecer um corpo de solicitação.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e uma matriz de `200 OK` [objetos accessReview](../resources/accessreview.md) no corpo da resposta.

## <a name="examples"></a>Exemplos
##### <a name="request"></a>Solicitação
O exemplo a seguir mostra uma solicitação para recuperar todas as análises de acesso único e recorrente para um modelo de fluxo de negócios '6e4f3d20-c5c3-407f-9695-8460952bcc68'.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'&$top=100&$skip=0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-accessreviews-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


##### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
       {
         "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
         "displayName": "review",
         "startDateTime": "2017-11-14T01:14:54.89Z",
         "endDateTime": "2017-12-14T01:14:54.89Z",
         "status": "InProgress",
         "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
         "reviewerType": "self",
         "description": "",
         "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"}
       }
    ]
}
```

## <a name="see-also"></a>Confira também

- [Obter accessReview](accessreview-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviews",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


