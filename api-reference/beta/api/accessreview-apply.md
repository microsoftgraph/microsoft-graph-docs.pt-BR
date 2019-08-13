---
title: Aplicar accessReview
description: 'No recurso de revisões do Azure AD Access, aplique as decisões de um accessReview concluído.  O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b012e1a23a0641c7abd5cc6c763481c251f961dd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313034"
---
# <a name="apply-accessreview"></a><span data-ttu-id="91124-104">Aplicar accessReview</span><span class="sxs-lookup"><span data-stu-id="91124-104">Apply accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91124-105">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , aplique as decisões de um [accessReview](../resources/accessreview.md)concluído.</span><span class="sxs-lookup"><span data-stu-id="91124-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, apply the decisions of a completed [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="91124-106">O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="91124-106">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  


<span data-ttu-id="91124-107">Após a conclusão da revisão do Access, porque ela atingiu a data de término ou um administrador o interrompeu manualmente e a aplicação automática não foi configurada para a revisão, você pode chamar aplicar para aplicar as alterações.</span><span class="sxs-lookup"><span data-stu-id="91124-107">After an access review is finished, either because it reached the end date or an administrator stopped it manually, and auto-apply wasn't configured for the review, you can call Apply to apply the changes.</span></span> <span data-ttu-id="91124-108">Até a aplicação ocorrer, as decisões para remover os direitos de acesso não aparecem no recurso de origem, os usuários da instância retêm suas associações de grupo.</span><span class="sxs-lookup"><span data-stu-id="91124-108">Until apply occurs, the decisions to remove access rights do not appear on the source resource, the users for instance retain their group memberships.</span></span> <span data-ttu-id="91124-109">Ao chamar Apply, o resultado da revisão é implementado atualizando o grupo ou aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91124-109">By calling apply, the outcome of the review is implemented by updating the group or application.</span></span> <span data-ttu-id="91124-110">Se o acesso de um usuário tiver sido negado na revisão, quando um administrador chamar essa API, o Azure AD removerá sua associação ou atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="91124-110">If a user's access was denied in the review, when an administrator calls this API, Azure AD removes their membership or application assignment.</span></span> 

<span data-ttu-id="91124-111">Após a conclusão da revisão do Access, e a aplicação automática tiver sido configurada, o status da revisão será alterado de concluído através de Estados intermediários e, por fim, será alterado para estado aplicado.</span><span class="sxs-lookup"><span data-stu-id="91124-111">After an access review is finished, and auto-apply was configured, then the status of the review will change from Completed through intermediate states and finally will change to state Applied.</span></span> <span data-ttu-id="91124-112">Você deve esperar ver os usuários negados, se houver, removidos da Associação de grupo de recursos ou da atribuição de aplicativo em alguns minutos.</span><span class="sxs-lookup"><span data-stu-id="91124-112">You should expect to see denied users, if any, being removed from the resource group membership or app assignment in a few minutes.</span></span>

<span data-ttu-id="91124-113">Uma revisão de aplicação automática configurada ou a seleção de aplicar não tem efeito em um grupo que se origina em um diretório local ou em um grupo dinâmico.</span><span class="sxs-lookup"><span data-stu-id="91124-113">A configured auto applying review, or selecting Apply doesn't have an effect on a group that originates in an on-premises directory or a dynamic group.</span></span> <span data-ttu-id="91124-114">Se você quiser alterar um grupo que originou o local, baixe os resultados e aplique essas alterações à representação do grupo nesse diretório.</span><span class="sxs-lookup"><span data-stu-id="91124-114">If you want to change a group that originates on-premises, download the results and apply those changes to the representation of the group in that directory.</span></span>


## <a name="permissions"></a><span data-ttu-id="91124-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="91124-115">Permissions</span></span>
<span data-ttu-id="91124-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91124-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91124-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91124-118">Permission type</span></span>                        | <span data-ttu-id="91124-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91124-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="91124-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91124-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="91124-121">AccessReview. ReadWrite. Membership, AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="91124-121">AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="91124-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91124-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91124-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91124-123">Not supported.</span></span> |
|<span data-ttu-id="91124-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91124-124">Application</span></span>                            | <span data-ttu-id="91124-125">AccessReview. ReadWrite. Membership</span><span class="sxs-lookup"><span data-stu-id="91124-125">AccessReview.ReadWrite.Membership</span></span> |

## <a name="http-request"></a><span data-ttu-id="91124-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91124-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="91124-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91124-127">Request headers</span></span>
| <span data-ttu-id="91124-128">Nome</span><span class="sxs-lookup"><span data-stu-id="91124-128">Name</span></span>         | <span data-ttu-id="91124-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="91124-129">Type</span></span>        | <span data-ttu-id="91124-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="91124-130">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="91124-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="91124-131">Authorization</span></span> | <span data-ttu-id="91124-132">string</span><span class="sxs-lookup"><span data-stu-id="91124-132">string</span></span> | <span data-ttu-id="91124-p107">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91124-p107">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91124-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91124-135">Request body</span></span>
<span data-ttu-id="91124-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="91124-136">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="91124-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="91124-137">Response</span></span>
<span data-ttu-id="91124-p108">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91124-p108">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="see-also"></a><span data-ttu-id="91124-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="91124-140">See also</span></span>

- [<span data-ttu-id="91124-141">Como concluir uma revisão do Access</span><span class="sxs-lookup"><span data-stu-id="91124-141">How to complete an access review</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a><span data-ttu-id="91124-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91124-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91124-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91124-143">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="91124-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="91124-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="91124-145">C#</span><span class="sxs-lookup"><span data-stu-id="91124-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/apply-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="91124-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91124-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/apply-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="91124-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="91124-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/apply-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="91124-148">Java</span><span class="sxs-lookup"><span data-stu-id="91124-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/apply-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="91124-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="91124-149">Response</span></span>
><span data-ttu-id="91124-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91124-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
