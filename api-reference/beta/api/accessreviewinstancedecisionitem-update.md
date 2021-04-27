---
title: Atualizar accessReviewInstanceDecisionItem
description: Atualize um objeto accessReviewInstanceDecisionItem existente de que chamar o usuário é o revisor.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a104d963c3d5bbad3cff11b998f9a9a2240d08b5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048376"
---
# <a name="update-accessreviewinstancedecisionitem"></a><span data-ttu-id="b416d-103">Atualizar accessReviewInstanceDecisionItem</span><span class="sxs-lookup"><span data-stu-id="b416d-103">Update accessReviewInstanceDecisionItem</span></span>

<span data-ttu-id="b416d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b416d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b416d-105">Atualizar decisões de acesso, conhecidas como [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), para as quais o usuário é o revisor.</span><span class="sxs-lookup"><span data-stu-id="b416d-105">Update access decisions, known as [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md), for which the user is the reviewer.</span></span>

>[!NOTE]
><span data-ttu-id="b416d-106">Todas as atualizações feitas em **um accessReviewInstanceDecisionItem** só podem ser feitas chamando usuários listados como revisores do [accessReviewInstance pai.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="b416d-106">Any updates made to an **accessReviewInstanceDecisionItem** can only be made by calling users who are listed as reviewer for the parent [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b416d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b416d-107">Permissions</span></span>
<span data-ttu-id="b416d-108">Uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="b416d-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b416d-109">Não há suporte para permissões delegadas para contas pessoais da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b416d-109">Delegated permissions to personal Microsoft accounts are not supported.</span></span> <span data-ttu-id="b416d-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b416d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b416d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b416d-111">Permission type</span></span>                        | <span data-ttu-id="b416d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b416d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b416d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b416d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b416d-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b416d-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b416d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b416d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b416d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b416d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b416d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b416d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a><span data-ttu-id="b416d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b416d-118">Request headers</span></span>
| <span data-ttu-id="b416d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b416d-119">Name</span></span>         | <span data-ttu-id="b416d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b416d-120">Description</span></span> |
|:-------------|:------------|
|<span data-ttu-id="b416d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b416d-121">Authorization</span></span>|<span data-ttu-id="b416d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b416d-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b416d-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="b416d-124">Content-type</span></span> | <span data-ttu-id="b416d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b416d-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b416d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b416d-127">Request body</span></span>
<span data-ttu-id="b416d-128">A tabela a seguir mostra as propriedades aceitas para atualizar um `accessReviewInstanceDecisionItem` .</span><span class="sxs-lookup"><span data-stu-id="b416d-128">The following table shows the properties accepted to update an `accessReviewInstanceDecisionItem`.</span></span>

| <span data-ttu-id="b416d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b416d-129">Property</span></span>     | <span data-ttu-id="b416d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b416d-130">Type</span></span>       | <span data-ttu-id="b416d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b416d-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b416d-132">decision</span><span class="sxs-lookup"><span data-stu-id="b416d-132">decision</span></span>  | <span data-ttu-id="b416d-133">String</span><span class="sxs-lookup"><span data-stu-id="b416d-133">String</span></span> | <span data-ttu-id="b416d-134">Decisão de acesso para a entidade que está sendo revisada.</span><span class="sxs-lookup"><span data-stu-id="b416d-134">Access decision for the entity being reviewed.</span></span> <span data-ttu-id="b416d-135">Os valores possíveis são: `Approve` `Deny` `NotReviewed` `DontKnow` .</span><span class="sxs-lookup"><span data-stu-id="b416d-135">Possible values are: `Approve` `Deny` `NotReviewed` `DontKnow`.</span></span> <span data-ttu-id="b416d-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b416d-136">Required.</span></span>  |
|  <span data-ttu-id="b416d-137">justification</span><span class="sxs-lookup"><span data-stu-id="b416d-137">justification</span></span> | <span data-ttu-id="b416d-138">String</span><span class="sxs-lookup"><span data-stu-id="b416d-138">String</span></span> | <span data-ttu-id="b416d-139">Contexto da revisão fornecida aos administradores.</span><span class="sxs-lookup"><span data-stu-id="b416d-139">Context of the review provided to admins.</span></span> <span data-ttu-id="b416d-140">Obrigatório se justificationRequiredOnApproval for True no accessReviewScheduleDefinition.</span><span class="sxs-lookup"><span data-stu-id="b416d-140">Required if justificationRequiredOnApproval is True on the accessReviewScheduleDefinition.</span></span>  |

## <a name="response"></a><span data-ttu-id="b416d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b416d-141">Response</span></span>
<span data-ttu-id="b416d-142">Se tiver êxito, este método retornará um `204, NoContent` código de resposta e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b416d-142">If successful, this method returns a `204, NoContent` response code and no response body.</span></span>

### <a name="request"></a><span data-ttu-id="b416d-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b416d-143">Request</span></span>
## <a name="examples"></a><span data-ttu-id="b416d-144">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b416d-144">Examples</span></span>

<span data-ttu-id="b416d-145">Este é um exemplo de aprovação do acesso a um usuário representado por `accessReviewInstanceDecisionItem` um .</span><span class="sxs-lookup"><span data-stu-id="b416d-145">This is an example of approving access for a user represented by an `accessReviewInstanceDecisionItem`.</span></span>



# <a name="http"></a>[<span data-ttu-id="b416d-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="b416d-146">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b416d-147">C#</span><span class="sxs-lookup"><span data-stu-id="b416d-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b416d-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b416d-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b416d-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b416d-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b416d-150">Java</span><span class="sxs-lookup"><span data-stu-id="b416d-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="b416d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="b416d-151">Response</span></span>
><span data-ttu-id="b416d-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b416d-152">**Note:** The response object shown here might be shortened for readability.</span></span>
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
