---
title: 'workbookRange: columnsAfter'
description: Obtém um determinado número de colunas à direita do intervalo especificado.
author: lumine2008
ms.openlocfilehash: b80657c6afb7709049a1e0ccaa3c3b232f5501c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304232"
---
# <a name="workbookrange-columnsafter"></a><span data-ttu-id="b6627-103">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="b6627-103">workbookRange: columnsAfter</span></span>

<span data-ttu-id="b6627-104">Obtém um determinado número de colunas à direita do intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="b6627-104">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6627-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6627-105">Permissions</span></span>
<span data-ttu-id="b6627-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6627-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6627-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6627-108">Permission type</span></span>      | <span data-ttu-id="b6627-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6627-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6627-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6627-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b6627-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b6627-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="b6627-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6627-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6627-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6627-113">Not supported.</span></span>    |
|<span data-ttu-id="b6627-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6627-114">Application</span></span> | <span data-ttu-id="b6627-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6627-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6627-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6627-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="b6627-117">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="b6627-117">Function parameters</span></span>

| <span data-ttu-id="b6627-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b6627-118">Parameter</span></span>    | <span data-ttu-id="b6627-119">Type</span><span class="sxs-lookup"><span data-stu-id="b6627-119">Type</span></span>   |<span data-ttu-id="b6627-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6627-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6627-121">Count</span><span class="sxs-lookup"><span data-stu-id="b6627-121">count</span></span>|<span data-ttu-id="b6627-122">Int32</span><span class="sxs-lookup"><span data-stu-id="b6627-122">Int32</span></span>|<span data-ttu-id="b6627-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b6627-123">Optional.</span></span> <span data-ttu-id="b6627-124">O número de colunas a serem incluídas no intervalo resultante.</span><span class="sxs-lookup"><span data-stu-id="b6627-124">The number of columns to include in the resulting range.</span></span> <span data-ttu-id="b6627-125">Em geral, use um número positivo para criar um intervalo de fora do intervalo atual.</span><span class="sxs-lookup"><span data-stu-id="b6627-125">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="b6627-126">Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual.</span><span class="sxs-lookup"><span data-stu-id="b6627-126">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="b6627-127">O valor padrão é 1</span><span class="sxs-lookup"><span data-stu-id="b6627-127">The default value is 1</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b6627-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6627-128">Request headers</span></span>
| <span data-ttu-id="b6627-129">Nome</span><span class="sxs-lookup"><span data-stu-id="b6627-129">Name</span></span>       | <span data-ttu-id="b6627-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6627-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b6627-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6627-131">Authorization</span></span>  | <span data-ttu-id="b6627-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6627-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b6627-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="b6627-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="b6627-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="b6627-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6627-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6627-137">Request body</span></span>
<span data-ttu-id="b6627-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6627-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6627-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6627-139">Response</span></span>
<span data-ttu-id="b6627-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6627-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6627-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6627-141">Example</span></span>
<span data-ttu-id="b6627-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b6627-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b6627-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6627-143">Request</span></span>
<span data-ttu-id="b6627-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6627-144">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_columnsafter",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="b6627-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6627-145">Response</span></span>
<span data-ttu-id="b6627-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6627-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
