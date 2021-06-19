---
title: Atualizar accessReviewScheduleDefinition
description: Atualize um objeto accessReviewScheduleDefinition existente para alterar uma ou mais de suas propriedades.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: be3b7603419d616ef9ea9e4da94fdb8942dc36f3
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030443"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="cb5f2-103">Atualizar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="cb5f2-103">Update accessReviewScheduleDefinition</span></span>

<span data-ttu-id="cb5f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb5f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb5f2-105">Atualize um [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) existente para alterar uma ou mais de suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-105">Update an existing [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object to change one or more of its properties.</span></span>

>[!NOTE]
><span data-ttu-id="cb5f2-106">Todas as atualizações feitas em um accessReviewScheduleDefinition só se aplicam a instâncias futuras.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-106">Any updates made to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="cb5f2-107">As instâncias em execução no momento não podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-107">Currently running instances cannot be updated.</span></span>
><span data-ttu-id="cb5f2-108">Além disso, essa API não se destina a atualizar propriedades, incluindo decisões, no nível accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="cb5f2-109">Consulte [accessReviewInstance para](../resources/accessreviewinstance.md) obter mais informações sobre instâncias.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb5f2-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb5f2-110">Permissions</span></span>
<span data-ttu-id="cb5f2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb5f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb5f2-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb5f2-113">Permission type</span></span>                        | <span data-ttu-id="cb5f2-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb5f2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb5f2-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb5f2-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb5f2-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb5f2-116">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="cb5f2-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb5f2-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb5f2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-118">Not supported.</span></span>|
|<span data-ttu-id="cb5f2-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb5f2-119">Application</span></span>                            | <span data-ttu-id="cb5f2-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb5f2-120">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb5f2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb5f2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="cb5f2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb5f2-122">Request headers</span></span>
| <span data-ttu-id="cb5f2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="cb5f2-123">Name</span></span>         | <span data-ttu-id="cb5f2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb5f2-124">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="cb5f2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb5f2-125">Authorization</span></span>|<span data-ttu-id="cb5f2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="cb5f2-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="cb5f2-128">Content-type</span></span> | <span data-ttu-id="cb5f2-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb5f2-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb5f2-131">Request body</span></span>
<span data-ttu-id="cb5f2-132">No corpo da solicitação, fornece uma representação JSON de [um objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cb5f2-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="cb5f2-133">A tabela a seguir mostra as propriedades aceitas para atualizar um accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="cb5f2-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb5f2-134">Property</span></span> | <span data-ttu-id="cb5f2-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb5f2-135">Type</span></span> | <span data-ttu-id="cb5f2-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb5f2-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cb5f2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cb5f2-137">displayName</span></span> | <span data-ttu-id="cb5f2-138">String</span><span class="sxs-lookup"><span data-stu-id="cb5f2-138">String</span></span> | <span data-ttu-id="cb5f2-139">Nome da série de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-139">Name of access review series.</span></span> |
| <span data-ttu-id="cb5f2-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="cb5f2-140">descriptionForAdmins</span></span> | <span data-ttu-id="cb5f2-141">String</span><span class="sxs-lookup"><span data-stu-id="cb5f2-141">String</span></span> | <span data-ttu-id="cb5f2-142">Contexto da revisão fornecida aos administradores.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="cb5f2-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="cb5f2-143">descriptionForReviewers</span></span> | <span data-ttu-id="cb5f2-144">String</span><span class="sxs-lookup"><span data-stu-id="cb5f2-144">String</span></span> | <span data-ttu-id="cb5f2-145">Contexto da revisão fornecida aos revisadores.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="cb5f2-146">configurações</span><span class="sxs-lookup"><span data-stu-id="cb5f2-146">settings</span></span> | [<span data-ttu-id="cb5f2-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="cb5f2-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="cb5f2-148">As configurações de uma série de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-148">The settings for an access review series.</span></span> <span data-ttu-id="cb5f2-149">Consulte [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cb5f2-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="cb5f2-150">revisadores</span><span class="sxs-lookup"><span data-stu-id="cb5f2-150">reviewers</span></span> | <span data-ttu-id="cb5f2-151">[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="cb5f2-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="cb5f2-152">Define quem são os revisadores.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-152">Defines who the reviewers are.</span></span> <span data-ttu-id="cb5f2-153">Se nenhum for especificado, a revisão será uma autoavaliação (os usuários revisam seu próprio acesso).</span><span class="sxs-lookup"><span data-stu-id="cb5f2-153">If none are specified, the review is a self-review (users review their own access).</span></span> <span data-ttu-id="cb5f2-154">A **propriedade reviewers** só será atualizável se usuários individuais são atribuídos como revistores.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-154">The **reviewers** property is only updatable if individual users are assigned as reviewers.</span></span> <span data-ttu-id="cb5f2-155">Consulte [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="cb5f2-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |
|<span data-ttu-id="cb5f2-156">fallbackReviewers</span><span class="sxs-lookup"><span data-stu-id="cb5f2-156">fallbackReviewers</span></span>|<span data-ttu-id="cb5f2-157">[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="cb5f2-157">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="cb5f2-158">Uma coleção de escopos do revistor usado para definir a lista de revisadores de fallback que são notificados para tomar medidas se nenhum usuário for encontrado na lista de revisadores especificados.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-158">A collection of reviewer scopes used to define the list of fallback reviewers who are notified to take action if no users are found from the list of reviewers specified.</span></span> <span data-ttu-id="cb5f2-159">Isso pode ocorrer quando o proprietário do grupo é especificado como o revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-159">This could occur when either the group owner is specified as the reviewer but the group owner does not exist, or manager is specified as reviewer but a user's manager does not exist.</span></span>|
| <span data-ttu-id="cb5f2-160">backupReviewers (preterido)</span><span class="sxs-lookup"><span data-stu-id="cb5f2-160">backupReviewers (deprecated)</span></span>|<span data-ttu-id="cb5f2-161">[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="cb5f2-161">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>| <span data-ttu-id="cb5f2-162">Essa propriedade foi substituída por **fallbackReviewers**.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-162">This property has been replaced by **fallbackReviewers**.</span></span> <span data-ttu-id="cb5f2-163">No entanto, especificar **backupReviewers** ou **fallbackReviewers** preenche automaticamente os mesmos valores para a outra propriedade.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-163">However, specifying either **backupReviewers** or **fallbackReviewers** automatically populates the same values to the other property.</span></span> |

<span data-ttu-id="cb5f2-164">Uma **solicitação PUT** espera que o objeto completo seja passado, o que inclui todas as propriedades que podem ser escritas, e não apenas as propriedades que estão sendo atualizadas.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-164">A **PUT** request expects the full object to be passed in, which includes all writable properties, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="cb5f2-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb5f2-165">Response</span></span>
<span data-ttu-id="cb5f2-166">Se tiver êxito, este método retornará um `204 No Content` código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-166">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb5f2-167">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cb5f2-167">Examples</span></span>

<span data-ttu-id="cb5f2-168">Este é um exemplo de atualização do displayName de uma série de revisão de acesso existente.</span><span class="sxs-lookup"><span data-stu-id="cb5f2-168">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="cb5f2-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb5f2-169">Request</span></span>
<span data-ttu-id="cb5f2-170">No corpo da solicitação, fornece uma representação JSON das novas propriedades do [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cb5f2-170">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="cb5f2-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb5f2-171">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="cb5f2-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb5f2-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb5f2-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb5f2-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="cb5f2-174">C#</span><span class="sxs-lookup"><span data-stu-id="cb5f2-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb5f2-175">Java</span><span class="sxs-lookup"><span data-stu-id="cb5f2-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="cb5f2-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb5f2-176">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
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
