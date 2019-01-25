---
title: Redefinir accessReview
description: No recurso de avaliações de acesso do Azure AD, redefina as decisões de um accessReview ativa no momento.  O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.  Decisões anteriores não são mais registradas, mas os revisores podem continuar a atualização decisões.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4e258a781707d2c3fe5419e3ebd5f7c6b43f271b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517012"
---
# <a name="reset-accessreview"></a><span data-ttu-id="0cd38-105">Redefinir accessReview</span><span class="sxs-lookup"><span data-stu-id="0cd38-105">Reset accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cd38-106">No Windows Azure AD [access analisa](../resources/accessreviews-root.md) recurso, redefina as decisões de um ativo no momento [accessReview](../resources/accessreview.md).</span><span class="sxs-lookup"><span data-stu-id="0cd38-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, reset the decisions of a currently active [accessReview](../resources/accessreview.md).</span></span>  <span data-ttu-id="0cd38-107">O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.</span><span class="sxs-lookup"><span data-stu-id="0cd38-107">The target object can be either a one-time access review, or an instance of a recurring access review.</span></span>  <span data-ttu-id="0cd38-108">Decisões anteriores não são mais registradas, mas os revisores podem continuar a atualização decisões.</span><span class="sxs-lookup"><span data-stu-id="0cd38-108">Previous decisions are no longer recorded, but reviewers can continue to update decisions.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cd38-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="0cd38-109">Permissions</span></span>
<span data-ttu-id="0cd38-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cd38-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cd38-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cd38-112">Permission type</span></span>                        | <span data-ttu-id="0cd38-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cd38-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cd38-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cd38-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="0cd38-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cd38-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="0cd38-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cd38-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cd38-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cd38-117">Not supported.</span></span> |
|<span data-ttu-id="0cd38-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cd38-118">Application</span></span>                            | <span data-ttu-id="0cd38-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cd38-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cd38-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cd38-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/resetDecisions()
```
## <a name="request-headers"></a><span data-ttu-id="0cd38-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd38-121">Request headers</span></span>
| <span data-ttu-id="0cd38-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0cd38-122">Name</span></span>         | <span data-ttu-id="0cd38-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cd38-123">Type</span></span>        | <span data-ttu-id="0cd38-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cd38-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="0cd38-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cd38-125">Authorization</span></span> | <span data-ttu-id="0cd38-126">string</span><span class="sxs-lookup"><span data-stu-id="0cd38-126">string</span></span> | <span data-ttu-id="0cd38-127">Token de portador</span><span class="sxs-lookup"><span data-stu-id="0cd38-127">Bearer \{token\}.</span></span> <span data-ttu-id="0cd38-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0cd38-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cd38-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd38-129">Request body</span></span>
<span data-ttu-id="0cd38-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0cd38-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="0cd38-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cd38-131">Response</span></span>
<span data-ttu-id="0cd38-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cd38-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cd38-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cd38-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cd38-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cd38-135">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "reset_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/resetDecisions()
```
##### <a name="response"></a><span data-ttu-id="0cd38-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cd38-136">Response</span></span>
><span data-ttu-id="0cd38-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cd38-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Reset accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-reset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
