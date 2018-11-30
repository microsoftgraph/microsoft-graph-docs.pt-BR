---
title: 'TableRow: delete'
description: Exclui a linha da tabela.
ms.openlocfilehash: a2202daf9a645a16a7ea6287edf468e12d829e9a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038663"
---
# <a name="tablerow-delete"></a><span data-ttu-id="d824d-103">TableRow: delete</span><span class="sxs-lookup"><span data-stu-id="d824d-103">TableRow: delete</span></span>

> <span data-ttu-id="d824d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d824d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d824d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d824d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d824d-106">Exclui a linha da tabela.</span><span class="sxs-lookup"><span data-stu-id="d824d-106">Deletes the row from the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="d824d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d824d-107">Permissions</span></span>
<span data-ttu-id="d824d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d824d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d824d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d824d-110">Permission type</span></span>      | <span data-ttu-id="d824d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d824d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d824d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d824d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d824d-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d824d-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d824d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d824d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d824d-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d824d-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d824d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d824d-116">Application</span></span> | <span data-ttu-id="d824d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d824d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d824d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d824d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/rows(<index>)/delete
POST /workbook/worksheets/{id|name}/tables/{id|name}/rows(<index>)/delete

```
## <a name="request-headers"></a><span data-ttu-id="d824d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d824d-119">Request headers</span></span>
| <span data-ttu-id="d824d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d824d-120">Name</span></span>       | <span data-ttu-id="d824d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d824d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d824d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d824d-122">Authorization</span></span>  | <span data-ttu-id="d824d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d824d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d824d-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d824d-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="d824d-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d824d-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d824d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d824d-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d824d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d824d-129">Response</span></span>

<span data-ttu-id="d824d-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d824d-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d824d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d824d-132">Example</span></span>
<span data-ttu-id="d824d-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d824d-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d824d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d824d-134">Request</span></span>
<span data-ttu-id="d824d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d824d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablerow_delete"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/rows(<index>)/delete
```

##### <a name="response"></a><span data-ttu-id="d824d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d824d-136">Response</span></span>
<span data-ttu-id="d824d-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d824d-137">Here is an example of the response.</span></span> 
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
  "description": "TableRow: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->