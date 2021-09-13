---
title: Atribuir revisadores à sua revisão de acesso usando a API Graph Microsoft
description: Saiba como usar a API de críticas de acesso no Microsoft Graph atribuir revisadores de acesso.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 53961c4dbadfa2732d45a277233673aac1ddb41e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139321"
---
# <a name="assign-reviewers-to-your-access-review-using-the-microsoft-graph-api"></a>Atribuir revisadores à sua revisão de acesso usando a API Graph Microsoft

A [API](/graph/api/resources/accessreviewsv2-root) de revisões de acesso do Azure AD permite que você revise programaticamente o acesso que os usuários, entidades de serviço ou grupos têm aos recursos do Azure AD.

Os revisores primários são configurados na propriedade **reviewers** do recurso [access Reviews accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition)  Além disso, você pode especificar revisores de fallback usando **a propriedade fallbackReviewers.** Essas propriedades não são necessárias ao criar uma auto-revisão (onde os usuários revisam seu próprio acesso).

## <a name="configure-reviewers"></a>Configurar revisadores

Para configurar os revisores e revisores de fallback, de definir os valores das propriedades **query**, **queryRoot** e **queryType** **do accessReviewReviewerScope**. Para descrições dessas propriedades, consulte [tipo de recurso accessReviewReviewerScope.](/graph/api/resources/accessreviewreviewerscope)

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

### <a name="example-5-application-owners-as-reviewers"></a>Exemplo 5: proprietários de aplicativos como revisadores

```http
"reviewers": [
    {
        "query": "/servicePrincipals/{id}/owners",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="see-also"></a>Confira também

+ [Configurar o escopo de sua definição de revisão de acesso](/graph/accessreviews-scope-concept)
