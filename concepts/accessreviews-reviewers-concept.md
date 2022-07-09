---
title: Atribuir revisores à sua revisão de acesso usando o Microsoft API do Graph
description: Use a API de revisões de acesso no Microsoft Graph para atribuir revisores de acesso, como usuários específicos, membros ou proprietários de um grupo, gerentes de pessoas ou proprietários de aplicativos.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: ce0e806920b2bb925cc16b7d31aa57156388935a
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698342"
---
# <a name="assign-reviewers-to-your-access-review-using-the-microsoft-graph-api"></a>Atribuir revisores à sua revisão de acesso usando o Microsoft API do Graph

A Azure AD [api](/graph/api/resources/accessreviewsv2-overview) de revisões de acesso permite que você examine programaticamente o acesso que os usuários, entidades de serviço ou grupos têm aos seus Azure AD recursos.

Os revisores principais são configurados na propriedade **reviewers** do recurso [accessReviewScheduleDefinition de revisões de](/graph/api/resources/accessreviewscheduledefinition) acesso.  Além disso, você pode especificar revisores de fallback usando a **propriedade fallbackReviewers** . Essas propriedades não são necessárias quando você cria uma auto-revisão (em que os usuários revisam seu próprio acesso).

Para configurar os revisores e revisores de fallback, defina os valores das propriedades **query**, **queryRoot** e **queryType** de **accessReviewReviewerScope**. Para obter descrições dessas propriedades, consulte o [tipo de recurso accessReviewReviewerScope](/graph/api/resources/accessreviewreviewerscope) .

## <a name="example-1-a-self-review"></a>Exemplo 1: uma auto-revisão

```http
"reviewers": []
```

Para configurar uma auto-revisão, não especifique a propriedade **dos revisores** ou forneça um objeto vazio para a propriedade.

Se o escopo de revisão  de acesso correspondente tiver como alvo usuários do B2B Direct Connect e equipes com canais compartilhados, o proprietário da equipe será atribuído para examinar o acesso dos usuários do B2B Direct Connect.

## <a name="example-2-a-specific-user-as-the-reviewer"></a>Exemplo 2: um usuário específico como revistor

```http
"reviewers": [
    {
        "query": "/users/{user id}",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="example-3-members-of-a-group-as-reviewers"></a>Exemplo 3: Membros de um grupo como revisores

```http
"reviewers": [
    {
        "query": "/groups/{group id}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="example-4-group-owners-as-reviewers"></a>Exemplo 4: Proprietários de grupo como revisores
```http
"reviewers": [
    {
        "query": "./owners",
        "queryType": "MicrosoftGraph"
    }
]
```

Para atribuir apenas os proprietários do grupo de um país específico como revisores:

```http
"reviewers": [
    {
        "query": "/groups/{group id}/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq 'USA'",
        "type": "MicrosoftGraph”
    }
]
```

## <a name="example-5-people-managers-as-reviewers"></a>Exemplo 5: Gerentes de pessoas como revisores

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```

Como `./manager` é uma consulta relativa, especifique **a propriedade queryRoot** com o valor `decisions`.

Se o escopo de revisão  de acesso correspondente tiver como alvo usuários do B2B Direct Connect e equipes com canais compartilhados, o proprietário da equipe será atribuído para examinar o acesso dos usuários do B2B Direct Connect.

## <a name="example-6-application-owners-as-reviewers"></a>Exemplo 6: Proprietários de aplicativos como revisores

```http
"reviewers": [
    {
        "query": "/servicePrincipals/{id}/owners",
        "queryType": "MicrosoftGraph"
    }
]
```

## <a name="next-steps"></a>Próximas etapas

+ [Configurar o escopo da definição de revisão de acesso](/graph/accessreviews-scope-concept)
+ [Experimente tutoriais para](/graph/accessreviews-overview) saber como usar a API de revisões de acesso para examinar o acesso a Azure AD recursos
+ [Criar uma revisão de acesso](/azure/active-directory/governance/create-access-review)
