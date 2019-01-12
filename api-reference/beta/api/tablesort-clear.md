---
title: 'TableSort: clear'
description: Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 1503b2b47935f8cdb1367bd5518c3bbc648f94c4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962818"
---
# <a name="tablesort-clear"></a><span data-ttu-id="d3eae-104">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="d3eae-104">TableSort: clear</span></span>

> <span data-ttu-id="d3eae-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d3eae-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3eae-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d3eae-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3eae-p103">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="d3eae-p103">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3eae-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3eae-109">Permissions</span></span>
<span data-ttu-id="d3eae-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3eae-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3eae-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3eae-112">Permission type</span></span>      | <span data-ttu-id="d3eae-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3eae-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3eae-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3eae-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d3eae-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3eae-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d3eae-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3eae-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3eae-117">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3eae-117">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d3eae-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3eae-118">Application</span></span> | <span data-ttu-id="d3eae-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3eae-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3eae-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3eae-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="d3eae-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3eae-121">Request headers</span></span>
| <span data-ttu-id="d3eae-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d3eae-122">Name</span></span>       | <span data-ttu-id="d3eae-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3eae-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d3eae-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3eae-124">Authorization</span></span>  | <span data-ttu-id="d3eae-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3eae-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3eae-127">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d3eae-127">Workbook-Session-Id</span></span>  | <span data-ttu-id="d3eae-p106">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d3eae-p106">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3eae-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3eae-130">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d3eae-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3eae-131">Response</span></span>

<span data-ttu-id="d3eae-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3eae-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3eae-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d3eae-134">Example</span></span>
<span data-ttu-id="d3eae-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d3eae-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d3eae-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3eae-136">Request</span></span>
<span data-ttu-id="d3eae-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3eae-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="d3eae-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3eae-138">Response</span></span>
<span data-ttu-id="d3eae-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3eae-139">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
