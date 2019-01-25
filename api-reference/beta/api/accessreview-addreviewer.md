---
title: Adicionar Revisor accessReview
description: 'No recurso de avaliações de acesso do Azure AD, atualize um objeto accessReview existente para adicionar outro usuário como um revisor.  Essa operação só é permitida para uma revisão de acesso que ainda não foi concluída e apenas para uma revisão de acesso onde os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do access no qual os usuários revisam sua próprias acesso e não foi projetada para uma revisão de acesso na qual os proprietários do grupo são atribuídos como os revisores. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1a526451330321c7fbbfd1d5287dd5ad892eee84
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516361"
---
# <a name="add-accessreview-reviewer"></a><span data-ttu-id="4be72-105">Adicionar Revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="4be72-105">Add accessReview reviewer</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4be72-106">No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, atualize um objeto [accessReview](../resources/accessreview.md) existente para adicionar outro usuário como um revisor.</span><span class="sxs-lookup"><span data-stu-id="4be72-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [accessReview](../resources/accessreview.md) object to add another user as a reviewer.</span></span>  <span data-ttu-id="4be72-107">Essa operação só é permitida para uma revisão de acesso que ainda não foi concluída e apenas para uma revisão de acesso onde os revisores são explicitamente especificados.</span><span class="sxs-lookup"><span data-stu-id="4be72-107">This operation is only permitted for an access review that is not yet completed, and only for an access review where the reviewers are explicitly specified.</span></span> <span data-ttu-id="4be72-108">Essa operação não é permitida para uma revisão do access no qual os usuários revisam sua próprias acesso e não foi projetada para uma revisão de acesso na qual os proprietários do grupo são atribuídos como os revisores.</span><span class="sxs-lookup"><span data-stu-id="4be72-108">This operation is not permitted for an access review in which users review their own access, and not intended for an access review in which the group owners are assigned as the reviewers.</span></span> 


## <a name="permissions"></a><span data-ttu-id="4be72-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4be72-109">Permissions</span></span>
<span data-ttu-id="4be72-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4be72-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4be72-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4be72-112">Permission type</span></span>                        | <span data-ttu-id="4be72-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4be72-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4be72-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4be72-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4be72-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4be72-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="4be72-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4be72-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4be72-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4be72-117">Not supported.</span></span> |
|<span data-ttu-id="4be72-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4be72-118">Application</span></span>                            | <span data-ttu-id="4be72-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4be72-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4be72-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4be72-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="4be72-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4be72-121">Request headers</span></span>
| <span data-ttu-id="4be72-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4be72-122">Name</span></span>         | <span data-ttu-id="4be72-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="4be72-123">Type</span></span>        | <span data-ttu-id="4be72-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4be72-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4be72-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4be72-125">Authorization</span></span> | <span data-ttu-id="4be72-126">string</span><span class="sxs-lookup"><span data-stu-id="4be72-126">string</span></span> | <span data-ttu-id="4be72-127">Token de portador</span><span class="sxs-lookup"><span data-stu-id="4be72-127">Bearer \{token\}.</span></span> <span data-ttu-id="4be72-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4be72-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4be72-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4be72-129">Request body</span></span>
<span data-ttu-id="4be72-130">No corpo da solicitação, fornece uma representação JSON da ID de um usuário que será um revisor.</span><span class="sxs-lookup"><span data-stu-id="4be72-130">In the request body, supply a JSON representation of the ID of a user who will be a reviewer.</span></span>

<span data-ttu-id="4be72-131">A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um accessReview.</span><span class="sxs-lookup"><span data-stu-id="4be72-131">The following table shows the properties that can be supplied when you update an accessReview.</span></span>

| <span data-ttu-id="4be72-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4be72-132">Property</span></span>     | <span data-ttu-id="4be72-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="4be72-133">Type</span></span>        | <span data-ttu-id="4be72-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="4be72-134">Description</span></span> |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | <span data-ttu-id="4be72-135">ID do usuário.</span><span class="sxs-lookup"><span data-stu-id="4be72-135">The user ID.</span></span>  |


## <a name="response"></a><span data-ttu-id="4be72-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4be72-136">Response</span></span>
<span data-ttu-id="4be72-137">Se tiver êxito, este método retornará um `201, Created` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="4be72-137">If successful, this method returns a `201, Created` response code .</span></span>

## <a name="example"></a><span data-ttu-id="4be72-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4be72-138">Example</span></span>

<span data-ttu-id="4be72-139">Este é um exemplo de como atualizar uma revisão de acesso (não recorrentes) ocasional com um revisor adicional.</span><span class="sxs-lookup"><span data-stu-id="4be72-139">This is an example of updating a one-time (not reoccurring) access review with an additional reviewer.</span></span>

##### <a name="request"></a><span data-ttu-id="4be72-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4be72-140">Request</span></span>
<span data-ttu-id="4be72-141">No corpo da solicitação, fornece uma representação JSON da id do objeto de usuário.</span><span class="sxs-lookup"><span data-stu-id="4be72-141">In the request body, supply a JSON representation of the id of the user object.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
Content-type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```

##### <a name="response"></a><span data-ttu-id="4be72-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4be72-142">Response</span></span>
><span data-ttu-id="4be72-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4be72-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-addreviewer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
