---
title: Atualizar accessReviewInstanceDecisionItem
description: Atualize um objeto accessReviewInstanceDecisionItem existente de que chamar o usuário é o revisor.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 913c53927ecc8e436c8d3c63e73d827af5eb4271
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507188"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="18341-103">Atualizar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="18341-103">Update accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="18341-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18341-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18341-105">Atualizar decisões de acesso, conhecidas como [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), para as quais o usuário é o revisor.</span><span class="sxs-lookup"><span data-stu-id="18341-105">Update access decisions, known as [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), for which the user is the reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="18341-106">Todas as atualizações feitas em **um accessReviewInstanceDecisionItem** só podem ser feitas chamando usuários listados como revisores do [accessReviewInstance pai.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="18341-106">Any updates made to an **accessReviewInstanceDecisionItem** can only be made by calling users who are listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18341-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="18341-107">Permissions</span></span>
<span data-ttu-id="18341-108">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="18341-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="18341-109">Não há suporte para permissões delegadas para contas pessoais da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="18341-109">Delegated permissions to personal Microsoft accounts are not supported.</span></span> <span data-ttu-id="18341-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18341-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18341-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18341-111">Permission type</span></span>                        | <span data-ttu-id="18341-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18341-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="18341-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18341-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="18341-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18341-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="18341-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18341-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18341-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18341-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18341-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18341-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a><span data-ttu-id="18341-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18341-118">Request headers</span></span>
| <span data-ttu-id="18341-119">Nome</span><span class="sxs-lookup"><span data-stu-id="18341-119">Name</span></span>         | <span data-ttu-id="18341-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="18341-120">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="18341-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="18341-121">Authorization</span></span>|<span data-ttu-id="18341-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18341-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="18341-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="18341-124">Content-type</span></span> | <span data-ttu-id="18341-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18341-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18341-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18341-127">Request body</span></span>
<span data-ttu-id="18341-128">A tabela a seguir mostra as propriedades aceitas para atualizar um `accessReviewInstanceDecisionItem` .</span><span class="sxs-lookup"><span data-stu-id="18341-128">The following table shows the properties accepted to update an `accessReviewInstanceDecisionItem`.</span></span>

| <span data-ttu-id="18341-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18341-129">Property</span></span>     | <span data-ttu-id="18341-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="18341-130">Type</span></span>       | <span data-ttu-id="18341-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="18341-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="18341-132">decision</span><span class="sxs-lookup"><span data-stu-id="18341-132">decision</span></span>  | <span data-ttu-id="18341-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18341-133">String</span></span> | <span data-ttu-id="18341-134">Decisão de acesso para a entidade que está sendo revisada.</span><span class="sxs-lookup"><span data-stu-id="18341-134">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="18341-135">Os valores possíveis são: `Approve` `Deny` `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="18341-135">Possible values are: `Approve` `Deny` `NotReviewed` `DontKnow`.</span></span> <span data-ttu-id="18341-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18341-136">Required.</span></span>  |
|  <span data-ttu-id="18341-137">justification</span><span class="sxs-lookup"><span data-stu-id="18341-137">justification</span></span> | <span data-ttu-id="18341-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18341-138">String</span></span> | <span data-ttu-id="18341-139">Contexto da revisão fornecida aos administradores.</span><span class="sxs-lookup"><span data-stu-id="18341-139">Context of the review provided to admins.</span></span> <span data-ttu-id="18341-140">Obrigatório se justificationRequiredOnApproval for True no accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="18341-140">Required if justificationRequiredOnApproval is True on the accessReviewScheduleDefinition.</span></span>  |

## <a name="response"></a><span data-ttu-id="18341-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="18341-141">Response</span></span>
<span data-ttu-id="18341-142">Se tiver êxito, este método retornará um `204, NoContent` código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18341-142">If successful, this method returns a `204, NoContent` response code and no response body.</span></span>

### <a name="request"></a><span data-ttu-id="18341-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18341-143">Request</span></span>
## <a name="examples"></a><span data-ttu-id="18341-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="18341-144">Examples</span></span>

<span data-ttu-id="18341-145">Este é um exemplo de aprovação do acesso a um usuário representado por `accessReviewInstanceDecisionItem` um .</span><span class="sxs-lookup"><span data-stu-id="18341-145">This is an example of approving access for a user represented by an `accessReviewInstanceDecisionItem`.</span></span>



# <a name="http"></a>[<span data-ttu-id="18341-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="18341-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
``` http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/12348410-67f3-4d4c-b946-6989e050be19
Content-Type: application/json
Content-length: 730

{
  "decision": "Approve",
  "justification": "This person is still on my team",
}
```
# <a name="c"></a>[<span data-ttu-id="18341-147">C#</span><span class="sxs-lookup"><span data-stu-id="18341-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18341-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18341-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18341-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18341-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18341-150">Java</span><span class="sxs-lookup"><span data-stu-id="18341-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="18341-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="18341-151">Response</span></span>
><span data-ttu-id="18341-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="18341-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem"
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
