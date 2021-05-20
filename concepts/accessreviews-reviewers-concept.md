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
# <a name="assign-reviewers-to-your-access-review-definition-using-the-microsoft-graph-api"></a><span data-ttu-id="27c4c-103">Atribuir revisadores à sua definição de revisão de acesso usando a API Graph Microsoft</span><span class="sxs-lookup"><span data-stu-id="27c4c-103">Assign reviewers to your access review definition using the Microsoft Graph API</span></span>

<span data-ttu-id="27c4c-104">A [API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) de revisões de acesso do Azure AD permite que você revise programaticamente o acesso que os usuários, entidades de serviço ou grupos têm aos recursos do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="27c4c-104">The Azure AD [access reviews API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) allows you to programmatically review the access that users, service principals, or groups have to your Azure AD resources.</span></span>

> [!NOTE]
> <span data-ttu-id="27c4c-105">No momento, a API de [críticas](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) de acesso está disponível apenas no ponto de extremidade do Microsoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="27c4c-105">The [access reviews API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) is currently available in only the Microsoft Graph beta endpoint.</span></span> <span data-ttu-id="27c4c-106">Não o use em aplicativos de produção, pois ele está sujeito a alterações sem aviso prévio.</span><span class="sxs-lookup"><span data-stu-id="27c4c-106">Do not use it in production apps, as it is subject to change without notice.</span></span>

<span data-ttu-id="27c4c-107">Os revisores primários são configurados na propriedade **reviewers** do recurso [access Reviews accessReviewScheduleDefinition.](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="27c4c-107">The primary reviewers are configured in the **reviewers** property of the access reviews [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true) resource.</span></span>  <span data-ttu-id="27c4c-108">Além disso, você pode especificar revisores de fallback usando **a propriedade fallbackReviewers.**</span><span class="sxs-lookup"><span data-stu-id="27c4c-108">In addition, you can specify fallback reviewers by using **fallbackReviewers** property.</span></span> <span data-ttu-id="27c4c-109">Essas propriedades não são necessárias ao criar uma auto-revisão (onde os usuários revisam seu próprio acesso).</span><span class="sxs-lookup"><span data-stu-id="27c4c-109">These properties are not required when you create a self-review (where users review their own access).</span></span>

## <a name="configure-reviewers"></a><span data-ttu-id="27c4c-110">Configurar revisadores</span><span class="sxs-lookup"><span data-stu-id="27c4c-110">Configure reviewers</span></span>

<span data-ttu-id="27c4c-111">Para configurar os revisores e revisores de fallback, de definir os valores das propriedades **query**, **queryRoot** e **queryType** **do accessReviewReviewerScope**.</span><span class="sxs-lookup"><span data-stu-id="27c4c-111">To configure the reviewers and fallback reviewers, set the values of **query**, **queryRoot**, and **queryType** properties of **accessReviewReviewerScope**.</span></span> <span data-ttu-id="27c4c-112">Para descrições dessas propriedades, consulte [tipo de recurso accessReviewReviewerScope.](/graph/api/resources/accessreviewreviewerscope?view=graph-rest-beta&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="27c4c-112">For descriptions of these properties, see [accessReviewReviewerScope](/graph/api/resources/accessreviewreviewerscope?view=graph-rest-beta&preserve-view=true) resource type.</span></span>

### <a name="example-1-a-specific-user-as-the-reviewer"></a><span data-ttu-id="27c4c-113">Exemplo 1: um usuário específico como revistor</span><span class="sxs-lookup"><span data-stu-id="27c4c-113">Example 1: A specific user as the reviewer</span></span>

```http
"reviewers": [
    {
        "query": "/users/{user id}",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-2-members-of-a-group-as-reviewers"></a><span data-ttu-id="27c4c-114">Exemplo 2: Membros de um grupo como revisadores</span><span class="sxs-lookup"><span data-stu-id="27c4c-114">Example 2: Members of a group as reviewers</span></span>

```http
"reviewers": [
    {
        "query": "/groups/{group id}}/transitiveMembers",
        "queryType": "MicrosoftGraph"
    }
]
```

### <a name="example-3-group-owners-as-reviewers"></a><span data-ttu-id="27c4c-115">Exemplo 3: Proprietários do grupo como revisadores</span><span class="sxs-lookup"><span data-stu-id="27c4c-115">Example 3: Group owners as reviewers</span></span>
```http
"reviewers": [
    {
        "query": "./owners",
        "queryType": "MicrosoftGraph"
    }
]
```

<span data-ttu-id="27c4c-116">Para atribuir apenas os proprietários do grupo de um país específico como revisadores:</span><span class="sxs-lookup"><span data-stu-id="27c4c-116">To assign only the group owners from a specific country as reviewers:</span></span>

```http
"reviewers": [
    {
        "query": "/groups/{group id}/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq 'USA'",
        "type": "MicrosoftGraph”
    }
]
```

### <a name="example-4-people-managers-as-reviewers"></a><span data-ttu-id="27c4c-117">Exemplo 4: Gerentes de pessoas como revisadores</span><span class="sxs-lookup"><span data-stu-id="27c4c-117">Example 4: People managers as reviewers</span></span>

```http
"reviewers": [
    {
        "query": "./manager",
        "queryType": "MicrosoftGraph",
        "queryRoot": "decisions"
    }
]
```
<span data-ttu-id="27c4c-118">Como `./manager` é uma consulta relativa, especifique a propriedade **queryRoot** com o valor `decisions` .</span><span class="sxs-lookup"><span data-stu-id="27c4c-118">Because `./manager` is a relative query, specify the **queryRoot** property with the value `decisions`.</span></span>

## <a name="see-also"></a><span data-ttu-id="27c4c-119">Confira também</span><span class="sxs-lookup"><span data-stu-id="27c4c-119">See also</span></span>

+ [<span data-ttu-id="27c4c-120">Configurar o escopo de sua definição de revisão de acesso</span><span class="sxs-lookup"><span data-stu-id="27c4c-120">Configure the scope of your access review definition</span></span>](/graph/accessreviews-scope-concept)
