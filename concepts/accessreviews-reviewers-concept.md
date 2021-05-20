---
title: Atribuir revisadores à sua definição de revisão de acesso usando a API Graph Microsoft
description: Saiba como usar a API de críticas de acesso no Microsoft Graph atribuir revisadores de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: f892e74f5bf7a7aa934872186208e21ede19780a
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579794"
---
# <a name="assign-reviewers-to-your-access-review-definition-using-the-microsoft-graph-api"></a>Atribuir revisadores à sua definição de revisão de acesso usando a API Graph Microsoft

A [API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) de revisões de acesso do Azure AD permite que você revise programaticamente o acesso que os usuários, entidades de serviço ou grupos têm aos recursos do Azure AD.

> [!NOTE]
> No momento, a API de [críticas](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) de acesso está disponível apenas no ponto de extremidade do Microsoft Graph beta. Não o use em aplicativos de produção, pois ele está sujeito a alterações sem aviso prévio.

Os revisores primários são configurados na propriedade **reviewers** do recurso [access Reviews accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true)  Além disso, você pode especificar revisores de fallback usando **a propriedade fallbackReviewers.** Essas propriedades não são necessárias ao criar uma auto-revisão (onde os usuários revisam seu próprio acesso).

## <a name="configure-reviewers"></a>Configurar revisadores

Para configurar os revisores e revisores de fallback, de definir os valores das propriedades **query**, **queryRoot** e **queryType** **do accessReviewReviewerScope**. Para descrições dessas propriedades, consulte [tipo de recurso accessReviewReviewerScope.](/graph/api/resources/accessreviewreviewerscope?view=graph-rest-beta&preserve-view=true)

### <a name="example-1-a-specific-user-as-the-reviewer"></a>Exemplo 1: um usuário específico como revistor

```http
"reviewers": [
    {
        "query": "/users/{user id}",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-2-members-of-a-group-as-reviewers"></a>Exemplo 2: Membros de um grupo como revisadores

```http
"reviewers": [
    {
        "query": "/groups/{group id}}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-3-group-owners-as-reviewers"></a>Exemplo 3: Proprietários do grupo como revisadores
```http
"reviewers": [
    {
        "query": "./owners",
        "queryType": "MicrosoftGraph"
    }
]
```

Para atribuir apenas os proprietários do grupo de um país específico como revisadores:

```http
"reviewers": [
    {
        "query": "/groups/{group id}/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq 'USA'",
        "type": "MicrosoftGraph”
    }
]
```

### <a name="example-4-people-managers-as-reviewers"></a>Exemplo 4: Gerentes de pessoas como revisadores

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```
Como `./manager` é uma consulta relativa, especifique a propriedade **queryRoot** com o valor `decisions` .

## <a name="see-also"></a>Confira também

+ [Configurar o escopo de sua definição de revisão de acesso](/graph/accessreviews-scope-concept)
