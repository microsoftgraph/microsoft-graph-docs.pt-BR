---
title: Parar accessReview
description: No recurso de revisões do Azure AD Access, interrompa um accessReview ativo no momento.  O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.  Para impedir que uma revisão de acesso recorrente inicie instâncias futuras, atualize-a para alterar sua data de término agendada.  Depois que a revisão do Access for interrompida, os revisores não poderão mais fornecer entradas e as decisões de revisão do Access poderão ser aplicadas.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bbce4cf62a849a2ec70a84c1c953ab1064aca2fa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439998"
---
# <a name="stop-accessreview"></a><span data-ttu-id="4d3c3-106">Parar accessReview</span><span class="sxs-lookup"><span data-stu-id="4d3c3-106">Stop accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d3c3-107">No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , interrompa um [accessReview](../resources/accessreview.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="4d3c3-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, stop a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="4d3c3-108">O objeto de destino pode ser uma revisão de acesso única ou uma instância de uma revisão de acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="4d3c3-108">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="4d3c3-109">Para impedir que uma revisão de acesso recorrente inicie instâncias futuras, [atualize-](accessreview-update.md) a para alterar sua data de término agendada.</span><span class="sxs-lookup"><span data-stu-id="4d3c3-109">(To prevent a recurring access review from starting future instances, [update it](accessreview-update.md) to change its scheduled end date).</span></span>  <span data-ttu-id="4d3c3-110">Depois que a revisão do Access for interrompida, os revisores não poderão mais fornecer entradas e as decisões de revisão do Access poderão ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="4d3c3-110">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="4d3c3-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d3c3-111">Permissions</span></span>
<span data-ttu-id="4d3c3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d3c3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d3c3-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d3c3-114">Permission type</span></span>                        | <span data-ttu-id="4d3c3-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d3c3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d3c3-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d3c3-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d3c3-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d3c3-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="4d3c3-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d3c3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d3c3-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d3c3-119">Not supported.</span></span> |
|<span data-ttu-id="4d3c3-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d3c3-120">Application</span></span>                            | <span data-ttu-id="4d3c3-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d3c3-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4d3c3-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d3c3-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a><span data-ttu-id="4d3c3-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d3c3-123">Request headers</span></span>
| <span data-ttu-id="4d3c3-124">Nome</span><span class="sxs-lookup"><span data-stu-id="4d3c3-124">Name</span></span>         | <span data-ttu-id="4d3c3-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d3c3-125">Type</span></span>        | <span data-ttu-id="4d3c3-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d3c3-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4d3c3-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d3c3-127">Authorization</span></span> | <span data-ttu-id="4d3c3-128">string</span><span class="sxs-lookup"><span data-stu-id="4d3c3-128">string</span></span> | <span data-ttu-id="4d3c3-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d3c3-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d3c3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d3c3-131">Request body</span></span>
<span data-ttu-id="4d3c3-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d3c3-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4d3c3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d3c3-133">Response</span></span>
<span data-ttu-id="4d3c3-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d3c3-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d3c3-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d3c3-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d3c3-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d3c3-137">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4d3c3-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d3c3-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4d3c3-139">C#</span><span class="sxs-lookup"><span data-stu-id="4d3c3-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d3c3-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d3c3-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4d3c3-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4d3c3-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4d3c3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d3c3-142">Response</span></span>
><span data-ttu-id="4d3c3-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d3c3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
