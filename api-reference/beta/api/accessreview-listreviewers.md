---
title: Listar accessReview revisores
description: No Windows Azure AD para acessar o recurso de revisões, recuperar os revisores de um objeto accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8dca759f71f13af18c291f1af9843da6729ef701
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946809"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="e7e2d-103">Listar accessReview revisores</span><span class="sxs-lookup"><span data-stu-id="e7e2d-103">List accessReview reviewers</span></span>

> <span data-ttu-id="e7e2d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7e2d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e7e2d-106">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, pode recupere os revisores de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="e7e2d-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7e2d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e7e2d-107">Permissions</span></span>
<span data-ttu-id="e7e2d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7e2d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7e2d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7e2d-110">Permission type</span></span>                        | <span data-ttu-id="e7e2d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e7e2d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7e2d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7e2d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e7e2d-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-113"></span></span>  <span data-ttu-id="e7e2d-114">O usuário conectado também deve estar em uma função de diretório que permite que uma revisão de acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="e7e2d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7e2d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7e2d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-116">Not supported.</span></span> |
|<span data-ttu-id="e7e2d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7e2d-117">Application</span></span>                            | <span data-ttu-id="e7e2d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7e2d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7e2d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="e7e2d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7e2d-120">Request headers</span></span>
| <span data-ttu-id="e7e2d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e7e2d-121">Name</span></span>         | <span data-ttu-id="e7e2d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7e2d-122">Type</span></span>        | <span data-ttu-id="e7e2d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7e2d-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="e7e2d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7e2d-124">Authorization</span></span> | <span data-ttu-id="e7e2d-125">string</span><span class="sxs-lookup"><span data-stu-id="e7e2d-125">string</span></span> | <span data-ttu-id="e7e2d-126">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-126">Bearer \{token\}.</span></span> <span data-ttu-id="e7e2d-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7e2d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7e2d-128">Request body</span></span>
<span data-ttu-id="e7e2d-129">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="e7e2d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7e2d-130">Response</span></span>
<span data-ttu-id="e7e2d-131">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [userIdentity](../resources/useridentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-131">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7e2d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7e2d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7e2d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7e2d-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="e7e2d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7e2d-134">Response</span></span>
><span data-ttu-id="e7e2d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e7e2d-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="e7e2d-137">See also</span></span>

| <span data-ttu-id="e7e2d-138">Método</span><span class="sxs-lookup"><span data-stu-id="e7e2d-138">Method</span></span>           | <span data-ttu-id="e7e2d-139">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e7e2d-139">Return Type</span></span>    |<span data-ttu-id="e7e2d-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7e2d-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e7e2d-141">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="e7e2d-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="e7e2d-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="e7e2d-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="e7e2d-143">Recupere uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="e7e2d-144">Adicionar Revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="e7e2d-144">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="e7e2d-145">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-145">None.</span></span>   |   <span data-ttu-id="e7e2d-146">Adicione um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-146">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="e7e2d-147">Remover accessReview revisor</span><span class="sxs-lookup"><span data-stu-id="e7e2d-147">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="e7e2d-148">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-148">None.</span></span> |   <span data-ttu-id="e7e2d-149">Remova um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="e7e2d-149">Remove a reviewer from an accessReview.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
