---
title: Listar accessReview revisores
description: No Windows Azure AD para acessar o recurso de revisões, recuperar os revisores de um objeto accessReview.
localization_priority: Normal
ms.openlocfilehash: 042887944902be9a603ae0581835c8d55355f8a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829369"
---
# <a name="list-accessreview-reviewers"></a><span data-ttu-id="3727f-103">Listar accessReview revisores</span><span class="sxs-lookup"><span data-stu-id="3727f-103">List accessReview reviewers</span></span>

> <span data-ttu-id="3727f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3727f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3727f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3727f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3727f-106">O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, pode recupere os revisores de um objeto [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="3727f-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, retrieve the reviewers of an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3727f-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="3727f-107">Permissions</span></span>
<span data-ttu-id="3727f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3727f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3727f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3727f-110">Permission type</span></span>                        | <span data-ttu-id="3727f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3727f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3727f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3727f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3727f-113">`AccessReview.Read.All`, `AccessReview.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="3727f-113"></span></span>  <span data-ttu-id="3727f-114">O usuário conectado também deve estar em uma função de diretório que permite que uma revisão de acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="3727f-114">The signed in user must also be in a directory role which permits them to read an access review.</span></span> |
|<span data-ttu-id="3727f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3727f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3727f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3727f-116">Not supported.</span></span> |
|<span data-ttu-id="3727f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3727f-117">Application</span></span>                            | <span data-ttu-id="3727f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3727f-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3727f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3727f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a><span data-ttu-id="3727f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3727f-120">Request headers</span></span>
| <span data-ttu-id="3727f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3727f-121">Name</span></span>         | <span data-ttu-id="3727f-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3727f-122">Type</span></span>        | <span data-ttu-id="3727f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3727f-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="3727f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3727f-124">Authorization</span></span> | <span data-ttu-id="3727f-125">string</span><span class="sxs-lookup"><span data-stu-id="3727f-125">string</span></span> | <span data-ttu-id="3727f-126">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="3727f-126">Bearer \{token\}.</span></span> <span data-ttu-id="3727f-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3727f-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3727f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3727f-128">Request body</span></span>
<span data-ttu-id="3727f-129">Nenhum corpo da solicitação deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="3727f-129">No request body should be supplied.</span></span>

## <a name="response"></a><span data-ttu-id="3727f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3727f-130">Response</span></span>
<span data-ttu-id="3727f-131">Se tiver êxito, este método retornará um `200, OK` código de resposta e uma matriz de objetos [userIdentity](../resources/useridentity.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3727f-131">If successful, this method returns a `200, OK` response code and an array of [userIdentity](../resources/useridentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3727f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3727f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3727f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3727f-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_accessReview_reviewers"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
```

##### <a name="response"></a><span data-ttu-id="3727f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3727f-134">Response</span></span>
><span data-ttu-id="3727f-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3727f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="3727f-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="3727f-137">See also</span></span>

| <span data-ttu-id="3727f-138">Método</span><span class="sxs-lookup"><span data-stu-id="3727f-138">Method</span></span>           | <span data-ttu-id="3727f-139">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3727f-139">Return Type</span></span>    |<span data-ttu-id="3727f-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="3727f-140">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3727f-141">Obter accessReview</span><span class="sxs-lookup"><span data-stu-id="3727f-141">Get accessReview</span></span>](accessreview-get.md) |  [<span data-ttu-id="3727f-142">accessReview</span><span class="sxs-lookup"><span data-stu-id="3727f-142">accessReview</span></span>](../resources/accessreview.md) |  <span data-ttu-id="3727f-143">Recupere uma revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="3727f-143">Retrieve an access review.</span></span> |
|[<span data-ttu-id="3727f-144">Adicionar Revisor accessReview</span><span class="sxs-lookup"><span data-stu-id="3727f-144">Add accessReview reviewer</span></span>](accessreview-addreviewer.md) |     <span data-ttu-id="3727f-145">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3727f-145">None.</span></span>   |   <span data-ttu-id="3727f-146">Adicione um revisor a um accessReview.</span><span class="sxs-lookup"><span data-stu-id="3727f-146">Add a reviewer to an accessReview.</span></span> |
|[<span data-ttu-id="3727f-147">Remover accessReview revisor</span><span class="sxs-lookup"><span data-stu-id="3727f-147">Remove accessReview reviewer</span></span>](accessreview-removereviewer.md) | <span data-ttu-id="3727f-148">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3727f-148">None.</span></span> |   <span data-ttu-id="3727f-149">Remova um revisor de um accessReview.</span><span class="sxs-lookup"><span data-stu-id="3727f-149">Remove a reviewer from an accessReview.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview reviewers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
