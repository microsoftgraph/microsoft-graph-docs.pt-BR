---
title: Atualizar accessReviewScheduleDefinition
description: Atualize as propriedades de um objeto accessReviewScheduleDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6f3c39f6111ad910d2551da7e03cdf6e03597b3d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208383"
---
# <a name="update-accessreviewscheduledefinition"></a>Atualizar accessReviewScheduleDefinition
Namespace: microsoft.graph

Atualize as propriedades de [um objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)

Todas as atualizações de um accessReviewScheduleDefinition só se aplicam a instâncias futuras. As instâncias em execução no momento não podem ser atualizadas. Além disso, essa API não se destina a atualizar propriedades, incluindo decisões, no nível accessReviewInstance. Consulte [accessReviewInstance para](../resources/accessreviewinstance.md) obter mais informações sobre instâncias.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|AccessReview.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|AccessReview.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de [um objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)

A tabela a seguir mostra as propriedades aceitas para atualizar um accessReviewScheduleDefinition.

| Propriedade | Tipo | Descrição |
|:-------------|:------------|:------------|
| displayName | String | Nome da série de revisão de acesso. |
| descriptionForAdmins | String | Contexto da revisão fornecida aos administradores. |
| descriptionForReviewers | String | Contexto da revisão fornecida aos revisadores. |
| settings | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md) | As configurações de uma série de revisão de acesso. Consulte [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md). |
| revisadores | [Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|  Define quem são os revisadores. Se nenhum for especificado, a revisão será uma autoavaliação (os usuários revisam seu próprio acesso). A **propriedade reviewers** só será atualizável se usuários individuais são atribuídos como revistores. Consulte [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md). |
|fallbackReviewers|[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Uma coleção de escopos do revistor usado para definir a lista de revisadores de fallback que são notificados para tomar medidas se nenhum usuário for encontrado na lista de revisadores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como o revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe.|

Uma **solicitação PUT** espera que o objeto completo seja passado, o que inclui todas as propriedades que podem ser escritas, e não apenas as propriedades que estão sendo atualizadas.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `204 No Content` código de resposta e nenhum corpo de resposta.

## <a name="examples"></a>Exemplos
Este é um exemplo de atualização do displayName de uma série de revisão de acesso existente.

### <a name="request"></a>Solicitação
No corpo da solicitação, fornece uma representação JSON das novas propriedades do [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewscheduledefinition"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6

{
  "id": "60860cdd-fb4d-4054-91ba-f75e04444aa6",
  "displayName": "Test world UPDATED NAME!",
  "descriptionForAdmins": "Test world",
  "descriptionForReviewers": "Test world",
  "scope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "instanceEnumerationScope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 3,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-15"
      }
    }
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
