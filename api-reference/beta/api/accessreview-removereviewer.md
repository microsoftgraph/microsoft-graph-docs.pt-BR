---
title: Remover accessReview revisor
description: 'No recurso de avaliações de acesso do Azure AD, atualize um objeto accessReview existente para remover um usuário como um revisor.  Essa operação só é permitida para uma revisão de acesso que ainda não foi concluída e apenas para uma revisão de acesso onde os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do access no qual os usuários revisam sua próprias acesso e não foi projetada para uma revisão de acesso na qual os proprietários do grupo são atribuídos como os revisores. '
localization_priority: Normal
ms.openlocfilehash: d33c1c2409b866a48d0684612f8c878e14dedb68
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866021"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="faebe-105">Remover accessReview revisor</span><span class="sxs-lookup"><span data-stu-id="faebe-105">Remove accessReview reviewer</span></span>

> <span data-ttu-id="faebe-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="faebe-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="faebe-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="faebe-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="faebe-108">No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, atualize um objeto [accessReview](../resources/accessreview.md) existente para remover um usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="faebe-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="faebe-109">Essa operação só é permitida para uma revisão de acesso que ainda não foi concluída e apenas para uma revisão de acesso onde os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="faebe-109">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="faebe-110">Essa operação não é permitida para uma revisão do access no qual os usuários revisam sua próprias acesso e não foi projetada para uma revisão de acesso na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="faebe-110">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="faebe-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="faebe-111">Permissions</span></span>
<span data-ttu-id="faebe-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faebe-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faebe-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="faebe-114">Permission type</span></span>                        | <span data-ttu-id="faebe-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="faebe-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="faebe-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="faebe-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="faebe-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faebe-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="faebe-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="faebe-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="faebe-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="faebe-119">Not supported.</span></span> |
|<span data-ttu-id="faebe-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="faebe-120">Application</span></span>                            | <span data-ttu-id="faebe-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="faebe-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="faebe-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="faebe-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="faebe-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="faebe-123">Request headers</span></span>
| <span data-ttu-id="faebe-124">Nome</span><span class="sxs-lookup"><span data-stu-id="faebe-124">Name</span></span>         | <span data-ttu-id="faebe-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="faebe-125">Type</span></span>        | <span data-ttu-id="faebe-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="faebe-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="faebe-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="faebe-127">Authorization</span></span> | <span data-ttu-id="faebe-128">string</span><span class="sxs-lookup"><span data-stu-id="faebe-128">string</span></span> | <span data-ttu-id="faebe-129">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="faebe-129">Bearer \{token\}.</span></span> <span data-ttu-id="faebe-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="faebe-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="faebe-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="faebe-131">Request body</span></span>
<span data-ttu-id="faebe-132">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="faebe-132">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="faebe-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="faebe-133">Response</span></span>
<span data-ttu-id="faebe-134">Se tiver êxito, esse método retorna um código de resposta de série 200.</span><span class="sxs-lookup"><span data-stu-id="faebe-134">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="faebe-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="faebe-135">Example</span></span>

<span data-ttu-id="faebe-136">Este é um exemplo de atualização de uma única revisão de acesso (não recorrentes) para remover um revisor desnecessário.</span><span class="sxs-lookup"><span data-stu-id="faebe-136">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="faebe-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="faebe-137">Request</span></span>
<span data-ttu-id="faebe-138">Na URL da solicitação, fornece a id do objeto accessReview e, em seguida, a id do objeto de usuário.</span><span class="sxs-lookup"><span data-stu-id="faebe-138">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers('006111db-0810-4494-a6df-904d368bd81b')

```

##### <a name="response"></a><span data-ttu-id="faebe-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="faebe-139">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No content
```

<!-- {
  "type": "#page.annotation",
  "description": "Remove accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
