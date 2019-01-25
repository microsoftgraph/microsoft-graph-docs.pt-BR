---
title: Excluir accessReview
description: No Windows Azure AD para acessar o recurso de revisões, excluir um objeto accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 28848cc047306259248d0ba4663ab3eb3e964224
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527770"
---
# <a name="delete-accessreview"></a><span data-ttu-id="d5987-103">Excluir accessReview</span><span class="sxs-lookup"><span data-stu-id="d5987-103">Delete accessReview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5987-104">No recurso de [acesso analisa](../resources/accessreviews-root.md) Azure AD, exclua um objeto de [accessReview](../resources/accessreview.md) .</span><span class="sxs-lookup"><span data-stu-id="d5987-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete an [accessReview](../resources/accessreview.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d5987-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5987-105">Permissions</span></span>
<span data-ttu-id="d5987-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5987-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5987-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5987-108">Permission type</span></span>                        | <span data-ttu-id="d5987-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5987-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5987-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5987-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5987-111">AccessReview.ReadWrite.All e também devem ter ProgramControl.ReadWrite.All ao cenário completo com uma chamada para excluir um programControl</span><span class="sxs-lookup"><span data-stu-id="d5987-111">AccessReview.ReadWrite.All, and should also have ProgramControl.ReadWrite.All to complete scenario with a call to delete a programControl</span></span> |
|<span data-ttu-id="d5987-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5987-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5987-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5987-113">Not supported.</span></span> |
|<span data-ttu-id="d5987-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5987-114">Application</span></span>                            | <span data-ttu-id="d5987-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5987-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5987-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5987-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /accessReviews('<id>')
```
## <a name="request-headers"></a><span data-ttu-id="d5987-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5987-117">Request headers</span></span>
| <span data-ttu-id="d5987-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d5987-118">Name</span></span>         | <span data-ttu-id="d5987-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5987-119">Type</span></span>        | <span data-ttu-id="d5987-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5987-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d5987-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5987-121">Authorization</span></span> | <span data-ttu-id="d5987-122">string</span><span class="sxs-lookup"><span data-stu-id="d5987-122">string</span></span> | <span data-ttu-id="d5987-123">Token de portador</span><span class="sxs-lookup"><span data-stu-id="d5987-123">Bearer \{token\}.</span></span> <span data-ttu-id="d5987-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5987-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5987-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5987-125">Request body</span></span>
<span data-ttu-id="d5987-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5987-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d5987-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5987-127">Response</span></span>
<span data-ttu-id="d5987-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5987-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5987-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5987-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5987-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5987-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessReview"
}-->
```http
DELETE https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')
```
##### <a name="response"></a><span data-ttu-id="d5987-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5987-132">Response</span></span>
><span data-ttu-id="d5987-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5987-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
