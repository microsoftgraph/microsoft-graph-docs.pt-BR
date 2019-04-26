---
title: Remover revisor accessReview
description: 'No recurso de revisões do Azure AD Access, atualize um objeto accessReview existente para remover um usuário como um revisor.  Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7c2b80659ae1f9d4ce547a9d64d81f1fdb0403c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33323087"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="bdc0f-105">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="bdc0f-105">Remove accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdc0f-106">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , atualize um objeto [accessReview](../resources/accessreview.md) existente para remover um usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="bdc0f-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="bdc0f-107">Essa operação só é permitida para uma revisão do Access que ainda não foi concluída e somente para uma revisão do Access em que os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="bdc0f-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="bdc0f-108">Essa operação não é permitida para uma revisão do Access na qual os usuários revisam seu próprio acesso e não se destinam a uma revisão do Access na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="bdc0f-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="bdc0f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdc0f-109">Permissions</span></span>
<span data-ttu-id="bdc0f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdc0f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdc0f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdc0f-112">Permission type</span></span>                        | <span data-ttu-id="bdc0f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdc0f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdc0f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdc0f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdc0f-115">AccessReview. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bdc0f-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="bdc0f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdc0f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdc0f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdc0f-117">Not supported.</span></span> |
|<span data-ttu-id="bdc0f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdc0f-118">Application</span></span>                            | <span data-ttu-id="bdc0f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdc0f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdc0f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdc0f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="bdc0f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdc0f-121">Request headers</span></span>
| <span data-ttu-id="bdc0f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bdc0f-122">Name</span></span>         | <span data-ttu-id="bdc0f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdc0f-123">Type</span></span>        | <span data-ttu-id="bdc0f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdc0f-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bdc0f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdc0f-125">Authorization</span></span> | <span data-ttu-id="bdc0f-126">string</span><span class="sxs-lookup"><span data-stu-id="bdc0f-126">string</span></span> | <span data-ttu-id="bdc0f-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdc0f-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdc0f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdc0f-129">Request body</span></span>
<span data-ttu-id="bdc0f-130">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="bdc0f-130">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="bdc0f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdc0f-131">Response</span></span>
<span data-ttu-id="bdc0f-132">Se tiver êxito, este método retornará um código de resposta da série 200.</span><span class="sxs-lookup"><span data-stu-id="bdc0f-132">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="bdc0f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdc0f-133">Example</span></span>

<span data-ttu-id="bdc0f-134">Este é um exemplo de atualização de um modo de exibição de acesso de uma única vez (não repetido) para remover um revisor desnecessário.</span><span class="sxs-lookup"><span data-stu-id="bdc0f-134">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="bdc0f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdc0f-135">Request</span></span>
<span data-ttu-id="bdc0f-136">Na URL da solicitação, forneça a ID do objeto accessReview e, em seguida, a ID do objeto user.</span><span class="sxs-lookup"><span data-stu-id="bdc0f-136">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers/006111db-0810-4494-a6df-904d368bd81b

```

##### <a name="response"></a><span data-ttu-id="bdc0f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdc0f-137">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!--
{
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
