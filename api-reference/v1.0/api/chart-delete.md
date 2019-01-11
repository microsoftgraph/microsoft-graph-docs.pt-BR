---
title: 'Chart: delete'
description: Exclui o objeto de gráfico.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 8b7eb6ff1d8a4d2eee16bdd0bcf9ce4a4c70b23a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871614"
---
# <a name="chart-delete"></a><span data-ttu-id="bacf1-103">Chart: delete</span><span class="sxs-lookup"><span data-stu-id="bacf1-103">Chart: delete</span></span>

<span data-ttu-id="bacf1-104">Exclui o objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="bacf1-104">Deletes the chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bacf1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bacf1-105">Permissions</span></span>
<span data-ttu-id="bacf1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bacf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bacf1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bacf1-108">Permission type</span></span>      | <span data-ttu-id="bacf1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bacf1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bacf1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bacf1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bacf1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bacf1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bacf1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bacf1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bacf1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bacf1-113">Not supported.</span></span>    |
|<span data-ttu-id="bacf1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bacf1-114">Application</span></span> | <span data-ttu-id="bacf1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bacf1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bacf1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bacf1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="bacf1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bacf1-117">Request headers</span></span>
| <span data-ttu-id="bacf1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bacf1-118">Name</span></span>       | <span data-ttu-id="bacf1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bacf1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bacf1-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bacf1-120">Authorization</span></span>  | <span data-ttu-id="bacf1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bacf1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bacf1-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="bacf1-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="bacf1-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bacf1-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bacf1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bacf1-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="bacf1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bacf1-127">Response</span></span>

<span data-ttu-id="bacf1-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bacf1-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bacf1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bacf1-130">Example</span></span>
<span data-ttu-id="bacf1-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="bacf1-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bacf1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bacf1-132">Request</span></span>
<span data-ttu-id="bacf1-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bacf1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/delete
```

##### <a name="response"></a><span data-ttu-id="bacf1-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bacf1-134">Response</span></span>
<span data-ttu-id="bacf1-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bacf1-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
