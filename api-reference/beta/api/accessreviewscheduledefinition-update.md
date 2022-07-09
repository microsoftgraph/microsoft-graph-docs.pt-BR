---
title: Atualizar accessReviewScheduleDefinition
description: Atualize um objeto accessReviewScheduleDefinition existente para alterar uma ou mais de suas propriedades.
ms.localizationpriority: medium
author: zhusijia26
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a92ccb653267783c34206749c8f98e02e1f5becb
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696852"
---
# <a name="update-accessreviewscheduledefinition"></a>Atualizar accessReviewScheduleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize um objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) existente para alterar uma ou mais de suas propriedades.

>[!NOTE]
>Todas as atualizações feitas em um accessReviewScheduleDefinition só se aplicam a instâncias futuras. As instâncias em execução no momento não podem ser atualizadas.
>Além disso, essa API não se destina a atualizar propriedades, incluindo decisões, no nível accessReviewInstance. Consulte [accessReviewInstance](../resources/accessreviewinstance.md) para obter mais informações sobre instâncias.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo                            | AccessReview.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Descrição |
|:-------------|:------------|
|Autorização|{token} de portador. Obrigatório.|
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .

A tabela a seguir mostra as propriedades aceitas para atualizar um accessReviewScheduleDefinition.

| Propriedade | Tipo | Descrição |
|:-------------|:------------|:------------|
| descriptionForAdmins | Cadeia de Caracteres | Contexto da revisão fornecida aos administradores. |
| descriptionForReviewers | Cadeia de caracteres | Contexto da revisão fornecida aos revisores. |
| displayName | Cadeia de caracteres | Nome da série de revisão de acesso. |
| fallbackReviewers|[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Uma coleção de escopos do revisores usado para definir a lista de revisores de fallback que são notificados para tomar medidas se nenhum usuário for encontrado na lista de revisores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe.|
| Revisores | [coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|  Define quem são os revisores. Se nenhum for especificado, a revisão será uma auto-revisão (os usuários revisam seu próprio acesso). A **propriedade de revisores** só poderá ser atualizada se usuários individuais forem atribuídos como revisores. Consulte [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md). |
|stageSettings|[coleção accessReviewStageSettings](../resources/accessreviewstagesettings.md)| Define quantos estágios cada instância de uma série de revisão de acesso terá. Os estágios serão criados sequencialmente com base na propriedade **dependsOn** . Cada estágio pode ter um conjunto diferente de revisores, revisores de fallback e configurações. Somente revisores e revisores de fallback são atualizáveis. Consulte [accessReviewStageSettings](../resources/accessreviewstagesettings.md). Opcional.|
| configurações | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md) | As configurações de uma série de revisão de acesso. Consulte [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md). |
| backupReviewers (preterido)|[coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa propriedade foi substituída por **fallbackReviewers**. No entanto, especificar **backupReviewers** ou **fallbackReviewers** preenche automaticamente os mesmos valores para a outra propriedade. |

Uma **solicitação PUT** espera que o objeto completo seja passado, o que inclui todas as propriedades graváveis, não apenas as propriedades que estão sendo atualizadas.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `204 No Content` de resposta e nenhum corpo de resposta.

## <a name="examples"></a>Exemplos

Este é um exemplo de atualização do displayName de uma série de revisão de acesso existente.

### <a name="request"></a>Solicitação
No corpo da solicitação, forneça uma representação JSON das novas propriedades do objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewScheduleDefinition"
}-->
```http
PUT https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6
Content-type: application/json

{
  "id": "60860cdd-fb4d-4054-91ba-f75e04444aa6",
  "displayName": "Test world UPDATED NAME!",
  "descriptionForAdmins": "Test world",
  "descriptionForReviewers": "Test world",
  "scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "instanceEnumerationScope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
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

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
