---
title: 'TableSort: reapply'
description: Reaplica os parâmetros de classificação atuais à tabela.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 7cb1631e56a9badcd9dea3708504c0848c9ee81d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520197"
---
# <a name="tablesort-reapply"></a><span data-ttu-id="303d0-103">TableSort: reapply</span><span class="sxs-lookup"><span data-stu-id="303d0-103">TableSort: reapply</span></span>

<span data-ttu-id="303d0-104">Reaplica os parâmetros de classificação atuais à tabela.</span><span class="sxs-lookup"><span data-stu-id="303d0-104">Reapplies the current sorting parameters to the table.</span></span>
## <a name="permissions"></a><span data-ttu-id="303d0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="303d0-105">Permissions</span></span>
<span data-ttu-id="303d0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="303d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="303d0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="303d0-108">Permission type</span></span>      | <span data-ttu-id="303d0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="303d0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="303d0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="303d0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="303d0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="303d0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="303d0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="303d0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="303d0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="303d0-113">Not supported.</span></span>    |
|<span data-ttu-id="303d0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="303d0-114">Application</span></span> | <span data-ttu-id="303d0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="303d0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="303d0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="303d0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/reapply
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/reapply

```
## <a name="request-headers"></a><span data-ttu-id="303d0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="303d0-117">Request headers</span></span>
| <span data-ttu-id="303d0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="303d0-118">Name</span></span>       | <span data-ttu-id="303d0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="303d0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="303d0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="303d0-120">Authorization</span></span>  | <span data-ttu-id="303d0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="303d0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="303d0-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="303d0-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="303d0-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="303d0-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="303d0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="303d0-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="303d0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="303d0-127">Response</span></span>

<span data-ttu-id="303d0-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="303d0-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="303d0-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="303d0-130">Example</span></span>
<span data-ttu-id="303d0-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="303d0-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="303d0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="303d0-132">Request</span></span>
<span data-ttu-id="303d0-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="303d0-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_reapply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply
```

##### <a name="response"></a><span data-ttu-id="303d0-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="303d0-134">Response</span></span>
<span data-ttu-id="303d0-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="303d0-135">Here is an example of the response.</span></span> 
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
  "description": "TableSort: reapply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
