---
title: Listar accessReview revisores
description: No Windows Azure AD para acessar o recurso de revisões, recuperar os revisores de um objeto accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d2227ed6343900780df57aeece2fe511f07da04f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529275"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="c38ea-103">Listar accessReview revisores</span><span class="sxs-lookup"><span data-stu-id="c38ea-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c38ea-104">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, pode recupere os revisores de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="c38ea-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c38ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c38ea-105">Permissions</span></span>
<span data-ttu-id="c38ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c38ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c38ea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c38ea-108">Permission type</span></span>                        | <span data-ttu-id="c38ea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c38ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c38ea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c38ea-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c38ea-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="c38ea-111"></span></span>  <span data-ttu-id="c38ea-112">O usuário conectado também deve estar em uma função de diretório que permite que uma revisão de acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="c38ea-112">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="c38ea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c38ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c38ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c38ea-114">Not supported.</span></span> |
|<span data-ttu-id="c38ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c38ea-115">Application</span></span>                            | <span data-ttu-id="c38ea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c38ea-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c38ea-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c38ea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="c38ea-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c38ea-118">Request headers</span></span>
| <span data-ttu-id="c38ea-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c38ea-119">Name</span></span>         | <span data-ttu-id="c38ea-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c38ea-120">Type</span></span>        | <span data-ttu-id="c38ea-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c38ea-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c38ea-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c38ea-122">Authorization</span></span> | <span data-ttu-id="c38ea-123">string</span><span class="sxs-lookup"><span data-stu-id="c38ea-123">string</span></span> | <span data-ttu-id="c38ea-124">Token de portador</span><span class="sxs-lookup"><span data-stu-id="c38ea-124">Bearer \{token\}.</span></span> <span data-ttu-id="c38ea-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c38ea-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c38ea-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c38ea-126">Request body</span></span>
<span data-ttu-id="c38ea-127">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="c38ea-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="c38ea-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c38ea-128">Response</span></span>
<span data-ttu-id="c38ea-129">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [userIdentity](../resources/useridentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c38ea-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c38ea-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c38ea-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c38ea-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c38ea-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="c38ea-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c38ea-132">Response</span></span>
><span data-ttu-id="c38ea-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c38ea-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userIdentity",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
       "id":"006111db-0810-4494-a6df-904d368bd81b"
    }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="c38ea-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="c38ea-135">See also</span></span>

| <span data-ttu-id="c38ea-136">Método</span><span class="sxs-lookup"><span data-stu-id="c38ea-136">Method</span></span>           | <span data-ttu-id="c38ea-137">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c38ea-137">Return Type</span></span>    |<span data-ttu-id="c38ea-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="c38ea-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c38ea-139">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="c38ea-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="c38ea-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="c38ea-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="c38ea-141">Recupere uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="c38ea-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="c38ea-142">Adicionar Revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="c38ea-142">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="c38ea-143">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c38ea-143">None.</span></span>   |   <span data-ttu-id="c38ea-144">Adicione um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="c38ea-144">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="c38ea-145">Remover accessReview revisor</span><span class="sxs-lookup"><span data-stu-id="c38ea-145">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="c38ea-146">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c38ea-146">None.</span></span> |   <span data-ttu-id="c38ea-147">Remova um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="c38ea-147">Remove a reviewer from an accessReview.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listreviewers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
