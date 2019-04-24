---
title: Listar revisores do accessReview
description: No recurso de revisões do Azure AD Access, recupere os revisores de um objeto accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d2227ed6343900780df57aeece2fe511f07da04f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459413"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="bbdd3-103">Listar revisores do accessReview</span><span class="sxs-lookup"><span data-stu-id="bbdd3-103">List accessReview reviewers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbdd3-104">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere os revisores de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="bbdd3-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bbdd3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbdd3-105">Permissions</span></span>
<span data-ttu-id="bbdd3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbdd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbdd3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbdd3-108">Permission type</span></span>                        | <span data-ttu-id="bbdd3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbdd3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbdd3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbdd3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bbdd3-111">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="bbdd3-111"></span></span>  <span data-ttu-id="bbdd3-112">O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="bbdd3-112">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="bbdd3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbdd3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbdd3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbdd3-114">Not supported.</span></span> |
|<span data-ttu-id="bbdd3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbdd3-115">Application</span></span>                            | <span data-ttu-id="bbdd3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbdd3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbdd3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbdd3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="bbdd3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbdd3-118">Request headers</span></span>
| <span data-ttu-id="bbdd3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bbdd3-119">Name</span></span>         | <span data-ttu-id="bbdd3-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbdd3-120">Type</span></span>        | <span data-ttu-id="bbdd3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbdd3-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bbdd3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbdd3-122">Authorization</span></span> | <span data-ttu-id="bbdd3-123">string</span><span class="sxs-lookup"><span data-stu-id="bbdd3-123">string</span></span> | <span data-ttu-id="bbdd3-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbdd3-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbdd3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbdd3-126">Request body</span></span>
<span data-ttu-id="bbdd3-127">Nenhum corpo de solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="bbdd3-127">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="bbdd3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbdd3-128">Response</span></span>
<span data-ttu-id="bbdd3-129">Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos UserIdentity no corpo da resposta. [](../resources/useridentity.md)</span><span class="sxs-lookup"><span data-stu-id="bbdd3-129">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbdd3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbdd3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbdd3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbdd3-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="bbdd3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbdd3-132">Response</span></span>
><span data-ttu-id="bbdd3-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbdd3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bbdd3-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="bbdd3-135">See also</span></span>

| <span data-ttu-id="bbdd3-136">Método</span><span class="sxs-lookup"><span data-stu-id="bbdd3-136">Method</span></span>           | <span data-ttu-id="bbdd3-137">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bbdd3-137">Return Type</span></span>    |<span data-ttu-id="bbdd3-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbdd3-138">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bbdd3-139">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="bbdd3-139">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="bbdd3-140">accessReview</span><span class="sxs-lookup"><span data-stu-id="bbdd3-140">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="bbdd3-141">Recupere uma revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="bbdd3-141">Retrieve an access review.</span></span> |
|[<span data-ttu-id="bbdd3-142">Adicionar revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="bbdd3-142">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="bbdd3-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbdd3-143">None.</span></span>   |   <span data-ttu-id="bbdd3-144">Adicionar um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="bbdd3-144">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="bbdd3-145">Remover revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="bbdd3-145">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="bbdd3-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbdd3-146">None.</span></span> |   <span data-ttu-id="bbdd3-147">Remover um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="bbdd3-147">Remove a reviewer from an accessReview.</span></span> |


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
