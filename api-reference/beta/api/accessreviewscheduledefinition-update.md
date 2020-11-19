---
title: Atualizar accessReviewScheduleDefinition
description: Atualize um objeto accessReviewScheduleDefinition existente para alterar uma ou mais de suas propriedades.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 06b69bb9e6defcbadb4694d4042fa3bb690ee0f4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221776"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="e1828-103">Atualizar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="e1828-103">Update accessReviewScheduleDefinition</span></span>

<span data-ttu-id="e1828-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1828-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1828-105">Atualize um objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) existente para alterar uma ou mais de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="e1828-105">Update an existing [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object to change one or more of its properties.</span></span>

>[!NOTE]
><span data-ttu-id="e1828-106">Todas as atualizações feitas em um accessReviewScheduleDefinition se aplicam apenas às instâncias futuras.</span><span class="sxs-lookup"><span data-stu-id="e1828-106">Any updates made to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="e1828-107">As instâncias em execução no momento não podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="e1828-107">Currently running instances cannot be updated.</span></span>
><span data-ttu-id="e1828-108">Além disso, essa API não se destina a atualizar propriedades, incluindo decisões, no nível accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="e1828-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="e1828-109">Consulte [accessReviewInstance](../resources/accessreviewinstance.md) para obter mais informações sobre instâncias.</span><span class="sxs-lookup"><span data-stu-id="e1828-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1828-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1828-110">Permissions</span></span>
<span data-ttu-id="e1828-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1828-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1828-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1828-113">Permission type</span></span>                        | <span data-ttu-id="e1828-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1828-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1828-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1828-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1828-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1828-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="e1828-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1828-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1828-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1828-118">Not supported.</span></span>|
|<span data-ttu-id="e1828-119">Application</span><span class="sxs-lookup"><span data-stu-id="e1828-119">Application</span></span>                            | <span data-ttu-id="e1828-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1828-120">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1828-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1828-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="e1828-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1828-122">Request headers</span></span>
| <span data-ttu-id="e1828-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e1828-123">Name</span></span>         | <span data-ttu-id="e1828-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1828-124">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="e1828-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1828-125">Authorization</span></span>|<span data-ttu-id="e1828-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1828-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e1828-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="e1828-128">Content-type</span></span> | <span data-ttu-id="e1828-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1828-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1828-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1828-131">Request body</span></span>
<span data-ttu-id="e1828-132">No corpo da solicitação, forneça uma representação JSON de um objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="e1828-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="e1828-133">A tabela a seguir mostra as propriedades aceitas para atualizar um accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="e1828-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="e1828-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1828-134">Property</span></span> | <span data-ttu-id="e1828-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1828-135">Type</span></span> | <span data-ttu-id="e1828-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1828-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e1828-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e1828-137">displayName</span></span> | <span data-ttu-id="e1828-138">String</span><span class="sxs-lookup"><span data-stu-id="e1828-138">String</span></span> | <span data-ttu-id="e1828-139">Nome da série de revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="e1828-139">Name of access review series.</span></span> |
| <span data-ttu-id="e1828-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="e1828-140">descriptionForAdmins</span></span> | <span data-ttu-id="e1828-141">String</span><span class="sxs-lookup"><span data-stu-id="e1828-141">String</span></span> | <span data-ttu-id="e1828-142">Contexto da revisão fornecida aos administradores.</span><span class="sxs-lookup"><span data-stu-id="e1828-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="e1828-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="e1828-143">descriptionForReviewers</span></span> | <span data-ttu-id="e1828-144">String</span><span class="sxs-lookup"><span data-stu-id="e1828-144">String</span></span> | <span data-ttu-id="e1828-145">Contexto da revisão fornecida aos revisores.</span><span class="sxs-lookup"><span data-stu-id="e1828-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="e1828-146">settings</span><span class="sxs-lookup"><span data-stu-id="e1828-146">settings</span></span> | [<span data-ttu-id="e1828-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="e1828-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="e1828-148">As configurações para uma série de análise do Access.</span><span class="sxs-lookup"><span data-stu-id="e1828-148">The settings for an access review series.</span></span> <span data-ttu-id="e1828-149">Consulte [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e1828-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="e1828-150">revisores</span><span class="sxs-lookup"><span data-stu-id="e1828-150">reviewers</span></span> | <span data-ttu-id="e1828-151">coleção [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="e1828-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="e1828-152">Define quem é os revisores.</span><span class="sxs-lookup"><span data-stu-id="e1828-152">Defines who the reviewers are.</span></span> <span data-ttu-id="e1828-153">Se nenhum for especificado, a revisão será uma autorevisão (os usuários revisaram revisar seu próprio acesso).</span><span class="sxs-lookup"><span data-stu-id="e1828-153">If none are specified, the review is a self-review (users reviewed review their own access).</span></span> <span data-ttu-id="e1828-154">A propriedade reviewers só será atualizável se os usuários individuais atribuídos forem como revisores.</span><span class="sxs-lookup"><span data-stu-id="e1828-154">The Reviewers property is only updatable if individual users assigned are as reviewers.</span></span> <span data-ttu-id="e1828-155">Consulte [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="e1828-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> | 

<span data-ttu-id="e1828-156">Observe que uma solicitação PUT espera que o objeto completo seja passado, no qual todas as propriedades graváveis são incluídas, e não apenas as propriedades que estão sendo atualizadas.</span><span class="sxs-lookup"><span data-stu-id="e1828-156">Note that a PUT request expects the full object to be passed in, in which all writable properties are included, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="e1828-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1828-157">Response</span></span>
<span data-ttu-id="e1828-158">Se tiver êxito, este método retornará um `204, Accepted` código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1828-158">If successful, this method returns a `204, Accepted` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e1828-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e1828-159">Examples</span></span>

<span data-ttu-id="e1828-160">Este é um exemplo de atualização do displayName de uma série de análise do Access existente.</span><span class="sxs-lookup"><span data-stu-id="e1828-160">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="e1828-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1828-161">Request</span></span>
<span data-ttu-id="e1828-162">No corpo da solicitação, forneça uma representação JSON das novas propriedades do objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="e1828-162">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="e1828-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1828-163">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="e1828-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1828-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1828-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1828-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="e1828-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1828-166">Response</span></span>
><span data-ttu-id="e1828-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1828-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
