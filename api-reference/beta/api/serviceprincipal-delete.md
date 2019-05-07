---
title: Excluir o servicePrincipalName
description: Exclua o servicePrincipalName.
localization_priority: Normal
ms.openlocfilehash: 224ebf07dbe569add6f8a47d08d0be6f4d53e379
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638827"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="bccb2-103">Excluir o servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="bccb2-103">Delete servicePrincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bccb2-104">Exclua o servicePrincipalName.</span><span class="sxs-lookup"><span data-stu-id="bccb2-104">Delete servicePrincipal.</span></span>
## <a name="permissions"></a><span data-ttu-id="bccb2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bccb2-105">Permissions</span></span>
<span data-ttu-id="bccb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bccb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bccb2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bccb2-108">Permission type</span></span>      | <span data-ttu-id="bccb2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bccb2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bccb2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bccb2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bccb2-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bccb2-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bccb2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bccb2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bccb2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bccb2-113">Not supported.</span></span>    |
|<span data-ttu-id="bccb2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bccb2-114">Application</span></span> | <span data-ttu-id="bccb2-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bccb2-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bccb2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bccb2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="bccb2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bccb2-117">Request headers</span></span>
| <span data-ttu-id="bccb2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bccb2-118">Name</span></span>       | <span data-ttu-id="bccb2-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="bccb2-119">Type</span></span> | <span data-ttu-id="bccb2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bccb2-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bccb2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bccb2-121">Authorization</span></span>  | <span data-ttu-id="bccb2-122">string</span><span class="sxs-lookup"><span data-stu-id="bccb2-122">string</span></span>  | <span data-ttu-id="bccb2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bccb2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bccb2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bccb2-125">Request body</span></span>
<span data-ttu-id="bccb2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bccb2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bccb2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bccb2-127">Response</span></span>

<span data-ttu-id="bccb2-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bccb2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bccb2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bccb2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bccb2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bccb2-131">Request</span></span>
<span data-ttu-id="bccb2-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bccb2-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
##### <a name="response"></a><span data-ttu-id="bccb2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bccb2-133">Response</span></span>
<span data-ttu-id="bccb2-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bccb2-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bccb2-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="bccb2-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bccb2-136">Basic</span><span class="sxs-lookup"><span data-stu-id="bccb2-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_serviceprincipal-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bccb2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bccb2-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_serviceprincipal-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
