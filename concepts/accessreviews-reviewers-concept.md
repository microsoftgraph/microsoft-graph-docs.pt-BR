---
title: Atribuir revisadores à sua revisão de acesso usando o microsoft API do Graph
description: Saiba como usar a API de críticas de acesso no Microsoft Graph atribuir revisadores de acesso.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 099419f3c1998b94f1c57d983b8d25af0b653faf
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510650"
---
# <a name="assign-reviewers-to-your-access-review-using-the-microsoft-graph-api"></a>Atribuir revisadores à sua revisão de acesso usando o microsoft API do Graph

A [API](/graph/api/resources/accessreviewsv2-overview) de revisões de acesso do Azure AD permite que você revise programaticamente o acesso que os usuários, entidades de serviço ou grupos têm aos recursos do Azure AD.

Os revisores primários são configurados na propriedade **reviewers** do recurso [access Reviews accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition) .  Além disso, você pode especificar revisores de fallback usando **a propriedade fallbackReviewers** . Essas propriedades não são necessárias ao criar uma auto-revisão (onde os usuários revisam seu próprio acesso).

## <a name="configure-reviewers"></a>Configurar revisadores

Para configurar os revisores e revisores de fallback, de definir os valores das propriedades **queryRoot** e **queryType** **do accessReviewReviewerScope**.  Para descrições dessas propriedades, consulte [tipo de recurso accessReviewReviewerScope](/graph/api/resources/accessreviewreviewerscope) .

### <a name="example-1-a-self-review"></a>Exemplo 1: uma autoavaliação

```http
"reviewers": []
```

Para configurar uma auto-revisão, não especifique a propriedade **reviewers** ou fornece um objeto vazio à propriedade.

Se o escopo de revisão  de acesso correspondente atingir usuários de conexão direta B2B e equipes com canais compartilhados, o proprietário da equipe será atribuído para revisar o acesso para os usuários de conexão direta B2B.

### <a name="example-2-a-specific-user-as-the-reviewer"></a>Exemplo 2: um usuário específico como revistor

```http
"reviewers": [
    {
        "query": "/users/{user id}",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-3-members-of-a-group-as-reviewers"></a>Exemplo 3: Membros de um grupo como revisadores

```http
"reviewers": [
    {
        "query": "/groups/{group id}}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-4-group-owners-as-reviewers"></a>Exemplo 4: proprietários do grupo como revisadores
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

### <a name="example-5-people-managers-as-reviewers"></a>Exemplo 5: Gerentes de pessoas como revisadores

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```

Como `./manager` é uma consulta relativa, especifique a **propriedade queryRoot** com o valor `decisions`.

Se o escopo de revisão  de acesso correspondente atingir usuários de conexão direta B2B e equipes com canais compartilhados, o proprietário da equipe será atribuído para revisar o acesso para os usuários de conexão direta B2B.

### <a name="example-6-application-owners-as-reviewers"></a>Exemplo 6: proprietários de aplicativos como revisadores

```http
"reviewers": [
    {
        "query": "/servicePrincipals/{id}/owners",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="next-steps"></a>Próximas etapas

+ [Configurar o escopo de sua definição de revisão de acesso](/graph/accessreviews-scope-concept)
+ [Experimente tutoriais para](/graph/accessreviews-overview) saber como usar a API de avaliações de acesso para revisar o acesso aos recursos do Azure AD
+ [Criar uma revisão de acesso](/azure/active-directory/governance/create-access-review)