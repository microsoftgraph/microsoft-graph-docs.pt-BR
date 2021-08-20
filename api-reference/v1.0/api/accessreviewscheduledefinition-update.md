---
title: Atualizar accessReviewScheduleDefinition
description: Atualize as propriedades de um objeto accessReviewScheduleDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: cd09f268bd1e25645ed782e6c0102b8837c23be5
ms.sourcegitcommit: 1e9a53e7b8e67349288f5cfbabe8355de83817b0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2021
ms.locfileid: "58366607"
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
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
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
| displayName | Cadeia de caracteres | Nome da série de revisão de acesso. |
| descriptionForAdmins | Cadeia de caracteres | Contexto da revisão fornecida aos administradores. |
| descriptionForReviewers | Cadeia de caracteres | Contexto da revisão fornecida aos revisadores. |
| configurações | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md) | As configurações de uma série de revisão de acesso. Consulte [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md). |
| revisadores | [Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|  Define quem são os revisadores. Se nenhum for especificado, a revisão será uma autoavaliação (os usuários revisam seu próprio acesso). A **propriedade reviewers** só será atualizável se usuários individuais são atribuídos como revistores. Consulte [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md). |
|fallbackReviewers|[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|Uma coleção de escopos do revistor usado para definir a lista de revisadores de fallback que são notificados para tomar medidas se nenhum usuário for encontrado na lista de revisadores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como o revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe.|

Uma **solicitação PUT** espera que o objeto completo seja passado, o que inclui todas as propriedades que podem ser escritas, e não apenas as propriedades que estão sendo atualizadas.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `204 No Content` código de resposta e nenhum corpo de resposta.

## <a name="examples"></a>Exemplos
Este é um exemplo de atualização do displayName de uma série de revisão de acesso existente.

### <a name="request"></a>Solicitação

No corpo da solicitação, fornece uma representação JSON das novas propriedades do [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)


<!-- {
  "blockType": "request",
  "name": "update_accessreviewscheduledefinition"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6
Content-type: application/json

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

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
