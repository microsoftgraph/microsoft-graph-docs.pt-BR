---
title: 'workbookPivotTable: atualizar'
description: Atualiza a Tabela Dinâmica.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3238f67fc7f017e64ab327619a4f4f90fba71d1f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534672"
---
# <a name="workbookpivottable-refresh"></a><span data-ttu-id="171b3-103">workbookPivotTable: atualizar</span><span class="sxs-lookup"><span data-stu-id="171b3-103">workbookPivotTable: refresh</span></span>

<span data-ttu-id="171b3-104">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="171b3-104">Refreshes the PivotTable.</span></span>


## <a name="permissions"></a><span data-ttu-id="171b3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="171b3-105">Permissions</span></span>
<span data-ttu-id="171b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="171b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="171b3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="171b3-108">Permission type</span></span>      | <span data-ttu-id="171b3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="171b3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="171b3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="171b3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="171b3-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="171b3-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="171b3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="171b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="171b3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="171b3-113">Not supported.</span></span>    |
|<span data-ttu-id="171b3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="171b3-114">Application</span></span> | <span data-ttu-id="171b3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="171b3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="171b3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="171b3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```
## <a name="request-headers"></a><span data-ttu-id="171b3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="171b3-117">Request headers</span></span>
| <span data-ttu-id="171b3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="171b3-118">Name</span></span>       | <span data-ttu-id="171b3-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="171b3-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="171b3-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="171b3-120">Authorization</span></span>  | <span data-ttu-id="171b3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="171b3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="171b3-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="171b3-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="171b3-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="171b3-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="171b3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="171b3-126">Request body</span></span>

### <a name="response"></a><span data-ttu-id="171b3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="171b3-127">Response</span></span>
<span data-ttu-id="171b3-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="171b3-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="171b3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="171b3-130">Example</span></span>
<span data-ttu-id="171b3-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="171b3-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="171b3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="171b3-132">Request</span></span>
<span data-ttu-id="171b3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="171b3-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="171b3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="171b3-134">Response</span></span>
<span data-ttu-id="171b3-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="171b3-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
