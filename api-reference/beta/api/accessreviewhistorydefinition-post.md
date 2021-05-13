---
title: Criar accessReviewHistoryDefinition
description: Crie um novo objeto accessReviewHistoryDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3c0a1309ae67a2f4aa3f066deb5fe8adeec84119
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474103"
---
# <a name="create-accessreviewhistorydefinition"></a>Criar accessReviewHistoryDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|AccessReview.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|AccessReview.ReadWrite.All|

O usuário de entrada também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso para recuperar todos os dados.  Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviewsv2-root.md)

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

No corpo da solicitação, fornece uma representação JSON do [objeto accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)

A tabela a seguir mostra as propriedades necessárias usadas para criar [um accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName | String  | Nome da coleção de dados do histórico de revisão de acesso. Obrigatório. |
|reviewHistoryPeriodStartDateTime  | DateTimeOffset  | Timestamp, as avaliações que começam em ou após essa data serão incluídas nos dados de histórico buscados. Obrigatório.  |
|reviewHistoryPeriodEndDateTime  | DateTimeOffset  | Timestamp, as avaliações que começam em ou antes dessa data serão incluídas nos dados de histórico buscados. Obrigatório.  |
|escopos|coleção microsoft.graph.accessReviewQueryScope| Usado para filtrar quais avaliações estão incluídas nos dados de histórico buscados. Busca avaliações cujo escopo corresponde a esse escopo fornecido. Obrigatório.  |

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a>Consultas de escopo com suporte para accessReviewHistoryDefinition

A seguir, há consultas com suporte em [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) com base no [accessreviewqueryscope](../resources/accessreviewqueryscope.md). Esses escopos ditam que tipo de dados de histórico de revisão são incluídos no arquivo CSV baixável gerado quando a definição é criada.

|Cenário| Consulta |
|--|--|
| Incluir cada resultado de revisão em grupos individuais (exclui definições com escopo para todos os grupos Microsoft 365 `accessReviewScheduleDefinition` com usuários convidados) | /identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')" |
| Incluir todos os resultados de revisão em um grupo específico (exclui definições com escopo para todos os grupos Microsoft 365 `accessReviewScheduleDefinition` com usuários convidados) | /identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups/{group id}') |
| Incluir todos `accessReviewScheduleDefinition` os resultados de revisão com escopo para todos os grupos Microsoft 365 com usuários convidados | /identityGovernance/accessReviews/definitions?$filter=contains(scope/query, './members') |
| Incluir todos `accessReviewScheduleDefinition` os resultados de revisão em um pacote de acesso | /identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments') |
| Incluir todos `accessReviewScheduleDefinition` os resultados de revisão para entidades de serviço atribuídas à função privilegiada | /identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances') |
| Incluir cada `accessReviewScheduleDefinition` resultado de revisão para reivews de um grupo específico | /identityGovernance/accessReviews/definitions?$filter=scope/query eq '/groups/a1382a9b-8320-4e9c-8f73-dfead37d7723/members' |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir mostra como criar uma definição de histórico de revisão de acesso com escopo para acessar análises em pacotes e grupos de acesso, em execução entre a data de início de 01/01/2021 e a data de término de 05/04/2021.

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
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
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
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "status": "requested",
  "createdDateTime": "2021-04-14T00:22:48.9392594Z",
  "fulfilledDateTime": null,
  "downloadUri": null,
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
