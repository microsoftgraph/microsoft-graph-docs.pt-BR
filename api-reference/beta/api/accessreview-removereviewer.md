---
title: Remover accessReview revisor
description: 'No recurso de avaliações de acesso do Azure AD, atualize um objeto accessReview existente para remover um usuário como um revisor.  Essa operação só é permitida para uma revisão de acesso que ainda não foi concluída e apenas para uma revisão de acesso onde os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do access no qual os usuários revisam sua próprias acesso e não foi projetada para uma revisão de acesso na qual os proprietários do grupo são atribuídos como os revisores. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d3b6ea0fecb6b9179f40fa185aa770a743776eaa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523124"
---
# <a name="remove-accessreview-reviewer"></a><span data-ttu-id="4ac89-105">Remover accessReview revisor</span><span class="sxs-lookup"><span data-stu-id="4ac89-105">Remove accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ac89-106">No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, atualize um objeto [accessReview](../resources/accessreview.md) existente para remover um usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="4ac89-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to remove a user as a reviewer.</span></span>  <span data-ttu-id="4ac89-107">Essa operação só é permitida para uma revisão de acesso que ainda não foi concluída e apenas para uma revisão de acesso onde os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="4ac89-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="4ac89-108">Essa operação não é permitida para uma revisão do access no qual os usuários revisam sua próprias acesso e não foi projetada para uma revisão de acesso na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="4ac89-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="4ac89-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ac89-109">Permissions</span></span>
<span data-ttu-id="4ac89-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ac89-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ac89-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ac89-112">Permission type</span></span>                        | <span data-ttu-id="4ac89-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ac89-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ac89-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ac89-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ac89-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ac89-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="4ac89-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ac89-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ac89-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ac89-117">Not supported.</span></span> |
|<span data-ttu-id="4ac89-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ac89-118">Application</span></span>                            | <span data-ttu-id="4ac89-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ac89-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ac89-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ac89-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('{reviewId}')/reviewers('{userId'})
```
## <a name="request-headers"></a><span data-ttu-id="4ac89-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ac89-121">Request headers</span></span>
| <span data-ttu-id="4ac89-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4ac89-122">Name</span></span>         | <span data-ttu-id="4ac89-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ac89-123">Type</span></span>        | <span data-ttu-id="4ac89-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ac89-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4ac89-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ac89-125">Authorization</span></span> | <span data-ttu-id="4ac89-126">string</span><span class="sxs-lookup"><span data-stu-id="4ac89-126">string</span></span> | <span data-ttu-id="4ac89-127">Token de portador</span><span class="sxs-lookup"><span data-stu-id="4ac89-127">Bearer \{token\}.</span></span> <span data-ttu-id="4ac89-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ac89-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ac89-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ac89-129">Request body</span></span>
<span data-ttu-id="4ac89-130">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="4ac89-130">No request body should be supplied.</span></span>


## <a name="response"></a><span data-ttu-id="4ac89-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ac89-131">Response</span></span>
<span data-ttu-id="4ac89-132">Se tiver êxito, esse método retorna um código de resposta de série 200.</span><span class="sxs-lookup"><span data-stu-id="4ac89-132">If successful, this method returns a 200-series response code.</span></span>

## <a name="example"></a><span data-ttu-id="4ac89-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ac89-133">Example</span></span>

<span data-ttu-id="4ac89-134">Este é um exemplo de atualização de uma única revisão de acesso (não recorrentes) para remover um revisor desnecessário.</span><span class="sxs-lookup"><span data-stu-id="4ac89-134">This is an example of updating a one-time (not reoccurring) access review to remove an unnecessary reviewer.</span></span>


##### <a name="request"></a><span data-ttu-id="4ac89-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ac89-135">Request</span></span>
<span data-ttu-id="4ac89-136">Na URL da solicitação, fornece a id do objeto accessReview e, em seguida, a id do objeto de usuário.</span><span class="sxs-lookup"><span data-stu-id="4ac89-136">In the request URL, supply the id of the accessReview object and then the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_accessReview_reviewer"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers('006111db-0810-4494-a6df-904d368bd81b')

```

##### <a name="response"></a><span data-ttu-id="4ac89-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ac89-137">Response</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-removereviewer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
