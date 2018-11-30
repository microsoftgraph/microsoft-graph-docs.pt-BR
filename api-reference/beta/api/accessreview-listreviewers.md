---
title: Listar accessReview revisores
description: No Windows Azure AD para acessar o recurso de revisões, recuperar os revisores de um objeto accessReview.
ms.openlocfilehash: 24c8b3dacbbe1a5868c9ba82141f37b006dc7a75
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034654"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="74567-103">Listar accessReview revisores</span><span class="sxs-lookup"><span data-stu-id="74567-103">List accessReview reviewers</span></span>

> <span data-ttu-id="74567-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="74567-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74567-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="74567-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74567-106">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, pode recupere os revisores de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="74567-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="74567-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="74567-107">Permissions</span></span>
<span data-ttu-id="74567-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74567-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74567-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74567-110">Permission type</span></span>                        | <span data-ttu-id="74567-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74567-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="74567-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74567-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="74567-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="74567-113"></span></span>  <span data-ttu-id="74567-114">O usuário conectado também deve estar em uma função de diretório que permite que uma revisão de acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="74567-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="74567-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74567-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74567-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74567-116">Not supported.</span></span> |
|<span data-ttu-id="74567-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74567-117">Application</span></span>                            | <span data-ttu-id="74567-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74567-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="74567-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74567-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="74567-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74567-120">Request headers</span></span>
| <span data-ttu-id="74567-121">Nome</span><span class="sxs-lookup"><span data-stu-id="74567-121">Name</span></span>         | <span data-ttu-id="74567-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="74567-122">Type</span></span>        | <span data-ttu-id="74567-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="74567-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="74567-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="74567-124">Authorization</span></span> | <span data-ttu-id="74567-125">string</span><span class="sxs-lookup"><span data-stu-id="74567-125">string</span></span> | <span data-ttu-id="74567-126">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="74567-126">Bearer \{token\}.</span></span> <span data-ttu-id="74567-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74567-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74567-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74567-128">Request body</span></span>
<span data-ttu-id="74567-129">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="74567-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="74567-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="74567-130">Response</span></span>
<span data-ttu-id="74567-131">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [userIdentity](../resources/useridentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74567-131">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74567-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74567-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74567-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74567-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="74567-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="74567-134">Response</span></span>
><span data-ttu-id="74567-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74567-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="74567-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="74567-137">See also</span></span>

| <span data-ttu-id="74567-138">Método</span><span class="sxs-lookup"><span data-stu-id="74567-138">Method</span></span>           | <span data-ttu-id="74567-139">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74567-139">Return Type</span></span>    |<span data-ttu-id="74567-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="74567-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74567-141">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="74567-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="74567-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="74567-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="74567-143">Recupere uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="74567-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="74567-144">Adicionar Revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="74567-144">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="74567-145">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74567-145">None.</span></span>   |   <span data-ttu-id="74567-146">Adicione um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="74567-146">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="74567-147">Remover accessReview revisor</span><span class="sxs-lookup"><span data-stu-id="74567-147">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="74567-148">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74567-148">None.</span></span> |   <span data-ttu-id="74567-149">Remova um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="74567-149">Remove a reviewer from an accessReview.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
