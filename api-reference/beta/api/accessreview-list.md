---
title: Listar accessReviews (preterido)
description: Recuperar objetos accessReview para um businessFlowTemplate.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 916229324c87bf4d7423dde0af86f6434e7cdef7
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819122"
---
# <a name="list-accessreviews-deprecated"></a>Listar accessReviews (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

Recupere os [objetos accessReview](../resources/accessreview.md) para um [businessFlowTemplate específico](../resources/businessflowtemplate.md). Uma lista de zero ou mais objetos **accessReview** são retornados para cada revisão de acesso única e recorrente que foi criada com esse modelo de fluxo de negócios.  Observe que as IDs do modelo de fluxo de negócios diferenciam maiúsculas de minúsculas.

>[!NOTE]
> Se qualquer uma das revisões de acesso que correspondem ao filtro for uma revisão de acesso recorrente, um objeto **accessReview** será retornado para representar cada série recorrente como um todo, além de qualquer instância atual, passada e próxima. Por exemplo, se houver uma revisão de acesso recorrente mensal de membros convidados do grupo A, uma revisão de acesso recorrente trimestral de membros convidados do grupo B e uma revisão de acesso única de membros convidados do grupo C, cada uma dessas recorrências acabou de ser iniciada e as consultas do chamador para revisões de acesso com um modelo de fluxo de negócios de revisões de membros convidados de grupos,  três objetos serão retornados representando as três séries, bem como três objetos para as instâncias de revisão de acesso atuais e, potencialmente, três objetos para as próximas instâncias. Para recuperar as instâncias de uma revisão de acesso recorrente ou a instância de revisão de acesso agendada para um mês ou trimestre específico, o chamador pode navegar subsequentemente pela relação de instância do objeto **accessReview** recorrente. A **relação** de instância vincula-se **aos objetos accessReview** para uma instância atual ou passada da revisão de acesso recorrente.

Se muitas revisões de acesso corresponderem ao filtro, para melhorar a eficiência e evitar tempos limite, recupere o conjunto de resultados em páginas, `$top` incluindo o parâmetro de consulta com um tamanho de página, por exemplo, 100 `$skip=0` e o parâmetro de consulta na solicitação. Esses parâmetros podem ser incluídos mesmo quando você não prevê que a solicitação abrangerá várias páginas. Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph `@odata.nextLink` retorna essa página com uma propriedade na resposta que contém uma URL para a próxima página de resultados. Se essa propriedade estiver presente, continue fazendo solicitações adicionais com o `@odata.nextLink` URL em cada resposta, até que todos os resultados sejam retornados, conforme descrito em [paginação de dados do Microsoft Graph no aplicativo](/graph/paging).

Os **objetos accessReview** retornados por essa API não incluirão propriedades de estrutura aninhadas, como **configurações** ou relações.  Para recuperar configurações ou relações de revisão de acesso, use a API [get accessReview](accessreview-get.md) .


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)     | AccessReview.Read.All, AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All  |
|Delegada (conta pessoal da Microsoft) | Sem suporte. |
|Application                            | AccessReview.Read.All, AccessReview.ReadWrite.Membership |

 O usuário conectado também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso.

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
Não forneça um corpo de solicitação.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `200 OK` de resposta e uma matriz de [objetos accessReview](../resources/accessreview.md) no corpo da resposta.

## <a name="examples"></a>Exemplos
##### <a name="request"></a>Solicitação
O exemplo a seguir mostra uma solicitação para recuperar todas as revisões de acesso única e recorrentes para um modelo de fluxo de negócios '6e4f3d20-c5c3-407f-9695-8460952bcc68'.

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

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-accessreviews-powershell-snippets.md)]
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


