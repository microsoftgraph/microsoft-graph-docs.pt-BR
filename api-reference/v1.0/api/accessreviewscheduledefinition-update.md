---
title: Atualizar accessReviewScheduleDefinition
description: Atualize as propriedades de um objeto accessReviewScheduleDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6f3c39f6111ad910d2551da7e03cdf6e03597b3d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208383"
---
# <a name="update-accessreviewscheduledefinition"></a><span data-ttu-id="50a6b-103">Atualizar accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="50a6b-103">Update accessReviewScheduleDefinition</span></span>
<span data-ttu-id="50a6b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50a6b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50a6b-105">Atualize as propriedades de [um objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50a6b-105">Update the properties of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="50a6b-106">Todas as atualizações de um accessReviewScheduleDefinition só se aplicam a instâncias futuras.</span><span class="sxs-lookup"><span data-stu-id="50a6b-106">Any updates to an accessReviewScheduleDefinition only apply to future instances.</span></span> <span data-ttu-id="50a6b-107">As instâncias em execução no momento não podem ser atualizadas.</span><span class="sxs-lookup"><span data-stu-id="50a6b-107">Currently running instances cannot be updated.</span></span> <span data-ttu-id="50a6b-108">Além disso, essa API não se destina a atualizar propriedades, incluindo decisões, no nível accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="50a6b-108">Additionally, this API is not intended to update properties, including decisions, on the accessReviewInstance level.</span></span> <span data-ttu-id="50a6b-109">Consulte [accessReviewInstance para](../resources/accessreviewinstance.md) obter mais informações sobre instâncias.</span><span class="sxs-lookup"><span data-stu-id="50a6b-109">See [accessReviewInstance](../resources/accessreviewinstance.md) for more information on instances.</span></span>

## <a name="permissions"></a><span data-ttu-id="50a6b-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="50a6b-110">Permissions</span></span>
<span data-ttu-id="50a6b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50a6b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50a6b-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50a6b-113">Permission type</span></span>|<span data-ttu-id="50a6b-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="50a6b-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50a6b-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50a6b-115">Delegated (work or school account)</span></span>|<span data-ttu-id="50a6b-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50a6b-116">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="50a6b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50a6b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50a6b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50a6b-118">Not supported.</span></span>|
|<span data-ttu-id="50a6b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50a6b-119">Application</span></span>|<span data-ttu-id="50a6b-120">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50a6b-120">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50a6b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50a6b-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="50a6b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50a6b-122">Request headers</span></span>
|<span data-ttu-id="50a6b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="50a6b-123">Name</span></span>|<span data-ttu-id="50a6b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="50a6b-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="50a6b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="50a6b-125">Authorization</span></span>|<span data-ttu-id="50a6b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50a6b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="50a6b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50a6b-128">Content-Type</span></span>|<span data-ttu-id="50a6b-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50a6b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="50a6b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50a6b-131">Request body</span></span>
<span data-ttu-id="50a6b-132">No corpo da solicitação, fornece uma representação JSON de [um objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50a6b-132">In the request body, supply a JSON representation of an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

<span data-ttu-id="50a6b-133">A tabela a seguir mostra as propriedades aceitas para atualizar um accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="50a6b-133">The following table shows the properties accepted to update an accessReviewScheduleDefinition.</span></span>

| <span data-ttu-id="50a6b-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50a6b-134">Property</span></span> | <span data-ttu-id="50a6b-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="50a6b-135">Type</span></span> | <span data-ttu-id="50a6b-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="50a6b-136">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="50a6b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="50a6b-137">displayName</span></span> | <span data-ttu-id="50a6b-138">String</span><span class="sxs-lookup"><span data-stu-id="50a6b-138">String</span></span> | <span data-ttu-id="50a6b-139">Nome da série de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="50a6b-139">Name of access review series.</span></span> |
| <span data-ttu-id="50a6b-140">descriptionForAdmins</span><span class="sxs-lookup"><span data-stu-id="50a6b-140">descriptionForAdmins</span></span> | <span data-ttu-id="50a6b-141">String</span><span class="sxs-lookup"><span data-stu-id="50a6b-141">String</span></span> | <span data-ttu-id="50a6b-142">Contexto da revisão fornecida aos administradores.</span><span class="sxs-lookup"><span data-stu-id="50a6b-142">Context of the review provided to admins.</span></span> |
| <span data-ttu-id="50a6b-143">descriptionForReviewers</span><span class="sxs-lookup"><span data-stu-id="50a6b-143">descriptionForReviewers</span></span> | <span data-ttu-id="50a6b-144">String</span><span class="sxs-lookup"><span data-stu-id="50a6b-144">String</span></span> | <span data-ttu-id="50a6b-145">Contexto da revisão fornecida aos revisadores.</span><span class="sxs-lookup"><span data-stu-id="50a6b-145">Context of the review provided to reviewers.</span></span> |
| <span data-ttu-id="50a6b-146">settings</span><span class="sxs-lookup"><span data-stu-id="50a6b-146">settings</span></span> | [<span data-ttu-id="50a6b-147">accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="50a6b-147">accessReviewScheduleSettings</span></span>](../resources/accessreviewschedulesettings.md) | <span data-ttu-id="50a6b-148">As configurações de uma série de revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="50a6b-148">The settings for an access review series.</span></span> <span data-ttu-id="50a6b-149">Consulte [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="50a6b-149">See [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md).</span></span> |
| <span data-ttu-id="50a6b-150">revisadores</span><span class="sxs-lookup"><span data-stu-id="50a6b-150">reviewers</span></span> | <span data-ttu-id="50a6b-151">[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="50a6b-151">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|  <span data-ttu-id="50a6b-152">Define quem são os revisadores.</span><span class="sxs-lookup"><span data-stu-id="50a6b-152">Defines who the reviewers are.</span></span> <span data-ttu-id="50a6b-153">Se nenhum for especificado, a revisão será uma autoavaliação (os usuários revisam seu próprio acesso).</span><span class="sxs-lookup"><span data-stu-id="50a6b-153">If none are specified, the review is a self-review (users review their own access).</span></span> <span data-ttu-id="50a6b-154">A **propriedade reviewers** só será atualizável se usuários individuais são atribuídos como revistores.</span><span class="sxs-lookup"><span data-stu-id="50a6b-154">The **reviewers** property is only updatable if individual users are assigned as reviewers.</span></span> <span data-ttu-id="50a6b-155">Consulte [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="50a6b-155">See [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md).</span></span> |
|<span data-ttu-id="50a6b-156">fallbackReviewers</span><span class="sxs-lookup"><span data-stu-id="50a6b-156">fallbackReviewers</span></span>|<span data-ttu-id="50a6b-157">[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)</span><span class="sxs-lookup"><span data-stu-id="50a6b-157">[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection</span></span>|<span data-ttu-id="50a6b-158">Uma coleção de escopos do revistor usado para definir a lista de revisadores de fallback que são notificados para tomar medidas se nenhum usuário for encontrado na lista de revisadores especificados.</span><span class="sxs-lookup"><span data-stu-id="50a6b-158">A collection of reviewer scopes used to define the list of fallback reviewers who are notified to take action if no users are found from the list of reviewers specified.</span></span> <span data-ttu-id="50a6b-159">Isso pode ocorrer quando o proprietário do grupo é especificado como o revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe.</span><span class="sxs-lookup"><span data-stu-id="50a6b-159">This could occur when either the group owner is specified as the reviewer but the group owner does not exist, or manager is specified as reviewer but a user's manager does not exist.</span></span>|

<span data-ttu-id="50a6b-160">Uma **solicitação PUT** espera que o objeto completo seja passado, o que inclui todas as propriedades que podem ser escritas, e não apenas as propriedades que estão sendo atualizadas.</span><span class="sxs-lookup"><span data-stu-id="50a6b-160">A **PUT** request expects the full object to be passed in, which includes all writable properties, not just the properties being updated.</span></span>

## <a name="response"></a><span data-ttu-id="50a6b-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="50a6b-161">Response</span></span>
<span data-ttu-id="50a6b-162">Se tiver êxito, este método retornará um `204 No Content` código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="50a6b-162">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="examples"></a><span data-ttu-id="50a6b-163">Exemplos</span><span class="sxs-lookup"><span data-stu-id="50a6b-163">Examples</span></span>
<span data-ttu-id="50a6b-164">Este é um exemplo de atualização do displayName de uma série de revisão de acesso existente.</span><span class="sxs-lookup"><span data-stu-id="50a6b-164">This is an example of updating the displayName of an existing access review series.</span></span>

### <a name="request"></a><span data-ttu-id="50a6b-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50a6b-165">Request</span></span>
<span data-ttu-id="50a6b-166">No corpo da solicitação, fornece uma representação JSON das novas propriedades do [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="50a6b-166">In the request body, supply a JSON representation of the new properties of the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="50a6b-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="50a6b-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewscheduledefinition"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6

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
# <a name="c"></a>[<span data-ttu-id="50a6b-168">C#</span><span class="sxs-lookup"><span data-stu-id="50a6b-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50a6b-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50a6b-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50a6b-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50a6b-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50a6b-171">Java</span><span class="sxs-lookup"><span data-stu-id="50a6b-171">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="50a6b-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="50a6b-172">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
