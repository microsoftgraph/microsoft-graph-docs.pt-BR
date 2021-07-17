---
title: Criar accessReviewScheduleDefinition
description: Crie um novo objeto accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1644621bfff2d33347204256a9c76a5c17129b54
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440505"
---
# <a name="create-accessreviewscheduledefinition"></a><span data-ttu-id="10a2e-103">Criar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="10a2e-103">Create accessReviewScheduleDefinition</span></span>

<span data-ttu-id="10a2e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10a2e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="10a2e-105">Crie um novo [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="10a2e-105">Create a new [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="10a2e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="10a2e-106">Permissions</span></span>

<span data-ttu-id="10a2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10a2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10a2e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10a2e-109">Permission type</span></span>                        | <span data-ttu-id="10a2e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10a2e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="10a2e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10a2e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="10a2e-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10a2e-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="10a2e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10a2e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10a2e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10a2e-114">Not supported.</span></span>|
|<span data-ttu-id="10a2e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10a2e-115">Application</span></span>                            | <span data-ttu-id="10a2e-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10a2e-116">AccessReview.ReadWrite.All</span></span> |

<span data-ttu-id="10a2e-117">O usuário interno também deve estar em uma função de diretório que permita que ele crie uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="10a2e-117">The signed-in user must also be in a directory role that permits them to create an access review.</span></span>  <span data-ttu-id="10a2e-118">Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviewsv2-root.md)</span><span class="sxs-lookup"><span data-stu-id="10a2e-118">For more details, see the role and permission requirements for [access reviews](../resources/accessreviewsv2-root.md).</span></span>

## <a name="http-request"></a><span data-ttu-id="10a2e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10a2e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a><span data-ttu-id="10a2e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10a2e-120">Request headers</span></span>
| <span data-ttu-id="10a2e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="10a2e-121">Name</span></span>         | <span data-ttu-id="10a2e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="10a2e-122">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="10a2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="10a2e-123">Authorization</span></span>|<span data-ttu-id="10a2e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10a2e-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="10a2e-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="10a2e-126">Content-type</span></span> | <span data-ttu-id="10a2e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10a2e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10a2e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10a2e-129">Request body</span></span>
<span data-ttu-id="10a2e-130">No corpo da solicitação, fornece uma representação JSON de [um objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="10a2e-130">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="10a2e-131">A tabela a seguir mostra as propriedades aceitas para criar um accessReview.</span><span class="sxs-lookup"><span data-stu-id="10a2e-131">The following table shows the properties accepted to create an accessReview.</span></span>

| <span data-ttu-id="10a2e-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10a2e-132">Property</span></span> | <span data-ttu-id="10a2e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="10a2e-133">Type</span></span> | <span data-ttu-id="10a2e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="10a2e-134">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="10a2e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="10a2e-135">displayName</span></span> | <span data-ttu-id="10a2e-136">String</span><span class="sxs-lookup"><span data-stu-id="10a2e-136">String</span></span> | <span data-ttu-id="10a2e-137">Nome da série de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="10a2e-137">Name of access review series.</span></span> <span data-ttu-id="10a2e-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10a2e-138">Required.</span></span>|
| <span data-ttu-id="10a2e-139">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="10a2e-139">descriptionForAdmins</span></span> | <span data-ttu-id="10a2e-140">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10a2e-140">string</span></span> | <span data-ttu-id="10a2e-141">Contexto da revisão fornecida aos administradores.</span><span class="sxs-lookup"><span data-stu-id="10a2e-141">Context of the review provided to admins.</span></span> <span data-ttu-id="10a2e-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10a2e-142">Required.</span></span> |
  <span data-ttu-id="10a2e-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="10a2e-143">descriptionForReviewers</span></span> | <span data-ttu-id="10a2e-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10a2e-144">string</span></span> | <span data-ttu-id="10a2e-145">Contexto da revisão fornecida aos revisadores.</span><span class="sxs-lookup"><span data-stu-id="10a2e-145">Context of the review provided to reviewers.</span></span> <span data-ttu-id="10a2e-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10a2e-146">Required.</span></span> |
| <span data-ttu-id="10a2e-147">scope</span><span class="sxs-lookup"><span data-stu-id="10a2e-147">scope</span></span> | [<span data-ttu-id="10a2e-148">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="10a2e-148">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="10a2e-149">Define o escopo dos usuários revisados em um grupo.</span><span class="sxs-lookup"><span data-stu-id="10a2e-149">Defines the scope of users reviewed in a group.</span></span> <span data-ttu-id="10a2e-150">Consulte [accessReviewScope](../resources/accessreviewscheduledefinition.md) e também saiba como [configurar o escopo da sua definição de revisão de acesso.](/graph/accessreviews-scope-concept)</span><span class="sxs-lookup"><span data-stu-id="10a2e-150">See  [accessReviewScope](../resources/accessreviewscheduledefinition.md) and also learn how to [configure the scope of your access review definition](/graph/accessreviews-scope-concept).</span></span> <span data-ttu-id="10a2e-151">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10a2e-151">Required.</span></span>| 
| <span data-ttu-id="10a2e-152">instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="10a2e-152">instanceEnumerationScope</span></span> | [<span data-ttu-id="10a2e-153">accessReviewScope</span><span class="sxs-lookup"><span data-stu-id="10a2e-153">accessReviewScope</span></span>](../resources/accessreviewscope.md) | <span data-ttu-id="10a2e-154">No caso de uma revisão de todos os grupos, isso determina o escopo de quais grupos serão revisados.</span><span class="sxs-lookup"><span data-stu-id="10a2e-154">In the case of an all groups review, this determines the scope of which groups will be reviewed.</span></span> <span data-ttu-id="10a2e-155">Consulte [accessReviewScope](../resources/accessreviewscheduledefinition.md) e também saiba como [configurar o escopo da sua definição de revisão de acesso.](/graph/accessreviews-scope-concept)</span><span class="sxs-lookup"><span data-stu-id="10a2e-155">See [accessReviewScope](../resources/accessreviewscheduledefinition.md) and also learn how to [configure the scope of your access review definition](/graph/accessreviews-scope-concept).</span></span>| 
| <span data-ttu-id="10a2e-156">settings</span><span class="sxs-lookup"><span data-stu-id="10a2e-156">settings</span></span> | [<span data-ttu-id="10a2e-157">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="10a2e-157">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md)| <span data-ttu-id="10a2e-158">As configurações de uma série de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="10a2e-158">The settings for an access review series.</span></span> <span data-ttu-id="10a2e-159">A recorrência é determinada aqui.</span><span class="sxs-lookup"><span data-stu-id="10a2e-159">Recurrence is determined here.</span></span> <span data-ttu-id="10a2e-160">Consulte [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="10a2e-160">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="10a2e-161">revisadores</span><span class="sxs-lookup"><span data-stu-id="10a2e-161">reviewers</span></span> | <span data-ttu-id="10a2e-162">[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="10a2e-162">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span> | <span data-ttu-id="10a2e-163">Define quem são os revisadores.</span><span class="sxs-lookup"><span data-stu-id="10a2e-163">Defines who the reviewers are.</span></span> <span data-ttu-id="10a2e-164">Se nenhum for especificado, a revisão será uma autoavaliação (os usuários revisados analisam seu próprio acesso).</span><span class="sxs-lookup"><span data-stu-id="10a2e-164">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="10a2e-165">Consulte [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="10a2e-165">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |
|<span data-ttu-id="10a2e-166">fallbackReviewers</span><span class="sxs-lookup"><span data-stu-id="10a2e-166">fallbackReviewers</span></span>|<span data-ttu-id="10a2e-167">[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="10a2e-167">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="10a2e-168">Se fornecido, os revisadores de fallback serão solicitados a concluir uma revisão se os revistores primários não existirem.</span><span class="sxs-lookup"><span data-stu-id="10a2e-168">If provided, the fallback reviewers are asked to complete a review if the primary reviewers do not exist.</span></span> <span data-ttu-id="10a2e-169">Por exemplo, se os gerentes forem selecionados como e uma entidade em revisão não tiver um gerente no Azure AD, os revisadores de fallback serão solicitados a revisar `reviewers` essa entidade.</span><span class="sxs-lookup"><span data-stu-id="10a2e-169">For example, if managers are selected as `reviewers` and a principal under review does not have a manager in Azure AD, the fallback reviewers are asked to review that principal.</span></span>|

## <a name="response"></a><span data-ttu-id="10a2e-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="10a2e-170">Response</span></span>
<span data-ttu-id="10a2e-171">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10a2e-171">If successful, this method returns a `201 Created` response code and an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10a2e-172">Exemplos</span><span class="sxs-lookup"><span data-stu-id="10a2e-172">Examples</span></span>

### <a name="example-1-create-an-access-review-on-a-group"></a><span data-ttu-id="10a2e-173">Exemplo 1: Criar uma revisão de acesso em um grupo</span><span class="sxs-lookup"><span data-stu-id="10a2e-173">Example 1: Create an access review on a group</span></span>

<span data-ttu-id="10a2e-174">Este é um exemplo de criação de uma revisão de acesso com as seguintes configurações:</span><span class="sxs-lookup"><span data-stu-id="10a2e-174">This is an example of creating an access review with the following settings:</span></span>
+ <span data-ttu-id="10a2e-175">A revisão revisa todos os membros de um grupo, cuja **id de grupo** é `02f3bafb-448c-487c-88c2-5fd65ce49a41` .</span><span class="sxs-lookup"><span data-stu-id="10a2e-175">The review reviews all members of a group, whose group **id** is `02f3bafb-448c-487c-88c2-5fd65ce49a41`.</span></span>
+ <span data-ttu-id="10a2e-176">Um usuário específico, cuja **id de usuário** `398164b1-5196-49dd-ada2-364b49f99b27` é o revistor.</span><span class="sxs-lookup"><span data-stu-id="10a2e-176">A specific user, whose user **id** is `398164b1-5196-49dd-ada2-364b49f99b27` is the reviewer.</span></span>
+ <span data-ttu-id="10a2e-177">Ela se recursa semanalmente e continua indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="10a2e-177">It recurs weekly and continues indefinitely.</span></span>

#### <a name="request"></a><span data-ttu-id="10a2e-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10a2e-178">Request</span></span>
<span data-ttu-id="10a2e-179">No corpo da solicitação, fornece uma representação JSON do [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="10a2e-179">In the request body, supply a JSON representation of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="10a2e-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="10a2e-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Test create",
  "descriptionForAdmins": "New scheduled access review",
  "descriptionForReviewers": "If you have any questions, contact jerry@contoso.com",
  "scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [
    {
      "query": "/users/398164b1-5196-49dd-ada2-364b49f99b27",
      "queryType": "MicrosoftGraph"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 1,
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
# <a name="c"></a>[<span data-ttu-id="10a2e-181">C#</span><span class="sxs-lookup"><span data-stu-id="10a2e-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10a2e-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10a2e-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10a2e-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10a2e-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10a2e-184">Java</span><span class="sxs-lookup"><span data-stu-id="10a2e-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="10a2e-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="10a2e-185">Response</span></span>
><span data-ttu-id="10a2e-186">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10a2e-186">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "userPrincipalName": "admin@contoso.com"
  },
  "scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
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

### <a name="example-2-create-an-access-review-on-all-teams-with-inactive-guest-users"></a><span data-ttu-id="10a2e-187">Exemplo 2: Criar uma revisão de acesso em todas as equipes com usuários convidados inativos</span><span class="sxs-lookup"><span data-stu-id="10a2e-187">Example 2: Create an access review on all teams with inactive guest users</span></span>

<span data-ttu-id="10a2e-188">Este é um exemplo de criação de uma revisão de acesso com as seguintes configurações:</span><span class="sxs-lookup"><span data-stu-id="10a2e-188">This is an example of creating an access review with the following settings:</span></span>
+ <span data-ttu-id="10a2e-189">A revisão revisa todas as equipes com usuários convidados inativos.</span><span class="sxs-lookup"><span data-stu-id="10a2e-189">The review reviews all teams with inactive guest users.</span></span> <span data-ttu-id="10a2e-190">O período de inatividade é de 30 dias a partir da data de início da revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="10a2e-190">The period of inactivity is 30 days from the start date of the access review.</span></span>
+ <span data-ttu-id="10a2e-191">Os proprietários do grupo são os revisadores e os revisadores de fallback são atribuídos.</span><span class="sxs-lookup"><span data-stu-id="10a2e-191">The group owners are the reviewers and fallback reviewers are assigned.</span></span>
+ <span data-ttu-id="10a2e-192">Ela se recorre no terceiro dia de cada trimestre e continua indefinidamente.</span><span class="sxs-lookup"><span data-stu-id="10a2e-192">It recurs on the third day of every quarter and continues indefinitely.</span></span>
+ <span data-ttu-id="10a2e-193">**autoApplyDecisionsEnabled** é definido como `true` com **o defaultDecision** definido como `Deny` .</span><span class="sxs-lookup"><span data-stu-id="10a2e-193">**autoApplyDecisionsEnabled** is set to `true` with the **defaultDecision** set to `Deny`.</span></span>

#### <a name="request"></a><span data-ttu-id="10a2e-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10a2e-194">Request</span></span>
<span data-ttu-id="10a2e-195">No corpo da solicitação, fornece uma representação JSON do [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="10a2e-195">In the request body, supply a JSON representation of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="10a2e-196">HTTP</span><span class="sxs-lookup"><span data-stu-id="10a2e-196">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition_inactiveguests_M365"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Review inactive guests on teams",
  "descriptionForAdmins": "Control guest user access to our teams.",
  "descriptionForReviewers": "Information security is everyone's responsibility. Review our access policy for more.",
  "instanceEnumerationScope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
  },
  "scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
    },
  "reviewers": [
    {
      "query": "./owners",
      "queryType": "MicrosoftGraph"
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
      "queryType": "MicrosoftGraph"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "recommendationsEnabled": true,
    "instanceDurationInDays": 3,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "dayOfMonth": 5,
        "interval": 3
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-05-04T00:00:00.000Z"
      }
    },
    "defaultDecisionEnabled": true,
    "defaultDecision": "Deny",
    "autoApplyDecisionsEnabled": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="10a2e-197">C#</span><span class="sxs-lookup"><span data-stu-id="10a2e-197">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-inactiveguests-m365-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10a2e-198">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10a2e-198">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-inactiveguests-m365-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10a2e-199">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10a2e-199">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-inactiveguests-m365-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10a2e-200">Java</span><span class="sxs-lookup"><span data-stu-id="10a2e-200">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-inactiveguests-m365-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="10a2e-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="10a2e-201">Response</span></span>
><span data-ttu-id="10a2e-202">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10a2e-202">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions/$entity",
  "id": "b0966e21-a01e-43c9-8f8b-9ba30ed5710a",
  "displayName": "Review inactive guests on teams",
  "createdDateTime": "2021-05-04T18:27:02.6719849Z",
  "lastModifiedDateTime": "2021-05-04T18:27:24.0889623Z",
  "status": "InProgress",
  "descriptionForAdmins": "Control guest user access to our teams.",
  "descriptionForReviewers": "Information security is everyone's responsibility. Review our access policy for more.",
  "createdBy": {
    "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
    "displayName": "MOD Administrator",
    "userPrincipalName": "admin@contoso.com"
  },
  "scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "queryRoot": null,
    "inactiveDuration": "P30D"
  },
  "instanceEnumerationScope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team'))&$count=true",
    "queryType": "MicrosoftGraph",
    "queryRoot": null
  },
  "reviewers": [
    {
      "query": "./owners",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "backupReviewers": [
    {
      "query": "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": true,
    "defaultDecision": "Deny",
    "instanceDurationInDays": 3,
    "autoApplyDecisionsEnabled": true,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "interval": 3,
        "month": 0,
        "dayOfMonth": 0,
        "daysOfWeek": [],
        "firstDayOfWeek": "sunday",
        "index": "first"
      },
      "range": {
        "type": "numbered",
        "numberOfOccurrences": 0,
        "recurrenceTimeZone": null,
        "startDate": "2021-05-05",
        "endDate": "9999-12-31"
      }
    },
    "applyActions": [
      {
        "@odata.type": "#microsoft.graph.removeAccessApplyAction"
      }
    ]
  }
}
```

### <a name="example-3-create-an-access-review-of-all-users-to-an-application"></a><span data-ttu-id="10a2e-203">Exemplo 3: Criar uma revisão de acesso de todos os usuários para um aplicativo</span><span class="sxs-lookup"><span data-stu-id="10a2e-203">Example 3: Create an access review of all users to an application</span></span>

<span data-ttu-id="10a2e-204">Este é um exemplo de criação de uma revisão de acesso com as seguintes configurações:</span><span class="sxs-lookup"><span data-stu-id="10a2e-204">This is an example of creating an access review with the following settings:</span></span>
+ <span data-ttu-id="10a2e-205">A revisão revisa o acesso do usuário a um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="10a2e-205">The review reviews user access to an application.</span></span>
+ <span data-ttu-id="10a2e-206">Os gerentes de pessoas são revisadores e revisadores de fallback são membros de um grupo.</span><span class="sxs-lookup"><span data-stu-id="10a2e-206">The people managers are the reviewers and fallback reviewers are the members of a group.</span></span>
+ <span data-ttu-id="10a2e-207">Ela recorre semesanuais e termina 1 ano a partir do startDate.</span><span class="sxs-lookup"><span data-stu-id="10a2e-207">It recurs semi-annually and ends 1 year from the startDate.</span></span>

#### <a name="request"></a><span data-ttu-id="10a2e-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10a2e-208">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="10a2e-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="10a2e-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition_allusers_M365_AADRole"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Review employee access to LinkedIn",
  "descriptionForAdmins": "Review employee access to LinkedIn",
  "scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/users",
        "queryType": "MicrosoftGraph"
      }
    ],
    "resourceScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/servicePrincipals/bae11f90-7d5d-46ba-9f55-8112b59d92ae",
        "queryType": "MicrosoftGraph"
      }
    ]
  },
  "reviewers": [
    {
      "query": "./manager",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "backupReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph"
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": true,
    "defaultDecision": "Recommendation",
    "instanceDurationInDays": 180,
    "autoApplyDecisionsEnabled": true,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "interval": 6,
        "dayOfMonth": 0
      },
      "range": {
        "type": "numbered",
        "startDate": "2021-05-05",
        "endDate": "2022-05-05"
      }
    }
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="10a2e-210">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10a2e-210">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-allusers-m365-aadrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="10a2e-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="10a2e-211">Response</span></span>
><span data-ttu-id="10a2e-212">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10a2e-212">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions/$entity",
  "id": "1f79f34b-8667-40d9-875c-893b630b3dec",
  "scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/users",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
      }
    ],
    "resourceScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/servicePrincipals/bae11f90-7d5d-46ba-9f55-8112b59d92ae",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
      }
    ]
  },
  "reviewers": [
    {
      "query": "./manager",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "backupReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "settings": {
    "instanceDurationInDays": 180,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "interval": 6,
        "month": 0,
        "dayOfMonth": 0,
        "daysOfWeek": [],
        "firstDayOfWeek": "sunday",
        "index": "first"
      },
      "range": {
        "type": "numbered",
        "numberOfOccurrences": 0,
        "recurrenceTimeZone": null,
        "startDate": "2021-05-05",
        "endDate": "2022-05-05"
      }
    }
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
