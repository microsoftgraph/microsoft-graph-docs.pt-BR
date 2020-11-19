---
title: Atualizar accessReviewInstanceDecisionItem
description: Atualize um objeto accessReviewInstanceDecisionItem existente que chama o usuário é o revisor de.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2f14ed26169c659354af16963e03e449f246421c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214328"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="a9fb8-103">Atualizar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="a9fb8-103">Update accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="a9fb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9fb8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9fb8-105">Atualize as decisões de acesso, conhecidas como [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), para as quais o usuário é o revisor.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-105">Update access decisions, known as [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), for which the user is the reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="a9fb8-106">Todas as atualizações feitas em um **accessReviewInstanceDecisionItem** só podem ser feitas chamando usuários que estão listados como revisor para o [accessReviewInstance](../resources/accessreviewinstance.md)pai.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-106">Any updates made to an **accessReviewInstanceDecisionItem** can only be made by calling users who are listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9fb8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9fb8-107">Permissions</span></span>
<span data-ttu-id="a9fb8-108">Uma das seguintes permissões é necessária para chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="a9fb8-109">Permissões delegadas para contas pessoais da Microsoft não são suportadas.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-109">Delegated permissions to personal Microsoft accounts are not supported.</span></span> <span data-ttu-id="a9fb8-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9fb8-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9fb8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9fb8-111">Permission type</span></span>                        | <span data-ttu-id="a9fb8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9fb8-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9fb8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9fb8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9fb8-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9fb8-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="a9fb8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9fb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9fb8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9fb8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9fb8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a><span data-ttu-id="a9fb8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9fb8-118">Request headers</span></span>
| <span data-ttu-id="a9fb8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a9fb8-119">Name</span></span>         | <span data-ttu-id="a9fb8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9fb8-120">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="a9fb8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9fb8-121">Authorization</span></span>|<span data-ttu-id="a9fb8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a9fb8-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="a9fb8-124">Content-type</span></span> | <span data-ttu-id="a9fb8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9fb8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9fb8-127">Request body</span></span>
<span data-ttu-id="a9fb8-128">A tabela a seguir mostra as propriedades aceitas para atualizar um `accessReviewInstanceDecisionItem` .</span><span class="sxs-lookup"><span data-stu-id="a9fb8-128">The following table shows the properties accepted to update an `accessReviewInstanceDecisionItem`.</span></span>

| <span data-ttu-id="a9fb8-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9fb8-129">Property</span></span>     | <span data-ttu-id="a9fb8-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9fb8-130">Type</span></span>       | <span data-ttu-id="a9fb8-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9fb8-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a9fb8-132">sobre</span><span class="sxs-lookup"><span data-stu-id="a9fb8-132">decision</span></span>  | <span data-ttu-id="a9fb8-133">String</span><span class="sxs-lookup"><span data-stu-id="a9fb8-133">String</span></span> | <span data-ttu-id="a9fb8-134">Decisão de acesso para a entidade que está sendo revisada.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-134">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="a9fb8-135">Os valores possíveis são: `Approve` `Deny` `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="a9fb8-135">Possible values are: `Approve` `Deny` `NotReviewed` `DontKnow`.</span></span> <span data-ttu-id="a9fb8-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-136">Required.</span></span>  |
|  <span data-ttu-id="a9fb8-137">elabora</span><span class="sxs-lookup"><span data-stu-id="a9fb8-137">justification</span></span> | <span data-ttu-id="a9fb8-138">String</span><span class="sxs-lookup"><span data-stu-id="a9fb8-138">String</span></span> | <span data-ttu-id="a9fb8-139">Contexto da revisão fornecida aos administradores.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-139">Context of the review provided to admins.</span></span> <span data-ttu-id="a9fb8-140">Obrigatório se justificationRequiredOnApproval for true no accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-140">Required if justificationRequiredOnApproval is True on the accessReviewScheduleDefinition.</span></span>  |

## <a name="response"></a><span data-ttu-id="a9fb8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9fb8-141">Response</span></span>
<span data-ttu-id="a9fb8-142">Se tiver êxito, este método retornará um `204, NoContent` código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-142">If successful, this method returns a `204, NoContent` response code and no response body.</span></span>

### <a name="request"></a><span data-ttu-id="a9fb8-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9fb8-143">Request</span></span>
## <a name="examples"></a><span data-ttu-id="a9fb8-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a9fb8-144">Examples</span></span>

<span data-ttu-id="a9fb8-145">Este é um exemplo de aprovação de acesso de um usuário representado por um `accessReviewInstanceDecisionItem` .</span><span class="sxs-lookup"><span data-stu-id="a9fb8-145">This is an example of approving access for a user represented by an `accessReviewInstanceDecisionItem`.</span></span>


# <a name="http"></a>[<span data-ttu-id="a9fb8-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9fb8-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/654b34e7-b48f-4772-a2d4-08f1d0dd014c

{
  "decision": "Approve",
  "justification": "I trust this person"
}
```
# <a name="c"></a>[<span data-ttu-id="a9fb8-147">C#</span><span class="sxs-lookup"><span data-stu-id="a9fb8-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9fb8-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9fb8-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9fb8-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9fb8-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9fb8-150">Java</span><span class="sxs-lookup"><span data-stu-id="a9fb8-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="a9fb8-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9fb8-151">Response</span></span>
><span data-ttu-id="a9fb8-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9fb8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
