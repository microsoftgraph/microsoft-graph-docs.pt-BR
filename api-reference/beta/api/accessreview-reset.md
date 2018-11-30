---
title: Redefinir accessReview
description: No recurso de avaliações de acesso do Azure AD, redefina as decisões de um accessReview ativa no momento.  O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.  Decisões anteriores não são mais registradas, mas os revisores podem continuar a atualização decisões.
ms.openlocfilehash: b633a56926b56b33c509214d7574971056831967
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034347"
---
# <a name="reset-accessreview"></a><span data-ttu-id="cd02c-105">Redefinir accessReview</span><span class="sxs-lookup"><span data-stu-id="cd02c-105">Reset accessReview</span></span>

> <span data-ttu-id="cd02c-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cd02c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd02c-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cd02c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd02c-108">No Windows Azure AD [access analisa](../resources/accessreviews-root.md) recurso, redefina as decisões de um ativo no momento [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="cd02c-108">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="cd02c-109">O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="cd02c-109">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="cd02c-110">Decisões anteriores não são mais registradas, mas os revisores podem continuar a atualização decisões.</span><span class="sxs-lookup"><span data-stu-id="cd02c-110">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd02c-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="cd02c-111">Permissions</span></span>
<span data-ttu-id="cd02c-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd02c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd02c-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd02c-114">Permission type</span></span>                        | <span data-ttu-id="cd02c-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd02c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd02c-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd02c-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd02c-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd02c-117">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="cd02c-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd02c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd02c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd02c-119">Not supported.</span></span> |
|<span data-ttu-id="cd02c-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd02c-120">Application</span></span>                            | <span data-ttu-id="cd02c-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd02c-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd02c-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd02c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="cd02c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd02c-123">Request headers</span></span>
| <span data-ttu-id="cd02c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="cd02c-124">Name</span></span>         | <span data-ttu-id="cd02c-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd02c-125">Type</span></span>        | <span data-ttu-id="cd02c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd02c-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cd02c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd02c-127">Authorization</span></span> | <span data-ttu-id="cd02c-128">string</span><span class="sxs-lookup"><span data-stu-id="cd02c-128">string</span></span> | <span data-ttu-id="cd02c-129">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="cd02c-129">Bearer \{token\}.</span></span> <span data-ttu-id="cd02c-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd02c-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd02c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd02c-131">Request body</span></span>
<span data-ttu-id="cd02c-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd02c-132">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="cd02c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd02c-133">Response</span></span>
<span data-ttu-id="cd02c-p106">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd02c-p106">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd02c-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd02c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd02c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd02c-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/resetDecisions()
```
##### <a name="response"></a><span data-ttu-id="cd02c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd02c-138">Response</span></span>
><span data-ttu-id="cd02c-p107">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd02c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
