---
title: 'Worksheet: delete'
description: Exclui a planilha da pasta de trabalho.
author: lumine2008
ms.openlocfilehash: 37a87ecbefbb88afb30a6cb773e03775c4de36b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318981"
---
# <a name="worksheet-delete"></a><span data-ttu-id="fe5be-103">Worksheet: delete</span><span class="sxs-lookup"><span data-stu-id="fe5be-103">Worksheet: delete</span></span>

> <span data-ttu-id="fe5be-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fe5be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe5be-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fe5be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe5be-106">Exclui a planilha da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="fe5be-106">Deletes the worksheet from the workbook.</span></span>
## <a name="permissions"></a><span data-ttu-id="fe5be-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe5be-107">Permissions</span></span>
<span data-ttu-id="fe5be-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe5be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe5be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe5be-110">Permission type</span></span>      | <span data-ttu-id="fe5be-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe5be-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe5be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe5be-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fe5be-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe5be-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fe5be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe5be-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe5be-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe5be-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fe5be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe5be-116">Application</span></span> | <span data-ttu-id="fe5be-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe5be-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe5be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe5be-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="fe5be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe5be-119">Request headers</span></span>
| <span data-ttu-id="fe5be-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fe5be-120">Name</span></span>       | <span data-ttu-id="fe5be-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe5be-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fe5be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe5be-122">Authorization</span></span>  | <span data-ttu-id="fe5be-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe5be-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe5be-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fe5be-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="fe5be-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="fe5be-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe5be-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe5be-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="fe5be-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe5be-129">Response</span></span>

<span data-ttu-id="fe5be-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe5be-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe5be-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe5be-132">Example</span></span>
<span data-ttu-id="fe5be-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fe5be-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fe5be-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe5be-134">Request</span></span>
<span data-ttu-id="fe5be-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe5be-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheet_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/worksheets/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="fe5be-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe5be-136">Response</span></span>
<span data-ttu-id="fe5be-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe5be-137">Here is an example of the response.</span></span> 
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
  "description": "Worksheet: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->