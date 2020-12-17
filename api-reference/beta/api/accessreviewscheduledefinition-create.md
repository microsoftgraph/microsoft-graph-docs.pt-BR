---
title: Criar accessReviewScheduleDefinition
description: Criar um novo objeto accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b9308111bdad2482b71339333822d7878d3187f
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705706"
---
# <a name="create-accessreviewscheduledefinition"></a><span data-ttu-id="87a1b-103">Criar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="87a1b-103">Create accessReviewScheduleDefinition</span></span>

<span data-ttu-id="87a1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87a1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87a1b-105">Criar um novo objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="87a1b-105">Create a new [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="87a1b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87a1b-106">Permissions</span></span>

<span data-ttu-id="87a1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87a1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87a1b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87a1b-109">Permission type</span></span>                        | <span data-ttu-id="87a1b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87a1b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="87a1b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87a1b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="87a1b-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87a1b-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="87a1b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87a1b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87a1b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87a1b-114">Not supported.</span></span>|
|<span data-ttu-id="87a1b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87a1b-115">Application</span></span>                            | <span data-ttu-id="87a1b-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87a1b-116">AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="87a1b-117">O usuário conectado também deve estar em uma função de diretório que permite que eles criem uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="87a1b-117">The signed-in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="87a1b-118">Para obter mais detalhes, consulte a função e os requisitos de permissão para [revisões do Access](../resources/accessreviewsv2-root.md).</span><span class="sxs-lookup"><span data-stu-id="87a1b-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="87a1b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87a1b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="87a1b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87a1b-120">Request headers</span></span>
| <span data-ttu-id="87a1b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="87a1b-121">Name</span></span>         | <span data-ttu-id="87a1b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="87a1b-122">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="87a1b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="87a1b-123">Authorization</span></span>|<span data-ttu-id="87a1b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87a1b-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="87a1b-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="87a1b-126">Content-type</span></span> | <span data-ttu-id="87a1b-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87a1b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87a1b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87a1b-129">Request body</span></span>
<span data-ttu-id="87a1b-130">No corpo da solicitação, forneça uma representação JSON de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="87a1b-130">In the request body, supply a JSON representation of an [accessReview](../resources/accessreview.md) object.</span></span>

<span data-ttu-id="87a1b-131">A tabela a seguir mostra as propriedades aceitas para criar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="87a1b-131">The following table shows the properties accepted to create an accessReview.</span></span>

| <span data-ttu-id="87a1b-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87a1b-132">Property</span></span> | <span data-ttu-id="87a1b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="87a1b-133">Type</span></span> | <span data-ttu-id="87a1b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="87a1b-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="87a1b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="87a1b-135">displayName</span></span> | <span data-ttu-id="87a1b-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87a1b-136">String</span></span> | <span data-ttu-id="87a1b-137">Nome da série de revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="87a1b-137">Name of access review series.</span></span> <span data-ttu-id="87a1b-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87a1b-138">Required.</span></span>|
| <span data-ttu-id="87a1b-139">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="87a1b-139">descriptionForAdmins</span></span> | <span data-ttu-id="87a1b-140">string</span><span class="sxs-lookup"><span data-stu-id="87a1b-140">string</span></span> | <span data-ttu-id="87a1b-141">Contexto da revisão fornecida aos administradores.</span><span class="sxs-lookup"><span data-stu-id="87a1b-141">Context of the review provided to admins.</span></span> <span data-ttu-id="87a1b-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87a1b-142">Required.</span></span> |
  <span data-ttu-id="87a1b-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="87a1b-143">descriptionForReviewers</span></span> | <span data-ttu-id="87a1b-144">string</span><span class="sxs-lookup"><span data-stu-id="87a1b-144">string</span></span> | <span data-ttu-id="87a1b-145">Contexto da revisão fornecida aos revisores.</span><span class="sxs-lookup"><span data-stu-id="87a1b-145">Context of the review provided to reviewers.</span></span> <span data-ttu-id="87a1b-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87a1b-146">Required.</span></span> |
| <span data-ttu-id="87a1b-147">escopo</span><span class="sxs-lookup"><span data-stu-id="87a1b-147">scope</span></span> | [<span data-ttu-id="87a1b-148">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="87a1b-148">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="87a1b-149">Define o escopo dos usuários revisados em um grupo.</span><span class="sxs-lookup"><span data-stu-id="87a1b-149">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="87a1b-150">Consulte  [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="87a1b-150">See  [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="87a1b-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87a1b-151">Required.</span></span>| 
| <span data-ttu-id="87a1b-152">instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="87a1b-152">instanceEnumerationScope</span></span> | [<span data-ttu-id="87a1b-153">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="87a1b-153">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="87a1b-154">No caso de uma revisão todos os grupos, isso determina o escopo de quais grupos serão revisados.</span><span class="sxs-lookup"><span data-stu-id="87a1b-154">In the case of an all groups review, this determines the scope of which groups will be reviewed.</span></span> <span data-ttu-id="87a1b-155">Consulte [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="87a1b-155">See [accessReviewScope](../resources/accessreviewscheduledefinition.md).</span></span> | 
| <span data-ttu-id="87a1b-156">settings</span><span class="sxs-lookup"><span data-stu-id="87a1b-156">settings</span></span> | [<span data-ttu-id="87a1b-157">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="87a1b-157">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md)| <span data-ttu-id="87a1b-158">As configurações para uma série de análise do Access.</span><span class="sxs-lookup"><span data-stu-id="87a1b-158">The settings for an access review series.</span></span> <span data-ttu-id="87a1b-159">A recorrência é determinada aqui.</span><span class="sxs-lookup"><span data-stu-id="87a1b-159">Recurrence is determined here.</span></span> <span data-ttu-id="87a1b-160">Consulte [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="87a1b-160">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="87a1b-161">revisores</span><span class="sxs-lookup"><span data-stu-id="87a1b-161">reviewers</span></span> | <span data-ttu-id="87a1b-162">coleção [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="87a1b-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span> | <span data-ttu-id="87a1b-163">Define quem é os revisores.</span><span class="sxs-lookup"><span data-stu-id="87a1b-163">Defines who the reviewers are.</span></span> <span data-ttu-id="87a1b-164">Se nenhum for especificado, a revisão será uma autorevisão (os usuários revisaram revisar seu próprio acesso).</span><span class="sxs-lookup"><span data-stu-id="87a1b-164">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="87a1b-165">Consulte [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="87a1b-165">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |


## <a name="response"></a><span data-ttu-id="87a1b-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="87a1b-166">Response</span></span>
<span data-ttu-id="87a1b-167">Se tiver êxito, este método retornará um `201, Created` código de resposta e um objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87a1b-167">If successful, this method returns a `201, Created` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87a1b-168">Exemplos</span><span class="sxs-lookup"><span data-stu-id="87a1b-168">Examples</span></span>

<span data-ttu-id="87a1b-169">Este é um exemplo de criação de uma série de revisão do Access com um usuário específico, cuja ID de objeto do usuário é 7eae4444-D425-48b2-adf2-3c777f6256f3, como o revisor.</span><span class="sxs-lookup"><span data-stu-id="87a1b-169">This is an example of creating an access review series with a specific user, whose user object id is 7eae4444-d425-48b2-adf2-3c777f6256f3, as the reviewer.</span></span> <span data-ttu-id="87a1b-170">A revisão revisa todos os membros de um grupo específico, cuja ID de objeto do grupo é b7a059cb-038a-4802-8fc9-b9d1ed0c4444.</span><span class="sxs-lookup"><span data-stu-id="87a1b-170">The review reviews all members of a specific group, whose group object id is b7a059cb-038a-4802-8fc9-b9d1ed0c4444.</span></span> <span data-ttu-id="87a1b-171">Ele se repete semanalmente.</span><span class="sxs-lookup"><span data-stu-id="87a1b-171">It recurs weekly.</span></span>

### <a name="request"></a><span data-ttu-id="87a1b-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87a1b-172">Request</span></span>
<span data-ttu-id="87a1b-173">No corpo da solicitação, forneça uma representação JSON do objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="87a1b-173">In the request body, supply a JSON representation of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="87a1b-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="87a1b-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Test create",
  "descriptionForAdmins": "New scheduled access review",
  "descriptionForReviewers": "If you have any questions, contact jerry@contoso.com",
  "scope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0c4444/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [
    {
      "query": "/users/7eae4444-d425-48b2-adf2-3c777f6256f3",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 1,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-08T12:02:30.667Z"
      }
    }
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="87a1b-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87a1b-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="87a1b-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="87a1b-176">Response</span></span>
><span data-ttu-id="87a1b-p113">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87a1b-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "29f2d16e-9ca6-4052-bbfe-802c48944448",
    "displayName": "Test create",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "lastModifiedDateTime": "0001-01-01T00:00:00Z",
    "status": "NotStarted",
    "descriptionForAdmins": "Test create",
    "descriptionForReviewers": "Test create",
    "instanceEnumerationScope": null,
    "createdBy": {
        "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@microsoft.com"
    },
    "scope": {
        "query": "/groups/b74444cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "/users/7eae986b-d425-48b2-adf2-3c777f4444f3",
            "queryType": "MicrosoftGraph",
            "queryRoot": "decisions"
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 1,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "weekly",
                "interval": 1,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "noEnd",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2020-09-08",
                "endDate": null
            }
        },
        "applyActions": []
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
