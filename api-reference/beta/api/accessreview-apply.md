---
title: Aplicar accessReview
description: 'No recurso de revisões de acesso do Azure AD, aplique as decisões de um accessReview concluído.  O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente.  '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b590b741915aaf9ef901ee51e2eb11d43f9b439f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048530"
---
# <a name="apply-accessreview"></a><span data-ttu-id="7a50a-104">Aplicar accessReview</span><span class="sxs-lookup"><span data-stu-id="7a50a-104">Apply accessReview</span></span>

<span data-ttu-id="7a50a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a50a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a50a-106">No recurso de revisões de acesso do Azure [AD,](../resources/accessreviews-root.md) aplique as decisões de um [accessReview concluído.](../resources/accessreview.md)</span><span class="sxs-lookup"><span data-stu-id="7a50a-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="7a50a-107">O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="7a50a-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="7a50a-108">Depois que uma revisão de acesso for concluída, porque ela atingiu a data de término ou um administrador a interrompeu manualmente e a aplicação automática não foi configurada para a revisão, você pode chamar Apply para aplicar as alterações.</span><span class="sxs-lookup"><span data-stu-id="7a50a-108">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="7a50a-109">Até que ocorra a aplicação, as decisões para remover direitos de acesso não aparecem no recurso de origem, os usuários, por exemplo, retêm suas associações de grupo.</span><span class="sxs-lookup"><span data-stu-id="7a50a-109">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="7a50a-110">Ao chamar aplicar, o resultado da revisão é implementado atualizando o grupo ou aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a50a-110">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="7a50a-111">Se o acesso de um usuário foi negado na revisão, quando um administrador chama essa API, o Azure AD remove sua atribuição de associação ou aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7a50a-111">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="7a50a-112">Depois que uma revisão de acesso for concluída e a aplicação automática tiver sido configurada, o status da revisão mudará de Concluído para estados intermediários e, finalmente, mudará para o estado Aplicado.</span><span class="sxs-lookup"><span data-stu-id="7a50a-112">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="7a50a-113">Você deve esperar ver usuários negados, se algum, sendo removidos da associação do grupo de recursos ou atribuição de aplicativos em alguns minutos.</span><span class="sxs-lookup"><span data-stu-id="7a50a-113">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="7a50a-114">Uma revisão automática configurada ou selecionar Aplicar não tem efeito em um grupo que se origina em um diretório local ou em um grupo dinâmico.</span><span class="sxs-lookup"><span data-stu-id="7a50a-114">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="7a50a-115">Se você quiser alterar um grupo que se origina no local, baixe os resultados e aplique essas alterações à representação do grupo nesse diretório.</span><span class="sxs-lookup"><span data-stu-id="7a50a-115">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="7a50a-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a50a-116">Permissions</span></span>
<span data-ttu-id="7a50a-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a50a-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a50a-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a50a-119">Permission type</span></span>                        | <span data-ttu-id="7a50a-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a50a-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a50a-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a50a-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a50a-122">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a50a-122">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="7a50a-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a50a-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a50a-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a50a-124">Not supported.</span></span> |
|<span data-ttu-id="7a50a-125">Application</span><span class="sxs-lookup"><span data-stu-id="7a50a-125">Application</span></span>                            | <span data-ttu-id="7a50a-126">AccessReview.ReadWrite.Membership</span><span class="sxs-lookup"><span data-stu-id="7a50a-126">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a50a-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a50a-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/applyDecisions
```
## <a name="request-headers"></a><span data-ttu-id="7a50a-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a50a-128">Request headers</span></span>
| <span data-ttu-id="7a50a-129">Nome</span><span class="sxs-lookup"><span data-stu-id="7a50a-129">Name</span></span>         | <span data-ttu-id="7a50a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a50a-130">Type</span></span>        | <span data-ttu-id="7a50a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a50a-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7a50a-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a50a-132">Authorization</span></span> | <span data-ttu-id="7a50a-133">string</span><span class="sxs-lookup"><span data-stu-id="7a50a-133">string</span></span> | <span data-ttu-id="7a50a-p107">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a50a-p107">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a50a-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a50a-136">Request body</span></span>
<span data-ttu-id="7a50a-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a50a-137">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7a50a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a50a-138">Response</span></span>
<span data-ttu-id="7a50a-p108">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a50a-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a50a-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a50a-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a50a-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a50a-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7a50a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a50a-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
# <a name="c"></a>[<span data-ttu-id="7a50a-144">C#</span><span class="sxs-lookup"><span data-stu-id="7a50a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/apply-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a50a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a50a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/apply-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a50a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a50a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/apply-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7a50a-147">Java</span><span class="sxs-lookup"><span data-stu-id="7a50a-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/apply-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="7a50a-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a50a-148">Response</span></span>
><span data-ttu-id="7a50a-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7a50a-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="7a50a-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="7a50a-150">See also</span></span>

- [<span data-ttu-id="7a50a-151">Como concluir uma revisão de acesso</span><span class="sxs-lookup"><span data-stu-id="7a50a-151">How to complete an access review</span></span>](/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)
