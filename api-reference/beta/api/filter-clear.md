---
title: 'Filter: clear'
description: Limpa o filtro na coluna determinada.
ms.openlocfilehash: ae71723ed3ca9074bb7a71ea131fd7103f3714af
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034912"
---
# <a name="filter-clear"></a><span data-ttu-id="a69f9-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="a69f9-103">Filter: clear</span></span>

> <span data-ttu-id="a69f9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a69f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a69f9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a69f9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a69f9-106">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="a69f9-106">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="a69f9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a69f9-107">Permissions</span></span>
<span data-ttu-id="a69f9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a69f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a69f9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a69f9-110">Permission type</span></span>      | <span data-ttu-id="a69f9-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a69f9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a69f9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a69f9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a69f9-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a69f9-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a69f9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a69f9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a69f9-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a69f9-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a69f9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a69f9-116">Application</span></span> | <span data-ttu-id="a69f9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a69f9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a69f9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a69f9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="a69f9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a69f9-119">Request headers</span></span>
| <span data-ttu-id="a69f9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a69f9-120">Name</span></span>       | <span data-ttu-id="a69f9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a69f9-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a69f9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a69f9-122">Authorization</span></span>  | <span data-ttu-id="a69f9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a69f9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a69f9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a69f9-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a69f9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a69f9-126">Response</span></span>

<span data-ttu-id="a69f9-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a69f9-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a69f9-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a69f9-129">Example</span></span>
<span data-ttu-id="a69f9-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a69f9-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a69f9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a69f9-131">Request</span></span>
<span data-ttu-id="a69f9-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a69f9-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="a69f9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a69f9-133">Response</span></span>
<span data-ttu-id="a69f9-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a69f9-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
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