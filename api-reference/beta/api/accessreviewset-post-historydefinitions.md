---
title: Criar historyDefinitions
description: Crie um novo objeto accessReviewHistoryDefinition.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: beff78c6d820d7d62956268d99c9b82ddab046a3
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697292"
---
# <a name="create-historydefinitions"></a>Criar historyDefinitions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|AccessReview.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|AccessReview.ReadWrite.All|

O usuário conectado também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso para recuperar todos os dados.  Para obter mais detalhes, consulte os requisitos de função e permissão para [revisões de acesso](../resources/accessreviewsv2-overview.md).

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identityGovernance/accessReviews/historyDefinitions
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do [objeto accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) .

A tabela a seguir mostra as propriedades necessárias usadas para criar [um accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName | Cadeia de caracteres  | Nome da coleta de dados do histórico de revisão de acesso. Obrigatório. |
|reviewHistoryPeriodStartDateTime  | DateTimeOffset  | Um carimbo de data/hora. As revisões que começam em ou após essa data serão incluídas nos dados de histórico buscados. Só será necessário se **scheduleSettings** não estiver definido.  |
|reviewHistoryPeriodEndDateTime  | DateTimeOffset  | Um carimbo de data/hora. As revisões que começam em ou antes dessa data serão incluídas nos dados de histórico buscados. Só será necessário se **scheduleSettings** não estiver definido.  |
|escopos|[coleção accessReviewQueryScope](../resources/accessreviewqueryscope.md)| Usado para filtrar quais revisões estão incluídas nos dados de histórico buscados. Busca revisões cujo escopo corresponde a esse escopo fornecido. Obrigatório. <br> Para obter mais informações, [consulte Consultas de escopo com suporte para accessReviewHistoryDefinition](#supported-scope-queries-for-accessreviewhistorydefinition). |
| scheduleSettings  |[accessReviewHistoryScheduleSettings](../resources/accessReviewHistoryScheduleSettings.md)| As configurações de uma série de definições de histórico de revisão de acesso recorrente. Obrigatório somente se **reviewHistoryPeriodStartDateTime** ou **reviewHistoryPeriodEndDateTime** não estiver definido. Ainda não há suporte.|

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a>Consultas de escopo com suporte para accessReviewHistoryDefinition

A propriedade **scopes** de [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) baseia-se em **accessReviewQueryScope**, um recurso que permite configurar recursos diferentes na propriedade de consulta. Em seguida, esses recursos representam o escopo da definição de histórico e determinam o tipo de dados do histórico de revisão incluídos no arquivo CSV para download, que é gerado quando [accessReviewHistoryInstances](../resources/accessreviewhistoryinstance.md) da definição de histórico é criado.

Use o seguinte formato para **a propriedade de** consulta:

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '{object}')
```

O valor de `{object}` é um dos recursos que podem ser configurados em **um accessReviewScheduleDefinition**. Por exemplo, o seguinte inclui todos os resultados de revisão accessReviewScheduleDefinition em grupos individuais (e exclui definições com escopo para todos os grupos do Microsoft 365 com usuários convidados).

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')
```

Para obter mais valores com suporte, consulte Usar o [parâmetro $filter consulta em accessReviewScheduleDefinition](accessreviewset-list-definitions.md#use-the-filter-query-parameter).

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um [objeto accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como criar uma definição de histórico de revisão de acesso com escopo para acessar revisões em pacotes e grupos de acesso, em execução entre a data de início de 01/01/2021 e a data de término de 05/04/2021.

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessreviewhistorydefinition_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions
Content-Type: application/json

{
  "displayName": "Last quarter's group reviews April 2021",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "scheduleSettings": {
      "reportRange": "P1M",
      "recurrence": {
          "pattern": {
              "type": "monthly",
              "interval": 1
          },
          "range": {
              "type": "noEnd",
              "startDate": "2018-08-03T21:02:30.667Z",
              "count": 0
          }
        }
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
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewhistorydefinition-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewhistorydefinition-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewhistorydefinition-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewhistorydefinition-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-accessreviewhistorydefinition-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
    "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
    "displayName": "Last quarter's group reviews April 2021",
    "scheduleSettings": {
        "reportRange": "P1M",
        "recurrence": {
            "pattern": {
                "type": "monthly",
                "interval": 1
            },
            "range": {
                "type": "noEnd",
                "startDate": "2018-08-03T21:02:30.667Z",
                "count": 0
            }
        }
    },
    "decisions": [
        "approve",
        "deny",
        "dontKnow",
        "notReviewed",
        "notNotified"
    ],
    "status": "requested",
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
        },
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "queryType": "MicrosoftGraph",
            "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
            "queryRoot": null
        }
    ]
}
```
