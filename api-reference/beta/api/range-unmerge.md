---
title: 'Range: unmerge'
description: Desfaz a mesclagem das células do intervalo em células separadas.
ms.openlocfilehash: 99b8cd596e49e4386ebeb995c3c5fa590ddcb4e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040448"
---
# <a name="range-unmerge"></a><span data-ttu-id="259ac-103">Range: unmerge</span><span class="sxs-lookup"><span data-stu-id="259ac-103">Range: unmerge</span></span>

> <span data-ttu-id="259ac-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="259ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="259ac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="259ac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="259ac-106">Desfaz a mesclagem das células do intervalo em células separadas.</span><span class="sxs-lookup"><span data-stu-id="259ac-106">Unmerge the range cells into separate cells.</span></span>
## <a name="permissions"></a><span data-ttu-id="259ac-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="259ac-107">Permissions</span></span>
<span data-ttu-id="259ac-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="259ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="259ac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="259ac-110">Permission type</span></span>      | <span data-ttu-id="259ac-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="259ac-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="259ac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="259ac-112">Delegated (work or school account)</span></span> | <span data-ttu-id="259ac-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="259ac-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="259ac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="259ac-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="259ac-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="259ac-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="259ac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="259ac-116">Application</span></span> | <span data-ttu-id="259ac-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="259ac-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="259ac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="259ac-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/unmerge
POST /workbook/worksheets/{id|name}/range(address='<address>')/unmerge
POST /workbook/tables/{id|name}/columns/{id|name}/range/unmerge

```
## <a name="request-headers"></a><span data-ttu-id="259ac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="259ac-119">Request headers</span></span>
| <span data-ttu-id="259ac-120">Nome</span><span class="sxs-lookup"><span data-stu-id="259ac-120">Name</span></span>       | <span data-ttu-id="259ac-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="259ac-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="259ac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="259ac-122">Authorization</span></span>  | <span data-ttu-id="259ac-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="259ac-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="259ac-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="259ac-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="259ac-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="259ac-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="259ac-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="259ac-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="259ac-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="259ac-129">Response</span></span>

<span data-ttu-id="259ac-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="259ac-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="259ac-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="259ac-132">Example</span></span>
<span data-ttu-id="259ac-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="259ac-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="259ac-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="259ac-134">Request</span></span>
<span data-ttu-id="259ac-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="259ac-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_unmerge"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/unmerge
```

##### <a name="response"></a><span data-ttu-id="259ac-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="259ac-136">Response</span></span>
<span data-ttu-id="259ac-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="259ac-137">Here is an example of the response.</span></span> 
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