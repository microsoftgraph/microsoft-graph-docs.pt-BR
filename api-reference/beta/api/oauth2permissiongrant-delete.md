---
title: Excluir oAuth2PermissionGrant
description: Excluir um oAuth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: 240462c1c20e3fc3d8ea55c95e348f6c7a7f53a7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597269"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="7ef30-103">Excluir oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="7ef30-103">Delete oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ef30-104">Excluir um oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="7ef30-104">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ef30-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7ef30-105">Permissions</span></span>
<span data-ttu-id="7ef30-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ef30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7ef30-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ef30-108">Permission type</span></span>      | <span data-ttu-id="7ef30-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7ef30-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ef30-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ef30-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7ef30-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7ef30-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7ef30-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ef30-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ef30-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ef30-113">Not supported.</span></span>    |
|<span data-ttu-id="7ef30-114">Application</span><span class="sxs-lookup"><span data-stu-id="7ef30-114">Application</span></span> | <span data-ttu-id="7ef30-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ef30-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ef30-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ef30-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7ef30-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ef30-117">Request headers</span></span>
| <span data-ttu-id="7ef30-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7ef30-118">Name</span></span>       | <span data-ttu-id="7ef30-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ef30-119">Type</span></span> | <span data-ttu-id="7ef30-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ef30-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ef30-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ef30-121">Authorization</span></span>  | <span data-ttu-id="7ef30-122">string</span><span class="sxs-lookup"><span data-stu-id="7ef30-122">string</span></span>  | <span data-ttu-id="7ef30-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ef30-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ef30-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ef30-125">Request body</span></span>
<span data-ttu-id="7ef30-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7ef30-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ef30-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ef30-127">Response</span></span>

<span data-ttu-id="7ef30-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ef30-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ef30-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ef30-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ef30-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ef30-131">Request</span></span>
<span data-ttu-id="7ef30-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ef30-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="7ef30-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ef30-133">Response</span></span>
<span data-ttu-id="7ef30-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ef30-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7ef30-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="7ef30-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7ef30-136">Basic</span><span class="sxs-lookup"><span data-stu-id="7ef30-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_oAuth2Permissiongrant-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ef30-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ef30-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_oAuth2Permissiongrant-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/oauth2permissiongrant-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
