---
title: 'Filter: clear'
description: Limpa o filtro na coluna determinada.
localization_priority: Normal
ms.openlocfilehash: bea500516e898fbbad2bbb881be437004405fb84
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524152"
---
# <a name="filter-clear"></a><span data-ttu-id="4b812-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="4b812-103">Filter: clear</span></span>

<span data-ttu-id="4b812-104">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="4b812-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="4b812-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b812-105">Permissions</span></span>
<span data-ttu-id="4b812-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b812-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b812-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b812-108">Permission type</span></span>      | <span data-ttu-id="4b812-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b812-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b812-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b812-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b812-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b812-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4b812-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b812-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b812-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b812-113">Not supported.</span></span>    |
|<span data-ttu-id="4b812-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b812-114">Application</span></span> | <span data-ttu-id="4b812-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b812-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b812-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b812-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="4b812-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b812-117">Request headers</span></span>
| <span data-ttu-id="4b812-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4b812-118">Name</span></span>       | <span data-ttu-id="4b812-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b812-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4b812-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b812-120">Authorization</span></span>  | <span data-ttu-id="4b812-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b812-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b812-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b812-123">Request body</span></span>
<span data-ttu-id="4b812-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b812-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b812-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b812-125">Response</span></span>

<span data-ttu-id="4b812-p103">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b812-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b812-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b812-128">Example</span></span>
<span data-ttu-id="4b812-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4b812-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4b812-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b812-130">Request</span></span>
<span data-ttu-id="4b812-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b812-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="4b812-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b812-132">Response</span></span>
<span data-ttu-id="4b812-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b812-133">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
