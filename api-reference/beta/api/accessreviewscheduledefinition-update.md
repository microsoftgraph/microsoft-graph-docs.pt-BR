---
title: Atualizar accessReviewScheduleDefinition
description: Atualize um objeto accessReviewScheduleDefinition existente para alterar uma ou mais de suas propriedades.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6d03271d78dea64edf1c410a4bf30886c3e13603
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439013"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="fb97f-103">Atualizar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="fb97f-103">Update accessReviewScheduleDefinition</span></span>

<span data-ttu-id="fb97f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb97f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb97f-105">Atualize um [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) existente para alterar uma ou mais de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="fb97f-105">Update an existing [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object to change one or more of its properties.</span></span>

>[!NOTE]
><span data-ttu-id="fb97f-106">Todas as atualizações feitas em um accessReviewScheduleDefinition só se aplicam a instâncias futuras.</span><span class="sxs-lookup"><span data-stu-id="fb97f-106">Any updates made to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="fb97f-107">As instâncias em execução no momento não podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="fb97f-107">Currently running instances cannot be updated.</span></span>
><span data-ttu-id="fb97f-108">Além disso, essa API não se destina a atualizar propriedades, incluindo decisões, no nível accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="fb97f-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="fb97f-109">Consulte [accessReviewInstance para](../resources/accessreviewinstance.md) obter mais informações sobre instâncias.</span><span class="sxs-lookup"><span data-stu-id="fb97f-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb97f-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="fb97f-110">Permissions</span></span>
<span data-ttu-id="fb97f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb97f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb97f-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fb97f-113">Permission type</span></span>                        | <span data-ttu-id="fb97f-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fb97f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb97f-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fb97f-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb97f-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb97f-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="fb97f-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fb97f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb97f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fb97f-118">Not supported.</span></span>|
|<span data-ttu-id="fb97f-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb97f-119">Application</span></span>                            | <span data-ttu-id="fb97f-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb97f-120">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb97f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fb97f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="fb97f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fb97f-122">Request headers</span></span>
| <span data-ttu-id="fb97f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="fb97f-123">Name</span></span>         | <span data-ttu-id="fb97f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb97f-124">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="fb97f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fb97f-125">Authorization</span></span>|<span data-ttu-id="fb97f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb97f-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="fb97f-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="fb97f-128">Content-type</span></span> | <span data-ttu-id="fb97f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fb97f-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb97f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fb97f-131">Request body</span></span>
<span data-ttu-id="fb97f-132">No corpo da solicitação, fornece uma representação JSON de [um objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fb97f-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="fb97f-133">A tabela a seguir mostra as propriedades aceitas para atualizar um accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="fb97f-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="fb97f-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb97f-134">Property</span></span> | <span data-ttu-id="fb97f-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb97f-135">Type</span></span> | <span data-ttu-id="fb97f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb97f-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fb97f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fb97f-137">displayName</span></span> | <span data-ttu-id="fb97f-138">String</span><span class="sxs-lookup"><span data-stu-id="fb97f-138">String</span></span> | <span data-ttu-id="fb97f-139">Nome da série de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="fb97f-139">Name of access review series.</span></span> |
| <span data-ttu-id="fb97f-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="fb97f-140">descriptionForAdmins</span></span> | <span data-ttu-id="fb97f-141">String</span><span class="sxs-lookup"><span data-stu-id="fb97f-141">String</span></span> | <span data-ttu-id="fb97f-142">Contexto da revisão fornecida aos administradores.</span><span class="sxs-lookup"><span data-stu-id="fb97f-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="fb97f-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="fb97f-143">descriptionForReviewers</span></span> | <span data-ttu-id="fb97f-144">String</span><span class="sxs-lookup"><span data-stu-id="fb97f-144">String</span></span> | <span data-ttu-id="fb97f-145">Contexto da revisão fornecida aos revisadores.</span><span class="sxs-lookup"><span data-stu-id="fb97f-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="fb97f-146">settings</span><span class="sxs-lookup"><span data-stu-id="fb97f-146">settings</span></span> | [<span data-ttu-id="fb97f-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="fb97f-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="fb97f-148">As configurações de uma série de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="fb97f-148">The settings for an access review series.</span></span> <span data-ttu-id="fb97f-149">Consulte [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fb97f-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="fb97f-150">revisadores</span><span class="sxs-lookup"><span data-stu-id="fb97f-150">reviewers</span></span> | <span data-ttu-id="fb97f-151">[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="fb97f-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="fb97f-152">Define quem são os revisadores.</span><span class="sxs-lookup"><span data-stu-id="fb97f-152">Defines who the reviewers are.</span></span> <span data-ttu-id="fb97f-153">Se nenhum for especificado, a revisão será uma autoavaliação (os usuários revisados analisam seu próprio acesso).</span><span class="sxs-lookup"><span data-stu-id="fb97f-153">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="fb97f-154">A propriedade Reviewers só será atualizável se usuários individuais atribuídos são revistores.</span><span class="sxs-lookup"><span data-stu-id="fb97f-154">The Reviewers property is only updatable if individual users assigned are as reviewers.</span></span> <span data-ttu-id="fb97f-155">Consulte [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="fb97f-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> | 

<span data-ttu-id="fb97f-156">Observe que uma solicitação PUT espera que o objeto completo seja passado, no qual todas as propriedades writable estão incluídas, e não apenas as propriedades que estão sendo atualizadas.</span><span class="sxs-lookup"><span data-stu-id="fb97f-156">Note that a PUT request expects the full object to be passed in, in which all writable properties are included, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="fb97f-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb97f-157">Response</span></span>
<span data-ttu-id="fb97f-158">Se tiver êxito, este método retornará um `204, Accepted` código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fb97f-158">If successful, this method returns a `204, Accepted` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb97f-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fb97f-159">Examples</span></span>

<span data-ttu-id="fb97f-160">Este é um exemplo de atualização do displayName de uma série de revisão de acesso existente.</span><span class="sxs-lookup"><span data-stu-id="fb97f-160">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="fb97f-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fb97f-161">Request</span></span>
<span data-ttu-id="fb97f-162">No corpo da solicitação, fornece uma representação JSON das novas propriedades do [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fb97f-162">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="fb97f-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb97f-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewScheduleDefinition"
}-->
```http
PUT https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6

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
# <a name="javascript"></a>[<span data-ttu-id="fb97f-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb97f-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb97f-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb97f-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fb97f-166">C#</span><span class="sxs-lookup"><span data-stu-id="fb97f-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb97f-167">Java</span><span class="sxs-lookup"><span data-stu-id="fb97f-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="fb97f-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="fb97f-168">Response</span></span>
><span data-ttu-id="fb97f-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fb97f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 Accepted
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
