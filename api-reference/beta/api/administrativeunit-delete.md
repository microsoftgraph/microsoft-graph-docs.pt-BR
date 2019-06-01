---
title: Excluir administrativeUnit
description: Excluir um administrativeUnit.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 84718cfe855db3bda5e4e9a72ecf73565a3873e6
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655422"
---
# <a name="delete-administrativeunit"></a><span data-ttu-id="3a5e5-103">Excluir administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="3a5e5-103">Delete administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a5e5-104">Excluir um [administrativeUnit](../resources/administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="3a5e5-104">Delete an [administrativeUnit](../resources/administrativeunit.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3a5e5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a5e5-105">Permissions</span></span>
<span data-ttu-id="3a5e5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a5e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3a5e5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a5e5-108">Permission type</span></span>      | <span data-ttu-id="3a5e5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a5e5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a5e5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a5e5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3a5e5-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a5e5-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3a5e5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a5e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a5e5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a5e5-113">Not supported.</span></span>    |
|<span data-ttu-id="3a5e5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a5e5-114">Application</span></span> | <span data-ttu-id="3a5e5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a5e5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a5e5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a5e5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3a5e5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a5e5-117">Request headers</span></span>
| <span data-ttu-id="3a5e5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3a5e5-118">Name</span></span>       | <span data-ttu-id="3a5e5-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a5e5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3a5e5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a5e5-120">Authorization</span></span>  | <span data-ttu-id="3a5e5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a5e5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a5e5-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a5e5-123">Request body</span></span>
<span data-ttu-id="3a5e5-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a5e5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a5e5-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a5e5-125">Response</span></span>

<span data-ttu-id="3a5e5-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a5e5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a5e5-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a5e5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a5e5-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a5e5-129">Request</span></span>
<span data-ttu-id="3a5e5-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a5e5-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_administrativeunit"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}
```
##### <a name="response"></a><span data-ttu-id="3a5e5-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a5e5-131">Response</span></span>
<span data-ttu-id="3a5e5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a5e5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3a5e5-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3a5e5-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3a5e5-136">C#</span><span class="sxs-lookup"><span data-stu-id="3a5e5-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_administrativeunit-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3a5e5-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="3a5e5-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_administrativeunit-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
