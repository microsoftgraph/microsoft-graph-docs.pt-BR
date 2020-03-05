---
title: 'Chart: delete'
description: Exclui o objeto de gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: fe2298b24c4ba2c229fa8344baf120295e0d4773
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440070"
---
# <a name="chart-delete"></a><span data-ttu-id="0aa7e-103">Chart: delete</span><span class="sxs-lookup"><span data-stu-id="0aa7e-103">Chart: delete</span></span>

<span data-ttu-id="0aa7e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0aa7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aa7e-105">Exclui o objeto de gráfico.</span><span class="sxs-lookup"><span data-stu-id="0aa7e-105">Deletes the chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0aa7e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0aa7e-106">Permissions</span></span>
<span data-ttu-id="0aa7e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0aa7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0aa7e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0aa7e-109">Permission type</span></span>      | <span data-ttu-id="0aa7e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0aa7e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0aa7e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0aa7e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0aa7e-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0aa7e-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0aa7e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0aa7e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0aa7e-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0aa7e-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0aa7e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0aa7e-115">Application</span></span> | <span data-ttu-id="0aa7e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0aa7e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0aa7e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0aa7e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="0aa7e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0aa7e-118">Request headers</span></span>
| <span data-ttu-id="0aa7e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0aa7e-119">Name</span></span>       | <span data-ttu-id="0aa7e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0aa7e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0aa7e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0aa7e-121">Authorization</span></span>  | <span data-ttu-id="0aa7e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0aa7e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0aa7e-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0aa7e-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="0aa7e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0aa7e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0aa7e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0aa7e-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0aa7e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0aa7e-128">Response</span></span>

<span data-ttu-id="0aa7e-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0aa7e-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0aa7e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0aa7e-131">Example</span></span>
<span data-ttu-id="0aa7e-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0aa7e-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0aa7e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0aa7e-133">Request</span></span>
<span data-ttu-id="0aa7e-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0aa7e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/delete
```

##### <a name="response"></a><span data-ttu-id="0aa7e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="0aa7e-135">Response</span></span>
<span data-ttu-id="0aa7e-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0aa7e-136">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "Chart: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
