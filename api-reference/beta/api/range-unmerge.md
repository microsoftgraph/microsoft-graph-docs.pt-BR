---
title: 'Range: unmerge'
description: Desfaz a mesclagem das células do intervalo em células separadas.
author: lumine2008
ms.openlocfilehash: 65192bedaa1f61f3e6b66bc5a593ba7c2d8b31f6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357187"
---
# <a name="range-unmerge"></a><span data-ttu-id="3a3f2-103">Range: unmerge</span><span class="sxs-lookup"><span data-stu-id="3a3f2-103">Range: unmerge</span></span>

> <span data-ttu-id="3a3f2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3a3f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a3f2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3a3f2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a3f2-106">Desfaz a mesclagem das células do intervalo em células separadas.</span><span class="sxs-lookup"><span data-stu-id="3a3f2-106">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a3f2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a3f2-107">Permissions</span></span>
<span data-ttu-id="3a3f2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a3f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a3f2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a3f2-110">Permission type</span></span>      | <span data-ttu-id="3a3f2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a3f2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a3f2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a3f2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a3f2-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a3f2-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3a3f2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a3f2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a3f2-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3a3f2-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="3a3f2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a3f2-116">Application</span></span> | <span data-ttu-id="3a3f2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a3f2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a3f2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a3f2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/unmerge
POST /workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="3a3f2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a3f2-119">Request headers</span></span>
| <span data-ttu-id="3a3f2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3a3f2-120">Name</span></span>       | <span data-ttu-id="3a3f2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a3f2-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3a3f2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a3f2-122">Authorization</span></span>  | <span data-ttu-id="3a3f2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a3f2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a3f2-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3a3f2-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="3a3f2-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3a3f2-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a3f2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a3f2-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3a3f2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a3f2-129">Response</span></span>

<span data-ttu-id="3a3f2-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a3f2-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a3f2-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a3f2-132">Example</span></span>
<span data-ttu-id="3a3f2-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3a3f2-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3a3f2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a3f2-134">Request</span></span>
<span data-ttu-id="3a3f2-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a3f2-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/unmerge
```

##### <a name="response"></a><span data-ttu-id="3a3f2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a3f2-136">Response</span></span>
<span data-ttu-id="3a3f2-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3a3f2-137">Here is an example of the response.</span></span> 
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
  "description": "Range: unmerge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->